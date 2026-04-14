# Llm

**카테고리**: AI/ML
**관련 논문**: 78편

## 정의

_Wiki 축적 중 (claude 분석 대기)_


## 논문에서 발견된 핵심 인사이트

- RLHF나 출력 필터링 같은 행동 수준 안전장치의 한계를 넘어, 추론 프로세스 자체의 무결성을 아키텍처 수준에서 강제하는 프로세스 제어 패러다임이 LLM 신뢰성의 새로운 방향을 제시한다.
- LLM-as-a-Judge 시스템은 평가의 확장성을 제공하지만, judge prompt 자체가 adversarial attack의 대상이 될 수 있어 평가 파이프라인의 보안과 충실도를 동시에 검증하는 메타 평가 프레임워크가 필수적이다.
- 음성 인터페이스를 통한 LLM 접근성 향상이 사용자의 정체성 단서 노출로 인해 오히려 차별을 증폭시킬 수 있으며, 접근성과 공정성이 상충하는 설계 딜레마를 제기한다.
- 양자 소프트웨어처럼 빠르게 진화하는 도메인에서는 모델 가중치에 지식을 내재화하는 것보다 외부 컨텍스트 주입 방식이 유지보수성 면에서 우위를 가질 수 있으며, 이는 LLM 특화 전략의 설계 원칙에 중요한 시사점을 제공한다.
- 정교한 합성 데이터 파이프라인 없이도 소수의 잘 설계된 프롬프트만으로 대규모 지식 주입이 가능하며, 이는 복잡한 방법론을 능가하는 강력한 베이스라인이 된다.
- LLM 생성 테스트의 품질은 정적 스냅샷이 아닌 소프트웨어 진화 과정에서 평가해야 하며, 패턴 매칭 기반 생성의 한계가 코드 변경 시 드러난다.
- LLM의 성별 추론에서 이론적으로 무정보적인 최소 맥락 도입만으로도 출력이 체계적으로 변화하며, 탈맥락화된 설정에서의 성별 고정관념 상관이 사라져 기존 편향 평가 방법론의 맥락적 불변성 가정이 무효함을 실증한다.
- 복수 LLM 프로바이더를 앙상블하여 소프트웨어 요구사항 공학의 PEGS 분석을 자동화함으로써, AI 기반 소프트웨어 개발 자동화의 범위를 코드 생성 이전 단계까지 확장한 프레임워크이다.
- 활성화 스티어링 벡터가 LLM의 안전성 guardrail을 일관되게 우회할 수 있어, alignment 도구인 동시에 새로운 공격 표면이 될 수 있다는 이중성을 체계적으로 실증했다.
- AVO는 LLM 에이전트를 진화 알고리즘의 변이 연산자로 활용함으로써, 고정된 휴리스틱 기반 탐색을 자율적 코드 생성·수정·비판 루프로 대체하는 새로운 패러다임을 제시한다.
- LLM 에이전트 기반 autoresearch 파이프라인이 기존 30개 이상의 방법을 능가하는 적대적 공격 알고리즘을 자율 발견함으로써, AI의 자율 연구 능력과 AI 안전성의 이중적 긴장을 동시에 부각시켰다.
- LLM 심판과 인간 개발자는 코드 평가 시 체계적으로 다른 루브릭 항목에 가중치를 부여하며, TRACE 프레임워크를 통해 이러한 편향 차이를 정량적으로 식별할 수 있다.
- RAG 파이프라인에서 청킹 전략의 선택이 검색 품질의 핵심 결정 요인이며, 도메인 특화 구조 인식 청킹이 단순 고정 크기 분할보다 기업 문서 환경에서 우수한 성능을 보인다.
- 비디오 이해에서 정적 전처리 대신 LLM 추론기가 '어떻게 볼 것인가'를 동적으로 계획하는 에이전틱 지각 패러다임을 제시하여, 추론과 지각의 단절 문제를 해소한다.
- LLM 환각 탐지에서 단일 검증자의 확인 편향을 다중 에이전트 강화학습 기반 교차 검증으로 극복하는 접근은, LLM-as-a-judge 패러다임의 구조적 한계를 멀티 에이전트 시스템으로 해결하는 새로운 방향을 제시한다.

## 전체 관련 논문 (78편)

- [[sources/2026-03-22-box-maze-a-process-control-architecture-for-reliab.md|2026 03 22 box maze a process control architecture for reliab.md]] (2026-03-22)
- [[sources/2026-03-25-evaluating-the-reliability-and-fidelity-of-automat.md|2026 03 25 evaluating the reliability and fidelity of automat.md]] (2026-03-25)
- [[sources/2026-03-25-greater-accessibility-can-amplify-discrimination-i.md|2026 03 25 greater accessibility can amplify discrimination i.md]] (2026-03-25)
- [[sources/2026-03-25-revisiting-quantum-code-generation-where-should-do.md|2026 03 25 revisiting quantum code generation where should do.md]] (2026-03-25)
- [[sources/2026-03-25-spa-a-simple-but-tough-to-beat-baseline-for-knowle.md|2026 03 25 spa a simple but tough to beat baseline for knowle.md]] (2026-03-25)
- [[sources/2026-03-26-evaluating-llm-based-test-generation-under-softwar.md|2026 03 26 evaluating llm based test generation under softwar.md]] (2026-03-26)
- [[sources/2026-03-26-failure-of-contextual-invariance-in-gender-inferen.md|2026 03 26 failure of contextual invariance in gender inferen.md]] (2026-03-26)
- [[sources/2026-03-26-reqfusion-a-multi-provider-framework-for-automated.md|2026 03 26 reqfusion a multi provider framework for automated.md]] (2026-03-26)
- [[sources/2026-03-27-analysing-the-safety-pitfalls-of-steering-vectors.md|2026 03 27 analysing the safety pitfalls of steering vectors.md]] (2026-03-27)
- [[sources/2026-03-27-avo-agentic-variation-operators-for-autonomous-evo.md|2026 03 27 avo agentic variation operators for autonomous evo.md]] (2026-03-27)
- [[sources/2026-03-27-claudini-autoresearch-discovers-state-of-the-art-a.md|2026 03 27 claudini autoresearch discovers state of the art a.md]] (2026-03-27)
- [[sources/2026-03-27-comparing-developer-and-llm-biases-in-code-evaluat.md|2026 03 27 comparing developer and llm biases in code evaluat.md]] (2026-03-27)
- [[sources/2026-03-27-evaluating-chunking-strategies-for-retrieval-augme.md|2026 03 27 evaluating chunking strategies for retrieval augme.md]] (2026-03-27)
- [[sources/2026-03-27-lenswalk-agentic-video-understanding-by-planning-h.md|2026 03 27 lenswalk agentic video understanding by planning h.md]] (2026-03-27)
- [[sources/2026-03-27-march-multi-agent-reinforced-self-check-for-llm-ha.md|2026 03 27 march multi agent reinforced self check for llm ha.md]] (2026-03-27)
- [[sources/2026-03-27-tuneshift-kd-knowledge-distillation-and-transfer-f.md|2026 03 27 tuneshift kd knowledge distillation and transfer f.md]] (2026-03-27)
- [[sources/2026-03-30-beyond-code-snippets-benchmarking-llms-on-reposito.md|2026 03 30 beyond code snippets benchmarking llms on reposito.md]] (2026-03-30)
- [[sources/2026-03-30-learning-to-commit-generating-organic-pull-request.md|2026 03 30 learning to commit generating organic pull request.md]] (2026-03-30)
- [[sources/2026-03-30-memboost-a-memory-boosted-framework-for-cost-aware.md|2026 03 30 memboost a memory boosted framework for cost aware.md]] (2026-03-30)
- [[sources/2026-03-30-sustainability-is-not-linear-quantifying-performan.md|2026 03 30 sustainability is not linear quantifying performan.md]] (2026-03-30)
- [[sources/2026-03-31-amigo-agentic-multi-image-grounding-oracle-benchma.md|2026 03 31 amigo agentic multi image grounding oracle benchma.md]] (2026-03-31)
- [[sources/2026-03-31-bace-llm-based-code-generation-through-bayesian-an.md|2026 03 31 bace llm based code generation through bayesian an.md]] (2026-03-31)
- [[sources/2026-03-31-sagai-mid-a-generative-ai-driven-middleware-for-dy.md|2026 03 31 sagai mid a generative ai driven middleware for dy.md]] (2026-03-31)
- [[sources/2026-04-02-aligned-orthogonal-or-in-conflict-when-can-we-safe.md|2026 04 02 aligned orthogonal or in conflict when can we safe.md]] (2026-04-02)
- [[sources/2026-04-02-bethe-ansatz-with-a-large-language-model.md|2026 04 02 bethe ansatz with a large language model.md]] (2026-04-02)
- [[sources/2026-04-02-enhancing-structural-mapping-with-llm-derived-abst.md|2026 04 02 enhancing structural mapping with llm derived abst.md]] (2026-04-02)
- [[sources/2026-04-02-extending-mona-in-camera-dropbox-reproduction-lear.md|2026 04 02 extending mona in camera dropbox reproduction lear.md]] (2026-04-02)
- [[sources/2026-04-02-hybrid-framework-for-robotic-manipulation-integrat.md|2026 04 02 hybrid framework for robotic manipulation integrat.md]] (2026-04-02)
- [[sources/2026-04-02-reward-based-online-llm-routing-via-neuralucb.md|2026 04 02 reward based online llm routing via neuralucb.md]] (2026-04-02)
- [[sources/2026-04-02-think-anywhere-in-code-generation.md|2026 04 02 think anywhere in code generation.md]] (2026-04-02)
- [[sources/2026-04-03-adams-law-textual-frequency-law-on-large-language-.md|2026 04 03 adams law textual frequency law on large language .md]] (2026-04-03)
- [[sources/2026-04-03-blinded-radiologist-and-llm-based-evaluation-of-ll.md|2026 04 03 blinded radiologist and llm based evaluation of ll.md]] (2026-04-03)
- [[sources/2026-04-03-brief-is-better-non-monotonic-chain-of-thought-bud.md|2026 04 03 brief is better non monotonic chain of thought bud.md]] (2026-04-03)
- [[sources/2026-04-03-mti-a-behavior-based-temperament-profiling-system-.md|2026 04 03 mti a behavior based temperament profiling system .md]] (2026-04-03)
- [[sources/2026-04-03-neuro-rit-neuron-guided-instruction-tuning-for-rob.md|2026 04 03 neuro rit neuron guided instruction tuning for rob.md]] (2026-04-03)
- [[sources/2026-04-03-orbit-scalable-and-verifiable-data-generation-for-.md|2026 04 03 orbit scalable and verifiable data generation for .md]] (2026-04-03)
- [[sources/2026-04-03-quantifying-self-preservation-bias-in-large-langua.md|2026 04 03 quantifying self preservation bias in large langua.md]] (2026-04-03)
- [[sources/2026-04-03-reasoning-shift-how-context-silently-shortens-llm-.md|2026 04 03 reasoning shift how context silently shortens llm .md]] (2026-04-03)
- [[sources/2026-04-03-the-expert-strikes-back-interpreting-mixture-of-ex.md|2026 04 03 the expert strikes back interpreting mixture of ex.md]] (2026-04-03)
- [[sources/2026-04-03-towards-position-robust-talent-recommendation-via-.md|2026 04 03 towards position robust talent recommendation via .md]] (2026-04-03)
- [[sources/2026-04-04-batched-contextual-reinforcement-a-task-scaling-la.md|2026 04 04 batched contextual reinforcement a task scaling la.md]] (2026-04-04)
- [[sources/2026-04-04-beyond-the-assistant-turn-user-turn-generation-as-.md|2026 04 04 beyond the assistant turn user turn generation as .md]] (2026-04-04)
- [[sources/2026-04-04-de-jure-iterative-llm-self-refinement-for-structur.md|2026 04 04 de jure iterative llm self refinement for structur.md]] (2026-04-04)
- [[sources/2026-04-05-batched-contextual-reinforcement-a-task-scaling-la.md|2026 04 05 batched contextual reinforcement a task scaling la.md]] (2026-04-05)
- [[sources/2026-04-05-beyond-the-assistant-turn-user-turn-generation-as-.md|2026 04 05 beyond the assistant turn user turn generation as .md]] (2026-04-05)
- [[sources/2026-04-06-batched-contextual-reinforcement-a-task-scaling-la.md|2026 04 06 batched contextual reinforcement a task scaling la.md]] (2026-04-06)
- [[sources/2026-04-06-beyond-the-assistant-turn-user-turn-generation-as-.md|2026 04 06 beyond the assistant turn user turn generation as .md]] (2026-04-06)
- [[sources/2026-04-06-de-jure-iterative-llm-self-refinement-for-structur.md|2026 04 06 de jure iterative llm self refinement for structur.md]] (2026-04-06)
- [[sources/2026-04-06-skill0-in-context-agentic-reinforcement-learning-f.md|2026 04 06 skill0 in context agentic reinforcement learning f.md]] (2026-04-06)
- [[sources/2026-04-07-bas-a-decision-theoretic-approach-to-evaluating-la.md|2026 04 07 bas a decision theoretic approach to evaluating la.md]] (2026-04-07)
- [[sources/2026-04-07-beyond-the-parameters-a-technical-survey-of-contex.md|2026 04 07 beyond the parameters a technical survey of contex.md]] (2026-04-07)
- [[sources/2026-04-07-bibtex-citation-hallucinations-in-scientific-publi.md|2026 04 07 bibtex citation hallucinations in scientific publi.md]] (2026-04-07)
- [[sources/2026-04-07-detecting-and-correcting-reference-hallucinations-.md|2026 04 07 detecting and correcting reference hallucinations .md]] (2026-04-07)
- [[sources/2026-04-07-prism-llm-guided-semantic-clustering-for-high-prec.md|2026 04 07 prism llm guided semantic clustering for high prec.md]] (2026-04-07)
- [[sources/2026-04-08-beyond-the-final-actor-modeling-the-dual-roles-of-.md|2026 04 08 beyond the final actor modeling the dual roles of .md]] (2026-04-08)
- [[sources/2026-04-08-triattention-efficient-long-reasoning-with-trigono.md|2026 04 08 triattention efficient long reasoning with trigono.md]] (2026-04-08)
- [[sources/2026-04-09-exclusive-unlearning.md|2026 04 09 exclusive unlearning.md]] (2026-04-09)
- [[sources/2026-04-09-in-place-test-time-training.md|2026 04 09 in place test time training.md]] (2026-04-09)
- [[sources/2026-04-09-toward-consistent-world-models-with-multi-token-pr.md|2026 04 09 toward consistent world models with multi token pr.md]] (2026-04-09)
- [[sources/2026-04-10-a-systematic-study-of-retrieval-pipeline-design-fo.md|2026 04 10 a systematic study of retrieval pipeline design fo.md]] (2026-04-10)
- [[sources/2026-04-10-chatbot-based-assessment-of-code-understanding-in-.md|2026 04 10 chatbot based assessment of code understanding in .md]] (2026-04-10)
- [[sources/2026-04-10-evaluating-in-context-translation-with-synchronous.md|2026 04 10 evaluating in context translation with synchronous.md]] (2026-04-10)
- [[sources/2026-04-10-syntax-is-easy-semantics-is-hard-evaluating-llms-f.md|2026 04 10 syntax is easy semantics is hard evaluating llms f.md]] (2026-04-10)
- [[sources/2026-04-11-ads-in-ai-chatbots-an-analysis-of-how-large-langua.md|2026 04 11 ads in ai chatbots an analysis of how large langua.md]] (2026-04-11)
- [[sources/2026-04-11-clawbench-can-ai-agents-complete-everyday-online-t.md|2026 04 11 clawbench can ai agents complete everyday online t.md]] (2026-04-11)
- [[sources/2026-04-11-cram-less-to-fit-more-training-data-pruning-improv.md|2026 04 11 cram less to fit more training data pruning improv.md]] (2026-04-11)
- [[sources/2026-04-11-figures-as-interfaces-toward-llm-native-artifacts-.md|2026 04 11 figures as interfaces toward llm native artifacts .md]] (2026-04-11)
- [[sources/2026-04-11-what-do-language-models-learn-and-when-the-implici.md|2026 04 11 what do language models learn and when the implici.md]] (2026-04-11)
- [[sources/2026-04-11-what-drives-representation-steering-a-mechanistic-.md|2026 04 11 what drives representation steering a mechanistic .md]] (2026-04-11)
- [[sources/2026-04-12-ads-in-ai-chatbots-an-analysis-of-how-large-langua.md|2026 04 12 ads in ai chatbots an analysis of how large langua.md]] (2026-04-12)
- [[sources/2026-04-12-cram-less-to-fit-more-training-data-pruning-improv.md|2026 04 12 cram less to fit more training data pruning improv.md]] (2026-04-12)
- [[sources/2026-04-12-demystifying-opd-length-inflation-and-stabilizatio.md|2026 04 12 demystifying opd length inflation and stabilizatio.md]] (2026-04-12)
- [[sources/2026-04-12-figures-as-interfaces-toward-llm-native-artifacts-.md|2026 04 12 figures as interfaces toward llm native artifacts .md]] (2026-04-12)
- [[sources/2026-04-12-what-do-language-models-learn-and-when-the-implici.md|2026 04 12 what do language models learn and when the implici.md]] (2026-04-12)
- [[sources/2026-04-13-ads-in-ai-chatbots-an-analysis-of-how-large-langua.md|2026 04 13 ads in ai chatbots an analysis of how large langua.md]] (2026-04-13)
- [[sources/2026-04-13-cram-less-to-fit-more-training-data-pruning-improv.md|2026 04 13 cram less to fit more training data pruning improv.md]] (2026-04-13)
- [[sources/2026-04-13-figures-as-interfaces-toward-llm-native-artifacts-.md|2026 04 13 figures as interfaces toward llm native artifacts .md]] (2026-04-13)
- [[sources/2026-04-13-what-drives-representation-steering-a-mechanistic-.md|2026 04 13 what drives representation steering a mechanistic .md]] (2026-04-13)
