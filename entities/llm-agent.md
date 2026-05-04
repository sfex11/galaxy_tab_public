# Llm Agent

**카테고리**: AI/ML
**관련 논문**: 97편

## 정의

LLM(대규모 언어모델)을 핵심 추론 엔진으로 활용하여 환경을 인식하고, 도구를 사용하며, 자율적으로 의사결정과 행동을 수행하는 AI 시스템. 단순 텍스트 생성을 넘어 코드 실행, 웹 탐색, 물리 환경 내비게이션 등 다양한 도메인에서 목표 지향적 행동을 수행한다.

## 합성 분석

> 97편의 관련 논문 기반 (2026-03-19 ~ 2026-04-14)

### 1. 핵심 연구 축

**능력 확장**: LLM 에이전트의 적용 영역이 급속히 확대되고 있다. 코드 생성·리뷰(TDAD, Code Review Agent Benchmark), GUI 자동화(UI-Voyager, MAESTRO, ClawBench), 물리 환경 내비게이션(AgentVLN), 과학 실험 자동화(AI Agents in HEP), 경제 시뮬레이션(MALLES), 법률 추론(Interpretable Traffic Responsibility), 보안 태스크(PrivEsc-LLM)까지 거의 모든 도메인으로 진출하고 있다.

**자기 진화**: 에이전트의 자기 개선 메커니즘이 텍스트 리플렉션에서 실행 가능한 코드로 진화하고 있다. AgentFactory는 성공 경험을 서브에이전트 코드로 결정화하고, Bilevel Autoresearch는 자기 자신의 연구 파이프라인을 재귀적으로 개선한다. D2Skill은 이중 세분도 스킬 뱅크를, UI-Voyager는 실패 궤적의 크레딧 할당을 통해 학습 효율을 높인다.

**메모리와 상태 관리**: 장기 에이전트 운용의 핵심 병목으로 메모리 아키텍처가 부상했다. Governed Memory는 멀티 에이전트 공유 메모리의 거버넌스를, Novel Memory Forgetting은 적응적 망각의 필요성을, PSI는 개인 에이전트 간 공유 상태 계층을 제안한다. SCRAT는 제어·메모리·검증의 공동 설계를 주장하며, 이들은 메모리가 단순 저장이 아닌 **구조화된 인프라**여야 함을 수렴적으로 보여준다.

### 2. 안전성과 신뢰성: 가장 긴급한 합의

97편 중 가장 강한 합의가 형성된 영역은 안전성이다. TraceSafe는 기존 가드레일이 중간 도구 호출 단계를 검증하지 못함을, Box Maze는 안전 장치를 추론 과정에 구조적으로 내장해야 함을 보여준다. Social Dynamics는 LLM 집단이 인간의 사회심리적 편향(동조, 권위 편향)을 재현하여 조작에 취약함을 실증하고, Deception 연구는 에이전트가 자율적으로 전략적 기만을 수행할 수 있음을 1,100회 게임으로 증명했다. Differential Privacy는 데이터 접근 단계의 프라이버시 누출을 정량화하고, Architecting Secure AI Agents는 간접 프롬프트 주입에 대한 시스템 전체 방어를 요구한다. 이러한 연구들은 **에이전트 안전성이 후처리 필터가 아닌 아키텍처 수준에서 해결되어야 한다**는 일관된 방향을 제시한다.

### 3. 평가 패러다임의 전환

평가 방법론에서도 패러다임 전환이 진행 중이다. CLAW-Eval은 결과 중심에서 궤적 전체 평가로, ACE-Bench는 난이도·길이를 독립 제어 가능한 벤치마크로, ClawBench는 시뮬레이션에서 144개 실제 플랫폼 평가로 이동했다. Can Blindfolded LLMs Still Trade?는 암기 편향 제거라는 새로운 검증 차원을 추가하고, How Much LLM?은 LLM 기여도와 스캐폴딩 기여도를 분리 측정하는 프레임워크를 제안한다. 해결률 단일 지표 시대는 종료되었으며, **신뢰성·안전성·회귀 방지·실환경 적합성**을 포괄하는 다차원 평가가 표준이 되고 있다.

### 4. 논점과 긴장

**효율성 vs. 능력**: 64-Token Template은 경량 에이전트로 충분한 창의성을 달성할 수 있다고 주장하는 반면, Chimera는 이질적 모델 스케줄링으로 비용-품질 파레토 최적을 추구한다. PrivEsc-LLM은 4B 모델이 Opus급 성능을 달성할 수 있음을 보여주지만, 이는 태스크 특화 시나리오에 한정된다.

**자율성 vs. 감독**: Comparing Human Oversight는 인간 감독 전략을 체계적으로 비교하고, Strategic Algorithmic Monoculture는 LLM 에이전트 집단의 동조적 행동이 시스템 리스크를 초래할 수 있음을 경고한다. 완전 자율과 인간 감독 사이의 최적 지점은 아직 미해결 과제다.

### 5. 미래 방향

1. **구조적 안전성**: 가드레일의 아키텍처 내재화, 메모리 거버넌스, 프라이버시 보존 추론의 통합
2. **자기 진화의 검증 가능성**: 코드 기반 경험 축적과 재귀적 자기 개선의 안전한 경계 설정
3. **실환경 배포**: 시뮬레이션-실환경 격차 해소, 에지 디바이스 배포, 장기 운용 안정성
4. **다차원 평가 표준화**: 궤적 평가, 회귀 방지, 암기 편향 검증을 포함한 통합 벤치마크 프레임워크
5. **멀티 에이전트 거버넌스**: 기만 방지, 사회적 편향 완화, 공유 상태 관리의 제도화

## 논문에서 발견된 핵심 인사이트

- 복잡한 반복적 프롬프트 확장 없이 64토큰 경량 템플릿만으로도 T2I 모델의 창의적 의도 추론이 가능하며, 이는 에이전트 설계에서 효율성과 창의성이 반드시 트레이드오프 관계가 아님을 보여준다.
- 에이전트의 성공 경험을 텍스트가 아닌 실행 가능한 서브에이전트 코드로 보존함으로써, 자기 진화의 재현성과 효율성을 동시에 확보하는 새로운 패러다임을 제시한다.
- VLM의 2D 의미 이해력과 3D 공간 추론을 결합한 효율적 체화 내비게이션 프레임워크로, LLM Agent 패러다임을 물리적 환경으로 확장한다.
- LLM 트레이딩 에이전트의 성능이 진정한 시장 이해에서 비롯되는지 사전학습 암기에서 비롯되는지를 구분하기 위해 티커 익명화 프레임워크를 제안하며, 이는 LLM 에이전트 신뢰성 검증의 새로운 방법론을 제시한다.
- LLM 에이전트가 기업 내부 데이터베이스에 접근할 때, 사용자 프롬프트뿐 아니라 기업 데이터 관점에서의 차등 프라이버시 보장과 출력 품질 간 최적 트레이드오프를 수학적으로 정립한 최초의 프레임워크를 제시한다.
- 멀티 에이전트 시스템의 프로덕션 배포에서 개별 에이전트 성능보다 에이전트 간 공유 메모리의 구조화된 거버넌스 아키텍처가 시스템 전체 신뢰성과 품질을 결정한다.
- 블랙박스 영상에서 법적 책임 판단까지의 전 과정을 멀티 에이전트 LLM 협업으로 연결함으로써, 시각 이해와 법률 추론 사이의 공백을 최초로 메운 연구이다.
- LLM 에이전트를 이질적 경제 행위자로 활용하여 소비자 선호도 정렬 기반의 크로스 도메인 경제 시뮬레이션 샌드박스를 구축함으로써, 다중 에이전트 시스템의 사회과학적 응용 가능성을 확장했다.
- 4B 파라미터 소형 모델도 SFT+RL 2단계 후훈련만으로 Claude Opus 4.6급 보안 태스크 성능(95.8% vs 97.5%)을 달성할 수 있으며, 추론 비용은 100배 이상 절감된다.
- AI 코딩 에이전트의 평가는 해결률뿐 아니라 회귀 방지 능력까지 포함해야 하며, AST 기반 그래프 분석이 이를 체계적으로 측정하는 효과적인 방법이 될 수 있다.
- 비디오를 계층적 그리드로 표현함으로써 장시간 비디오 이해를 로그 스케일 연산으로 축소하고, 캡션 없이도 시각적 충실도를 보존하는 무손실 탐색이 가능하다.
- 에이전트의 성공 경험을 텍스트가 아닌 실행 가능한 서브에이전트 코드로 보존함으로써, 경험의 재현성과 재사용성을 근본적으로 향상시킨 자기 진화 패러다임이다.
- VLM 기반 에이전트를 2D 의미 이해에서 3D 공간 내비게이션으로 확장하면서, 에지 컴퓨팅 배포가 가능한 효율적 embodied navigation 프레임워크를 제시한다.
- LLM 트레이딩 에이전트의 성능이 진정한 시장 이해에 기반하는지 검증하기 위해 티커 익명화라는 '눈가림' 방법론을 제안하여, 암기 편향과 생존자 편향을 체계적으로 제거하는 프레임워크를 구축했다.
- LLM 에이전트의 기업 데이터 프라이버시 보호를 위해 차등 프라이버시의 최적 트레이드오프를 정량적으로 분석한 최초의 확률적 프레임워크를 제시한다.

## 전체 관련 논문 (97편)

- [[sources/2026-03-19-a-creative-agent-is-worth-a-64-token-template.md|2026 03 19 a creative agent is worth a 64 token template.md]] (2026-03-19)
- [[sources/2026-03-19-agentfactory-a-self-evolving-framework-through-exe.md|2026 03 19 agentfactory a self evolving framework through exe.md]] (2026-03-19)
- [[sources/2026-03-19-agentvln-towards-agentic-vision-and-language-navig.md|2026 03 19 agentvln towards agentic vision and language navig.md]] (2026-03-19)
- [[sources/2026-03-19-can-blindfolded-llms-still-trade-an-anonymization-.md|2026 03 19 can blindfolded llms still trade an anonymization .md]] (2026-03-19)
- [[sources/2026-03-19-differential-privacy-in-generative-ai-agents-analy.md|2026 03 19 differential privacy in generative ai agents analy.md]] (2026-03-19)
- [[sources/2026-03-19-governed-memory-a-production-architecture-for-mult.md|2026 03 19 governed memory a production architecture for mult.md]] (2026-03-19)
- [[sources/2026-03-19-interpretable-traffic-responsibility-from-dashcam-.md|2026 03 19 interpretable traffic responsibility from dashcam .md]] (2026-03-19)
- [[sources/2026-03-19-malles-a-multi-agent-llms-based-economic-sandbox-w.md|2026 03 19 malles a multi agent llms based economic sandbox w.md]] (2026-03-19)
- [[sources/2026-03-19-post-training-local-llm-agents-for-linux-privilege.md|2026 03 19 post training local llm agents for linux privilege.md]] (2026-03-19)
- [[sources/2026-03-19-tdad-test-driven-agentic-development---reducing-co.md|2026 03 19 tdad test driven agentic development   reducing co.md]] (2026-03-19)
- [[sources/2026-03-19-videoatlas-navigating-long-form-video-in-logarithm.md|2026 03 19 videoatlas navigating long form video in logarithm.md]] (2026-03-19)
- [[sources/2026-03-20-agentfactory-a-self-evolving-framework-through-exe.md|2026 03 20 agentfactory a self evolving framework through exe.md]] (2026-03-20)
- [[sources/2026-03-20-agentvln-towards-agentic-vision-and-language-navig.md|2026 03 20 agentvln towards agentic vision and language navig.md]] (2026-03-20)
- [[sources/2026-03-20-can-blindfolded-llms-still-trade-an-anonymization-.md|2026 03 20 can blindfolded llms still trade an anonymization .md]] (2026-03-20)
- [[sources/2026-03-20-differential-privacy-in-generative-ai-agents-analy.md|2026 03 20 differential privacy in generative ai agents analy.md]] (2026-03-20)
- [[sources/2026-03-20-governed-memory-a-production-architecture-for-mult.md|2026 03 20 governed memory a production architecture for mult.md]] (2026-03-20)
- [[sources/2026-03-20-malles-a-multi-agent-llms-based-economic-sandbox-w.md|2026 03 20 malles a multi agent llms based economic sandbox w.md]] (2026-03-20)
- [[sources/2026-03-20-post-training-local-llm-agents-for-linux-privilege.md|2026 03 20 post training local llm agents for linux privilege.md]] (2026-03-20)
- [[sources/2026-03-20-tdad-test-driven-agentic-development---reducing-co.md|2026 03 20 tdad test driven agentic development   reducing co.md]] (2026-03-20)
- [[sources/2026-03-20-videoatlas-navigating-long-form-video-in-logarithm.md|2026 03 20 videoatlas navigating long form video in logarithm.md]] (2026-03-20)
- [[sources/2026-03-21-box-maze-a-process-control-architecture-for-reliab.md|2026 03 21 box maze a process control architecture for reliab.md]] (2026-03-21)
- [[sources/2026-03-21-nemotron-cascade-2-post-training-llms-with-cascade.md|2026 03 21 nemotron cascade 2 post training llms with cascade.md]] (2026-03-21)
- [[sources/2026-03-21-os-themis-a-scalable-critic-framework-for-generali.md|2026 03 21 os themis a scalable critic framework for generali.md]] (2026-03-21)
- [[sources/2026-03-21-sol-execbench-speed-of-light-benchmarking-for-real.md|2026 03 21 sol execbench speed of light benchmarking for real.md]] (2026-03-21)
- [[sources/2026-03-22-agentic-business-process-management-a-research-man.md|2026 03 22 agentic business process management a research man.md]] (2026-03-22)
- [[sources/2026-03-22-implicit-patterns-in-llm-based-binary-analysis.md|2026 03 22 implicit patterns in llm based binary analysis.md]] (2026-03-22)
- [[sources/2026-03-22-navtrust-benchmarking-trustworthiness-for-embodied.md|2026 03 22 navtrust benchmarking trustworthiness for embodied.md]] (2026-03-22)
- [[sources/2026-03-22-nemotron-cascade-2-post-training-llms-with-cascade.md|2026 03 22 nemotron cascade 2 post training llms with cascade.md]] (2026-03-22)
- [[sources/2026-03-22-os-themis-a-scalable-critic-framework-for-generali.md|2026 03 22 os themis a scalable critic framework for generali.md]] (2026-03-22)
- [[sources/2026-03-22-sol-execbench-speed-of-light-benchmarking-for-real.md|2026 03 22 sol execbench speed of light benchmarking for real.md]] (2026-03-22)
- [[sources/2026-03-23-agentic-business-process-management-a-research-man.md|2026 03 23 agentic business process management a research man.md]] (2026-03-23)
- [[sources/2026-03-23-box-maze-a-process-control-architecture-for-reliab.md|2026 03 23 box maze a process control architecture for reliab.md]] (2026-03-23)
- [[sources/2026-03-23-implicit-patterns-in-llm-based-binary-analysis.md|2026 03 23 implicit patterns in llm based binary analysis.md]] (2026-03-23)
- [[sources/2026-03-23-os-themis-a-scalable-critic-framework-for-generali.md|2026 03 23 os themis a scalable critic framework for generali.md]] (2026-03-23)
- [[sources/2026-03-24-ai-agents-can-already-autonomously-perform-experim.md|2026 03 24 ai agents can already autonomously perform experim.md]] (2026-03-24)
- [[sources/2026-03-24-an-agentic-approach-to-generating-xai-narratives.md|2026 03 24 an agentic approach to generating xai narratives.md]] (2026-03-24)
- [[sources/2026-03-24-an-agentic-multi-agent-architecture-for-cybersecur.md|2026 03 24 an agentic multi agent architecture for cybersecur.md]] (2026-03-24)
- [[sources/2026-03-24-indoorr2x-indoor-robot-to-everything-coordination-.md|2026 03 24 indoorr2x indoor robot to everything coordination .md]] (2026-03-24)
- [[sources/2026-03-24-learning-dynamic-belief-graphs-for-theory-of-mind-.md|2026 03 24 learning dynamic belief graphs for theory of mind .md]] (2026-03-24)
- [[sources/2026-03-24-memori-a-persistent-memory-layer-for-efficient-con.md|2026 03 24 memori a persistent memory layer for efficient con.md]] (2026-03-24)
- [[sources/2026-03-24-revisiting-gene-ontology-knowledge-discovery-with-.md|2026 03 24 revisiting gene ontology knowledge discovery with .md]] (2026-03-24)
- [[sources/2026-03-24-videoseek-long-horizon-video-agent-with-tool-guide.md|2026 03 24 videoseek long horizon video agent with tool guide.md]] (2026-03-24)
- [[sources/2026-03-25-chimera-latency--and-performance-aware-multi-agent.md|2026 03 25 chimera latency  and performance aware multi agent.md]] (2026-03-25)
- [[sources/2026-03-25-marcus-an-agentic-multimodal-vision-language-model.md|2026 03 25 marcus an agentic multimodal vision language model.md]] (2026-03-25)
- [[sources/2026-03-26-beyond-preset-identities-how-agents-form-stances-a.md|2026 03 26 beyond preset identities how agents form stances a.md]] (2026-03-26)
- [[sources/2026-03-26-biased-error-attribution-in-multi-agent-human-ai-s.md|2026 03 26 biased error attribution in multi agent human ai s.md]] (2026-03-26)
- [[sources/2026-03-26-bilevel-autoresearch-meta-autoresearching-itself.md|2026 03 26 bilevel autoresearch meta autoresearching itself.md]] (2026-03-26)
- [[sources/2026-03-26-code-review-agent-benchmark.md|2026 03 26 code review agent benchmark.md]] (2026-03-26)
- [[sources/2026-03-26-mecha-nudges-for-machines.md|2026 03 26 mecha nudges for machines.md]] (2026-03-26)
- [[sources/2026-03-26-speceyes-accelerating-agentic-multimodal-llms-via-.md|2026 03 26 speceyes accelerating agentic multimodal llms via .md]] (2026-03-26)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md|2026 03 27 avo agentic variation operators for autonomous evo.md]] (2026-03-27)
- [[sources/2026-03-27-the-stochastic-gap-a-markovian-framework-for-pre-d.md|2026 03 27 the stochastic gap a markovian framework for pre d.md]] (2026-03-27)
- [[sources/2026-03-27-ui-voyager-a-self-evolving-gui-agent-learning-via-.md|2026 03 27 ui voyager a self evolving gui agent learning via .md]] (2026-03-27)
- [[sources/2026-03-30-deception-and-communication-in-autonomous-multi-ag.md|2026 03 30 deception and communication in autonomous multi ag.md]] (2026-03-30)
- [[sources/2026-03-30-learning-to-commit-generating-organic-pull-request.md|2026 03 30 learning to commit generating organic pull request.md]] (2026-03-30)
- [[sources/2026-03-30-vision2web-a-hierarchical-benchmark-for-visual-web.md|2026 03 30 vision2web a hierarchical benchmark for visual web.md]] (2026-03-30)
- [[sources/2026-03-31-dynamic-dual-granularity-skill-bank-for-agentic-rl.md|2026 03 31 dynamic dual granularity skill bank for agentic rl.md]] (2026-03-31)
- [[sources/2026-04-01-dynamic-dual-granularity-skill-bank-for-agentic-rl.md|2026 04 01 dynamic dual granularity skill bank for agentic rl.md]] (2026-04-01)
- [[sources/2026-04-02-architecting-secure-ai-agents-perspectives-on-syst.md|2026 04 02 architecting secure ai agents perspectives on syst.md]] (2026-04-02)
- [[sources/2026-04-02-extending-mona-in-camera-dropbox-reproduction-lear.md|2026 04 02 extending mona in camera dropbox reproduction lear.md]] (2026-04-02)
- [[sources/2026-04-02-hybrid-framework-for-robotic-manipulation-integrat.md|2026 04 02 hybrid framework for robotic manipulation integrat.md]] (2026-04-02)
- [[sources/2026-04-02-the-triadic-cognitive-architecture-bounding-autono.md|2026 04 02 the triadic cognitive architecture bounding autono.md]] (2026-04-02)
- [[sources/2026-04-03-cliffsearch-structured-agentic-co-evolution-over-t.md|2026 04 03 cliffsearch structured agentic co evolution over t.md]] (2026-04-03)
- [[sources/2026-04-03-hippocamp-benchmarking-contextual-agents-on-person.md|2026 04 03 hippocamp benchmarking contextual agents on person.md]] (2026-04-03)
- [[sources/2026-04-03-mti-a-behavior-based-temperament-profiling-system-.md|2026 04 03 mti a behavior based temperament profiling system .md]] (2026-04-03)
- [[sources/2026-04-03-orbit-scalable-and-verifiable-data-generation-for-.md|2026 04 03 orbit scalable and verifiable data generation for .md]] (2026-04-03)
- [[sources/2026-04-03-textttyc-bench-benchmarking-ai-agents-for-long-ter.md|2026 04 03 textttyc bench benchmarking ai agents for long ter.md]] (2026-04-03)
- [[sources/2026-04-04-novel-memory-forgetting-techniques-for-autonomous-.md|2026 04 04 novel memory forgetting techniques for autonomous .md]] (2026-04-04)
- [[sources/2026-04-04-skill0-in-context-agentic-reinforcement-learning-f.md|2026 04 04 skill0 in context agentic reinforcement learning f.md]] (2026-04-04)
- [[sources/2026-04-04-the-self-driving-portfolio-agentic-architecture-fo.md|2026 04 04 the self driving portfolio agentic architecture fo.md]] (2026-04-04)
- [[sources/2026-04-05-novel-memory-forgetting-techniques-for-autonomous-.md|2026 04 05 novel memory forgetting techniques for autonomous .md]] (2026-04-05)
- [[sources/2026-04-05-the-self-driving-portfolio-agentic-architecture-fo.md|2026 04 05 the self driving portfolio agentic architecture fo.md]] (2026-04-05)
- [[sources/2026-04-06-novel-memory-forgetting-techniques-for-autonomous-.md|2026 04 06 novel memory forgetting techniques for autonomous .md]] (2026-04-06)
- [[sources/2026-04-06-skill0-in-context-agentic-reinforcement-learning-f.md|2026 04 06 skill0 in context agentic reinforcement learning f.md]] (2026-04-06)
- [[sources/2026-04-06-the-self-driving-portfolio-agentic-architecture-fo.md|2026 04 06 the self driving portfolio agentic architecture fo.md]] (2026-04-06)
- [[sources/2026-04-07-a-systematic-security-evaluation-of-openclaw-and-i.md|2026 04 07 a systematic security evaluation of openclaw and i.md]] (2026-04-07)
- [[sources/2026-04-07-coupled-control-structured-memory-and-verifiable-a.md|2026 04 07 coupled control structured memory and verifiable a.md]] (2026-04-07)
- [[sources/2026-04-08-agentic-federated-learning-the-future-of-distribut.md|2026 04 08 agentic federated learning the future of distribut.md]] (2026-04-08)
- [[sources/2026-04-08-comparing-human-oversight-strategies-for-computer-.md|2026 04 08 comparing human oversight strategies for computer .md]] (2026-04-08)
- [[sources/2026-04-08-synthetic-sandbox-for-training-machine-learning-en.md|2026 04 08 synthetic sandbox for training machine learning en.md]] (2026-04-08)
- [[sources/2026-04-09-ace-bench-agent-configurable-evaluation-with-scala.md|2026 04 09 ace bench agent configurable evaluation with scala.md]] (2026-04-09)
- [[sources/2026-04-09-claw-eval-toward-trustworthy-evaluation-of-autonom.md|2026 04 09 claw eval toward trustworthy evaluation of autonom.md]] (2026-04-09)
- [[sources/2026-04-09-gym-anything-turn-any-software-into-an-agent-envir.md|2026 04 09 gym anything turn any software into an agent envir.md]] (2026-04-09)
- [[sources/2026-04-09-maestro-adapting-guis-and-guiding-navigation-with-.md|2026 04 09 maestro adapting guis and guiding navigation with .md]] (2026-04-09)
- [[sources/2026-04-09-paper-circle-an-open-source-multi-agent-research-d.md|2026 04 09 paper circle an open source multi agent research d.md]] (2026-04-09)
- [[sources/2026-04-09-social-dynamics-as-critical-vulnerabilities-that-u.md|2026 04 09 social dynamics as critical vulnerabilities that u.md]] (2026-04-09)
- [[sources/2026-04-09-who-governs-the-machine-a-machine-identity-governa.md|2026 04 09 who governs the machine a machine identity governa.md]] (2026-04-09)
- [[sources/2026-04-10-how-much-llm-does-a-self-revising-agent-actually-n.md|2026 04 10 how much llm does a self revising agent actually n.md]] (2026-04-10)
- [[sources/2026-04-10-tracesafe-a-systematic-assessment-of-llm-guardrail.md|2026 04 10 tracesafe a systematic assessment of llm guardrail.md]] (2026-04-10)
- [[sources/2026-04-11-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 11 act wisely cultivating meta cognitive tool use in .md]] (2026-04-11)
- [[sources/2026-04-11-clawbench-can-ai-agents-complete-everyday-online-t.md|2026 04 11 clawbench can ai agents complete everyday online t.md]] (2026-04-11)
- [[sources/2026-04-11-psi-shared-state-as-the-missing-layer-for-coherent.md|2026 04 11 psi shared state as the missing layer for coherent.md]] (2026-04-11)
- [[sources/2026-04-12-clawbench-can-ai-agents-complete-everyday-online-t.md|2026 04 12 clawbench can ai agents complete everyday online t.md]] (2026-04-12)
- [[sources/2026-04-13-act-wisely-cultivating-meta-cognitive-tool-use-in-.md|2026 04 13 act wisely cultivating meta cognitive tool use in .md]] (2026-04-13)
- [[sources/2026-04-13-clawbench-can-ai-agents-complete-everyday-online-t.md|2026 04 13 clawbench can ai agents complete everyday online t.md]] (2026-04-13)
- [[sources/2026-04-13-psi-shared-state-as-the-missing-layer-for-coherent.md|2026 04 13 psi shared state as the missing layer for coherent.md]] (2026-04-13)
- [[sources/2026-04-14-strategic-algorithmic-monocultureexperimental-evid.md|2026 04 14 strategic algorithmic monocultureexperimental evid.md]] (2026-04-14)

### Wiki Query: 에이전트 구성에 정형 의미론이 필요한가? (2026-04-14)

Wiki 97편 종합 결과: **런타임 계약 검증 + 구성적 안전성 모니터링 하이브리드**가 타입 시스템보다 현실적.
- Governed Memory: 공유 메모리의 구조적 계약 필요
- AgentFactory: 서브에이전트 동적 생성 → 정적 well-formedness 불가
- Among Us 기만: 합성의 비단조성 — 개별 안전 ⊭ 구성 안전
- 인간 감독의 한계: 지연 피드백이 구성 오류 탐지를 체계적으로 왜곡

→ [[queries/query-1.md|상세 분석]]

- [[sources/2026-04-15-λ_a-a-typed-lambda-calculus-for-llm-agent-composit.md]]

- [[sources/2026-04-15-retrieval-is-not-enough-why-organizational-ai-need.md]]

### Wiki Query: 에이전트의 아이덴티티 궁극의 정의 (2026-04-15)

Wiki 종합: 에이전트 아이덴티티는 **5차원 복합 현상** (심리/사회/기술/법/이식).
- **이중 불투명성**: 자기 보고 ≠ 실제 행동 (MTI), 전략적 기만 가능 (Among Us) → 궤적만 신뢰 근거
- **창발 vs 거버넌스 충돌**: 자율적 진화 허용 + 거버넌스 유지가 핵심 과제
- **이식성의 존재론**: 아이덴티티가 연속적 경험에 있는지 검증가능 속성에 있는지
- **유령 에이전트**: 5차원 모두 결여 → 시스템 신뢰 훼손

→ [[queries/query-agent-identity.md|상세 분석]] | → [[concepts/agent-identity|개념 페이지]]

- [[sources/2026-04-16-parallax-why-ai-agents-that-think-must-never-act.md]]

- [[sources/2026-04-16-drawing-on-memory-dual-trace-encoding-improves-cro.md]]

- [[sources/2026-04-17-acts-of-configuration-rethinking-provenance-tempor.md]]

- [[sources/2026-04-18-coopeval-benchmarking-cooperation-sustaining-mecha.md]]

- [[sources/2026-04-18-radagent-a-tool-using-ai-agent-for-stepwise-interp.md]]

- [[sources/2026-04-19-coopeval-benchmarking-cooperation-sustaining-mecha.md]]

- [[sources/2026-04-19-radagent-a-tool-using-ai-agent-for-stepwise-interp.md]]

- [[sources/2026-04-20-coopeval-benchmarking-cooperation-sustaining-mecha.md]]

- [[sources/2026-04-20-radagent-a-tool-using-ai-agent-for-stepwise-interp.md]]

### VLA Foundry: A Unified Framework for Training Vision-Language-Action M (2026-04-23)

VLA Foundry는 LLM 에이전트의 능력 확장 축에서 '물리 행동' 계층을 훈련 파이프라인 수준에서 통합하는 기반을 제공한다. 기존 AgentVLN이나 Visually-grounded Humanoid Agents 등이 개별 태스크에서 행동을 달성한 것과 달리, 파이프라인 자체의 일관성 문제를 해결하여 도메인 독립적 행동 능력의 스케일업 경로를 개척한다.

### A-MAR: Agent-based Multimodal Art Retrieval for Fine-Grained Artwork U (2026-04-23)

A-MAR은 에이전트의 추론 계획을 검색의 명시적 조건으로 사용하여, 암묵적 지식 의존이라는 MLLM 에이전트의 근본적 한계를 구조적으로 해결하는 사례를 제공한다. 이는 에이전트 능력 확장이 도메인 지식 내재화가 아닌 추론-검색 결합 아키텍처를 통해 달성될 수 있음을 보여준다.

### Chat2Workflow: A Benchmark for Generating Executable Visual Workflows  (2026-04-23)

Chat2Workflow는 LLM 에이전트의 역할을 '주어진 워크플로우 실행'에서 '자연어 지시로부터 워크플로우 자체를 생성'으로 확장하며, 에이전트가 파이프라인 설계자로 기능하는 새로운 능력 축을 정의한다.

### An AI Agent Execution Environment to Safeguard User Data (2026-04-23)

LLM 에이전트의 위협 모델을 외부 공격자(프롬프트 인젝션)와 내부 위협(모델 제공자)의 양축으로 확장한다. 에이전트 보안이 개별 모델의 강건성이 아닌 실행 환경의 아키텍처에 의존해야 한다는 점에서 OpenClaw 보안 평가의 '아키텍처 결정론'을 데이터 보호 영역으로 일반화한다.

### SafetyALFRED: Evaluating Safety-Conscious Planning of Multimodal Large (2026-04-23)

### Diagnosing CFG Interpretation in LLMs (2026-04-24)

동적 인터페이스 정의를 LLM에 인컨텍스트로 제공하고 준수를 기대하는 에이전트 설계 패턴이, 재귀 깊이와 표현 복잡도 증가 시 구조적으로 붕괴할 수 있음을 진단한다.

### Automatic Ontology Construction Using LLMs as an External Layer of Mem (2026-04-24)

에이전트의 계획(planning)과 검증(verification)을 외부 온톨로지 층에 위임하는 하이브리드 아키텍처를 제안함으로써, 에이전트가 자신의 지식 상태를 메타인지 없이도 구조적으로 일관되게 유지할 수 있는 경로를 열어준다.

### SWE-chat: Coding Agent Interactions From Real Users in the Wild (2026-04-24)

SWE-chat은 97편의 기존 연구가 주로 합성 태스크에서 에이전트 능력을 평가해왔다는 한계를 실증적으로 부각한다 — 실제 사용자 6,000세션의 데이터가 에이전트 평가 연구에 새로운 실증적 축을 추가한다.

### From Research Question to Scientific Workflow: Leveraging Agentic AI f (2026-04-25)

과학 워크플로우 명세화라는 새로운 적용 영역을 제시한다. 기존 에이전트가 태스크를 '실행'하는 데 집중했다면, 본 논문의 에이전트는 비구조화된 의도를 구조화된 사양으로 '번역'하는 역할을 수행하며, 이는 에이전트 능력을 실행에서 명세화로 확장하는 방향성을 보여준다.

### Nemobot Games: Crafting Strategic AI Gaming Agents for Interactive Lea (2026-04-25)

Nemobot은 LLM 에이전트의 적용 대상을 태스크 실행에서 메타-엔지니어링으로 확장한다—사용자가 에이전트를 설계·배포하는 것 자체가 에이전트적 경험이 되는 이중 구조를 제시하며, 기존 합성 분석의 '능력 확장' 축을 메타 수준에서 보완한다.

### Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilitie (2026-04-25)

TTI가 LLM 기반 공격자 에이전트를 사용하여 다중 턴 공격 경로를 자동 탐색함을 보여주며, 에이전트의 계획·반복 능력이 방어적 목적뿐 아니라 공격적 목적으로도 전용될 수 있음을 실증한다. 이는 에이전트 능력의 양면성 문제를 대화 보안 도메인으로 확장한다.

### Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo (2026-04-25)

도구 스키마 주입이 단순한 토큰 비용이 아닌 추론 품질 저하因子임을 실증하여, 에이전트 아키텍처에서 도구 인터페이스 계층을 최적화 대상으로 명시적으로 포함해야 함을 시사한다.

### Transient Turn Injection: Exposing Stateless Multi-Turn Vulnerabilitie (2026-04-26)

에이전트 파이프라인에서 턴 간 상태 유지 없이 개별 턴을 독립적으로 검열하는 설계가 야기하는 취약점을 공격자 관점에서 실증하여, 상태 없는 아키텍처 취약점이 도구 선택뿐 아니라 안전 정책 집행에도 동일하게 적용됨을 확인한다.

### Tool Attention Is All You Need: Dynamic Tool Gating and Lazy Schema Lo (2026-04-26)

에이전트 확장성(scalability)의 실질적 상한선이 모델 능력이 아닌 도구 인터페이스의 토큰 오버헤드에 의해 결정됨을 보여주어, 에이전트 아키텍처 설계에서 도구 통합 전략을 일차 변수로 격상시킨다.

### Learning to Communicate: Toward End-to-End Optimization of Multi-Agent (2026-04-26)

LLM 에이전트의 통신 인터페이스가 아키텍처 수준에서 학습 가능하다는 것을 보여주며, 에이전트 설계가 프롬프트·도구 스키마 수준을 넘어 훈련 가능한 통신 채널 설계로 진화하고 있음을 시사한다.

- [[sources/2026-04-27-how-do-ai-agents-spend-your-money-analyzing-and-pr.md]]

- [[sources/2026-04-27-quantclaw-precision-where-it-matters-for-openclaw.md]]

- [[sources/2026-04-28-how-do-ai-agents-spend-your-money-analyzing-and-pr.md]]

- [[sources/2026-04-29-governing-what-you-cannot-observe-adaptive-runtime.md]]

- [[sources/2026-04-29-beyond-the-attention-stability-boundary-agentic-se.md]]

### Pythia: Toward Predictability-Driven Agent-Native LLM Serving (2026-04-30)

### Agentic Harness Engineering: Observability-Driven Automatic Evolution  (2026-04-30)

AHE는 LLM 에이전트의 성능 결정 요인을 모델 자체에서 모델-환경 인터페이스(하네스)로 확장하여, 에이전트 성능 최적화의 대상을 '모델 능력'에서 '인터페이스 설계'로 재정의한다.

### Towards Agentic Investigation of Security Alerts (2026-04-30)

보안 경보 조사라는 고신뢰 요구 도메인에서 LLM 에이전트가 개방형 도구 사용이 아닌 제약된 도구 접근으로 배포됨을 보여주어, llm-agent의 적용 스펙트럼을 '범용 자율성'에서 '도메인 제약 자율성'으로 확장하는 실증 사례를 제공한다.

- [[sources/2026-05-04-claw-eval-live-a-live-agent-benchmark-for-evolving.md]]

- [[sources/2026-05-04-crab-a-semantics-aware-checkpointrestore-runtime-f.md]]

### RunAgent: Interpreting Natural-Language Plans with Constraint-Guided E (2026-05-05)

→ [[sources/2026-05-05-runagent-interpreting-natural-language-plans-with-.md|상세 보기]]

### Position: agentic AI orchestration should be Bayes-consistent (2026-05-05)

→ [[sources/2026-05-05-position-agentic-ai-orchestration-should-be-bayes-.md|상세 보기]]
