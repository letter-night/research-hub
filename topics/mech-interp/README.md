# Mechanistic Interpretability

**나의 관점:** MI는 단순히 "모델 내부를 해석하는 것"이 아니다. feature를 disentangle하고(causal representation), feature 간 인과 관계를 찾고(causal discovery), 개입 효과를 구한다(causal inference). 그래서 MI는 **LLM이 data generating process를 이해하는지 검증할 수 있는 도구**다.

**가설:** LLM은 내부에 계층적인 causal concept를 저장하고, feature 간 causal graph(circuit)를 거쳐 추론한다. "확률적 앵무새"라는 관점은 낡았다.

**궁극적 질문:** 모델은 **어떤 추론 과정을 거쳐서** 답을 내놓았는가? → attribution graph가 현재 최선의 도구. 단, intervention으로 검증해야 한다.

**필수 읽기 경로 (2026-06 "(Review) Mechanistic Interpretability"에서)**
1. Zoom In: An Introduction to Circuits — https://distill.pub/2020/circuits/zoom-in/
2. A Mathematical Framework for Transformer Circuits
3. MI Through the Lens of Causal Mediation Analysis
4. A Primer on the Inner Workings of Transformer-based LMs
5. Open Problems in Mechanistic Interpretability — https://arxiv.org/abs/2501.16496

입문은 Anthropic 홈페이지 글, 자세한 내용은 Transformer Circuits Thread (인내심 필요).

## 열린 질문
- LLM 내부는 프롬프트에 기술된 인과 그래프를 충실하게 구현하는가? (→ I01)
- feature labeling은 어떻게 하는가? 프롬프트만 주고 attribution graph를 해석할 수 있는가?
- J-space로 암기와 추론을 구분할 수 있는가? (→ I11)
- post-training에서 형성되는 '자아'와 persona·meta-cognition의 관계는?

## 관련 아이디어
- [I01 LLM 내부는 프롬프트의 인과 그래프를 충실하게 구현하는가 (SCM faithfulness)](../../ideas/I01-scm-faithfulness-in-llm-internals.md) — `draft`
- [I02 PFN 기반 인과 foundation model은 정말 내부에서 인과 그래프를 찾는가](../../ideas/I02-mi-on-causal-pfn.md) — `seed`
- [I03 In-context learning만으로 복잡한 DAG 구조를 추론할 수 있는가](../../ideas/I03-complex-dag-in-context-learning.md) — `seed`
- [I09 Persona simulation의 내부 기전: 어떤 입력이 high-fidelity를 만드는가](../../ideas/I09-persona-simulation-mechanism.md) — `seed`
- [I11 J-space로 '암기한 답'과 '추론한 답'을 구분할 수 있는가](../../ideas/I11-j-space-memorization-vs-reasoning.md) — `seed`

<!-- auto:start -->
## 논문 계보 (발표 연도순)
✅ 읽음 · 📖 읽는 중 · 📌 읽을 예정

### 기초: circuits · superposition
| 연도 | 논문 | 상태 |
|---|---|---|
| 2021 | [A Mathematical Framework for Transformer Circuits](papers/2021-mathematical-framework-transformer-circuits.md) | ✅ |
| 2022 | [Interpretability in the Wild: A Circuit for Indirect Object Identification in GPT-2 Small](papers/2022-ioi-circuit-gpt2-small.md) | ✅ |
| 2022 | [Toy Models of Superposition](papers/2022-toy-models-of-superposition.md) | ✅ |
| 2024 | [Transcoders Find Interpretable LLM Feature Circuits](papers/2024-transcoders.md) | ✅ |
### Dictionary learning → attribution graph
| 연도 | 논문 | 상태 |
|---|---|---|
| 2023 | [Towards Monosemanticity: Decomposing Language Models With Dictionary Learning](papers/2023-towards-monosemanticity.md) | ✅ |
| 2024 | [Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet](papers/2024-scaling-monosemanticity.md) | ✅ |
| 2024 | [Sparse Crosscoders for Cross-Layer Features and Model Diffing](papers/2024-crosscoders.md) | ✅ |
| 2025 | [Circuit Tracing: Revealing Computational Graphs in Language Models](papers/2025-circuit-tracing.md) | ✅ |
| 2025 | [On the Biology of a Large Language Model](papers/2025-biology-of-a-large-language-model.md) | ✅ |
| 2025 | [Tracing Attention Computation Through Feature Interactions](papers/2025-tracing-attention-computation.md) | ✅ |
### 인과적 방법론 (patching · causal abstraction · mediation)
| 연도 | 논문 | 상태 |
|---|---|---|
| 2021 | [Causal Abstractions of Neural Networks](papers/2021-causal-abstractions-of-neural-networks.md) | ✅ |
| 2023 | [Finding Alignments Between Interpretable Causal Variables and Distributed Neural Representations (DAS)](papers/2023-das-finding-alignments.md) | ✅ |
| 2023 | [The Hydra Effect: Emergent Self-repair in Language Model Computations](papers/2023-hydra-effect.md) | ✅ |
| 2024 | [How to use and interpret activation patching](papers/2024-activation-patching-how-to.md) | ✅ |
| 2024 | [Mechanistic Interpretability Through the Lens of Causal Mediation Analysis (Right Mediator)](papers/2024-mi-through-causal-mediation.md) | ✅ |
### 표현 기하 · workspace · NLA
| 연도 | 논문 | 상태 |
|---|---|---|
| 2024 | [The Geometry of Categorical and Hierarchical Concepts in Large Language Models](papers/2024-geometry-categorical-hierarchical-concepts.md) | 📖 |
| 2026 | [Natural Language Autoencoders Produce Unsupervised Explanations of LLM Activations](papers/2026-natural-language-autoencoders.md) | ✅ |
| 2026 | [Verbalizable Representations Form a Global Workspace in Language Models](papers/2026-global-workspace-in-language-models.md) | 📖 |
### Survey · methods
| 연도 | 논문 | 상태 |
|---|---|---|
| 2024 | [A Primer on the Inner Workings of Transformer-based Language Models](papers/2024-primer-inner-workings-transformer-lms.md) | ✅ |

## 나의 생각 (최신순)
- [그간의 생각 정리, 근데 너무 어려움 (연구 과정)](thoughts/2026-07-26-research-process-proposal-is-hard.md) — 2026-07-26
- [human이랑 다를 게 뭔가?](thoughts/2026-07-24-how-different-from-humans.md) — 2026-07-24
- [J-lens와 attribution graph 비교](thoughts/2026-07-20-j-lens-vs-attribution-graph.md) — 2026-07-20
- [Pygmalion Effect: LLM의 identity 형성](thoughts/2026-07-20-pygmalion-effect-llm-identity.md) — 2026-07-20
- [Thought on Mechanistic Interpretability (CLT, NLA, J-space)](thoughts/2026-07-19-thought-on-mechanistic-interpretability.md) — 2026-07-19
- [궁금증 해결 방법 찾음: 의료 진단 추론과 해석가능성](thoughts/2026-07-18-mi-for-medical-diagnosis-reliability.md) — 2026-07-18
- [LLM은 거대한 graph database retrieval system 같다](thoughts/2026-06-15-llm-as-graph-database-retrieval.md) — 2026-06-15
- [생성모델 관점에서 생각해보더라도](thoughts/2026-06-15-generative-model-view-of-mi.md) — 2026-06-15
- [그렇다면 MI는 LLM이 causal reasoning을 할 수 있다는 증거 아닌가?](thoughts/2026-01-12-is-mi-evidence-of-causal-reasoning.md) — 2026-01-12
- [Mechanistic Interpretability가 Causal Representation & Discovery에 답을 주었다](thoughts/2026-01-09-mi-answers-causal-representation.md) — 2026-01-09

## 교재
- (없음)

## 강의
- (없음)

## 영상
- (없음)

## 외부 글
- (없음)

## 개념 정리
- [Circuits](concepts/circuits.md)
- [Transformer Circuits](concepts/transformer-circuits.md)
- [Why induction heads matter for meta-learning](concepts/induction-heads-and-meta-learning.md)
- [Superposition](concepts/superposition.md)
- [Activation Patching](concepts/activation-patching.md)
- [Causal Abstraction](concepts/causal-abstraction.md)
- [Features](concepts/features.md)
- [(Gentle Intro) how LLMs really work](concepts/gentle-intro-how-llms-work.md)
- [Circuit tracing tools: what's going on inside LMs?](concepts/circuit-tracing-tools.md)

## 다른 주제에서 온 관련 노트
- [고전의 중요성: LLM/Agent 기반 인과추론이라는 지향점](../../topics/causality/thoughts/2026-11-09-importance-of-classics.md) (causality)
- [인과의 시작과 끝을 아는 이: 현상 이면의 mechanism](../../topics/causality/thoughts/2026-04-18-knowing-the-mechanism-behind-phenomena.md) (causality)
- [정말로 implicit하게 causal graph를 찾고 추론했을까?](../../topics/causality/thoughts/2026-01-14-did-pfn-find-causal-graph-implicitly.md) (causality)
- [그렇다면 Agent는 정말로 human보다 intelligent한가?](../../topics/agentic-ai/thoughts/2026-11-22-is-agent-more-intelligent-than-human.md) (agentic-ai)
- [Virtual Society: persona simulation의 기전이 궁금하다](../../topics/agentic-ai/thoughts/2026-07-12-virtual-society-persona-simulation.md) (agentic-ai)
- [thought 1: persona agent는 왜 사람처럼 결정하는가](../../topics/agentic-ai/thoughts/2026-07-14-persona-agents-thought-1.md) (agentic-ai)
- [thought 3: 어떤 stimulus가 이런 결과를 만들었나](../../topics/agentic-ai/thoughts/2026-07-15-persona-agents-thought-3-which-stimulus.md) (agentic-ai)
- [Automating psychological hypothesis generation with AI: when large language models meet causal graph](../../topics/causality/papers/2024-llm-causal-graph-psych-hypothesis.md) (causality)

*마지막 갱신: 2026-11-23*
<!-- auto:end -->
