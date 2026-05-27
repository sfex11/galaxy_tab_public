# OrpQuant: Geometric Orthogonal Residual Projection for Multiplier-Free Power-of-Two Transformer Quantization

**타입**: 논문
**출처**: arXiv
**날짜**: 2026-05-27
**링크**: http://arxiv.org/abs/2605.26092v1

## 💡 핵심 인사이트

OrpQuant의 핵심은 기존 래티스 수정법이 '어떤 래티스를 쓸 것인가'와 '잔여를 어디에 투영할 것인가'를 분리한 데 있다. 기존 방법들은 래티스의 기하 기하 방향(저각 해상도가 낮은 방향)을 개선하려 래치스를 수정하여 근본 원인(차원별 각도 간극의 합)에 의존하지만, OrpQuant는 래치스를 그대로 유지하고 잔여를 기하급 방향의 직교 보완 공간으로 투영함으로써합 문제(저각 해상도)와 해결 방법(직교 투영)을 독립적으로 해결한다. 이는 `marginal-distribution-ceiling`과 `algorithm-system-translation-gap`의 교차점에서, 시스템 층별 문제(MAC 비효율)를 알고리즘적 해결하는 완벽한 사례다.

## 📖 분석

# Power-of-Two 양자화의 각도 분해: OrpQuant의 기하-저각 투영

## 정의

Power-of-Two (PoT) 양자화는 비균일 지수 래티스에서 MAC 연산을 비트 시프트로 대체하여 하드웨어 효율을 달성하지만, 초저 비트(2-bit 등) 영역에서 **저각 해상도(Low Angular Resolution, LAR)** 문제가 극명적으로 나타난다. OrpQuant은 이를 **기하급 기하 방향 저각 투영(GORP)**으로 해결한다.

## 문제 진단: PoT의 각도 분해

PoT 양자화의 비균 일정 지수 래티스의 각도 해상도는 차원별 각도 간극의 합으로 상한이 정의되며, 비트 폭이 감소할수록 래티스의 표현력이 급격히 저하된다. 기존 해법들(GPTQ, QuIP 등)이 래티스 구조 자체를 수정(새로운 각도 해상도를 가진 래티스로 교체, QuIP)하려 시도, 수정 자체가 PoT의 하드웨어 효율 원리(비트 시프트만으로 MAC 대체)과 충돌하여 LAR 개선에 한계가 있다.
## 핵심 메커니즘: 기하급 기하 방향 저각 투영
OrpQuant의 핵심은 **"무엇을 어디에 투영할 것인가"와 "어떻게 투영할 것인가"를 분리하는 데 있다.

1. **문제의 기하 방향(LAR)**: 기존 방법들은 래티스의 기하 기하 방향(저각 해상도가 낮은 방향)을 개선하려 래치스를 수정한다. 그러나 이는 래치스를 새로운 것으로 교체하는 것이 아니라, 기존 구조의 한계 내에서 최적화하는 것이므로 근본 원인(차원별 각도 간극의 합)에 의존한다.
2. **해결의 기하 방향(GORP)**: OrpQuant는 래치스 구조를 그대로 유지하고, 양자화 잔여를 기하급 방향(각도 해상도가 높은 방향)의 직교 보완 공간으로 투영한다. 저각 해상도를 가진 방향의 직교 여분에 잔여를 투영하면, 기존 구조의 한계 내에서 표현력을 회복할 수 있다.
이것은 `marginal-distribution-ceiling`과 연결된다. OrpQuant는 PoT의 주변 분포 $P(y)$를 변경하지 않고 그 내부에서 최적화를 수행한다 — marginal distribution ceiling을 충족하면서 기존 방법들의 간극 원인(수정된 래티스가 구조 변경으로 인한 성능 저하)을 우회한다.
## 하드웨어 보장: 곱살형 직교 여부
GORP가 제안하는 직교 여부는 기하급 기하 방향의 차원을 정확하게 투영했는지에 달라 달라진다:
- **정확한 투영**: 기하급 기하 방향의 직교 여부가 래티스의 기하 기하 방향과 정확히 일치할 경우, 잔여는 래치스에서 기최적 효율을 달성한다.
- **부정확 투영**: 직교 여부가 불일치하면 잔여가 기하급 기하 방향의 저각 방향으로 누출되어 성능이 오히려질 수 있다.
- **과잡 투영**: 직교 여부가 과도하게 정확하면 잔여가 기하급 기하 방향의 고해상도를 누출하지 못해 LAR이 완화되지 않는다.
OrpQuant는 이를 직교 여부의 기하-저각 해상도 정합으로 공식화하고, 비용 선형 변환을 통해 정확한 투영을 보장한다.
## 수학적 근거: 각도 해상도의 상한 정리
비균 일정 지수 래티스의 각도 해상도는 차원별 각도 간극의 합으로 상한이 정의된다:
$$\theta_{\text{max}} \leq \sum_{i=1}^{d} \theta_i$$
OrpQuant는 이 한계를 엄밀하게 증명한다. GORP가 잔여를 기하급 방향의 저각 방향의 직교 여분에 투영하면, 잔여의 기하급 기하 방향 성분이 기하급 방향 저각 방향의 성분만큼만큼 회복되어, 차원 간극이 잔여에서 사라지는 방향으로 전이되지 않음을 보인다.
## 결과: 하드웨어 효율 유지, 다중 모델 일관성
OrpQuant는 LLaMA-3.1, LLaVA-1.5, Mistral-7B 등 다중 모델에서 2-bit에서 4-bit까지 기존 PoT 양자화 방법(GPTQ, QuIP)과 비교하여 동등 또는 우수의 성능을 달성한다. 특히 초저 비트 영역에서 기존 방법들이 극복적인 성능 저하를 보일 때, OrpQuant가 유의미한 성능 회복을 달성한다.
## `algorithm-system-translation-gap`과의 연결
OrpQuant는 `algorithm-system-translation-gap`의 완벽한 사례다. 기존 해법들은 문제를 "어떤 래티스를 쓸 것인가"로 재정의(== 알고리즘 개선을 위한 래티스 재설계)하여 시스템 층별 문제(== MAC 대비 비효율)를 야기한다. OrpQuant는 문제를 "잔여를 어디에 투영할 것인가"로 재정의(== 잔여 투영의 기하-저각 분리)하여 시스템 층별 문제를 해결한다.
## 한계
OrpQuant는 PoT 양자화의 하드웨어 효율을 유지하면서도 초저 비트 영역에서 근본적 각도 분해를 극복하지 못하는 한계가 있다. GORP가 저각 방향의 직교 여부를 판별하는 데 필요한 메타정(차원별 각도 간극의 합)가 초저 비트에서는 충분히 불확실하여, 완벽한 직교 판별이 불가능할 수 있다.

## 🏷️ 엔티티

- [[entities/low-angular-resolution.md|low-angular-resolution]]
- [[entities/geometric-orthogonal-residual-projection.md|geometric-orthogonal-residual-projection]]
- [[entities/power-of-two-quantization.md|power-of-two-quantization]]

## 📐 개념

- [[concepts/low-angular-resolution.md|low-angular-resolution]]

---
_LLM 분석으로 생성됨_
