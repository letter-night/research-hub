# Causality

**나의 관점:** 인과추론은 관측 데이터 이면의 **data generating mechanism**을 추론하는 일이다. 표면적인 확률·통계적 추론을 넘어서야 새로운 환경에 적용할 수 있다.

**연구 지향점 (2026-11):** LLM/Agent 기반 인과추론. 관심은 양방향이다.
- (→) Agent의 추론 능력으로 인과추론을 개선한다: DAG 탐색, sensitivity analysis, multimodality
- (←) Agent의 인과추론 능력을 보이거나(MI) 심는다: causal world model, plan evaluation

**공부 궤적:** conformal·robust agents (2025.6) → causal discovery·CRL (2025.7) → PFN (2025.10) → Bayesian structure learning·active learning (2025.12) → causal foundation models (2026.1) → time-varying treatment (2026.1–3) → 고전 정독: *What If*, *Causality* (2026.11)

## 열린 질문
- Agent / foundation model이 Bayesian structure learning을 한다면 data generating process를 규명할 수 있을까? 그 결과에 confidence를 함께 줄 수 있을까?
- time-fixed DAG/SCM 추론은 실제 인과효과의 얼마만큼을 보는가?
- PFN 계열 모델은 정말 내부에서 인과 그래프를 찾는가? (→ I02)
- 어떻게 causal model을 학습시킬 것인가?

## 관련 아이디어
- [I01 LLM 내부는 프롬프트의 인과 그래프를 충실하게 구현하는가 (SCM faithfulness)](../../ideas/I01-scm-faithfulness-in-llm-internals.md) — `draft`
- [I02 PFN 기반 인과 foundation model은 정말 내부에서 인과 그래프를 찾는가](../../ideas/I02-mi-on-causal-pfn.md) — `seed`
- [I03 In-context learning만으로 복잡한 DAG 구조를 추론할 수 있는가](../../ideas/I03-complex-dag-in-context-learning.md) — `seed`
- [I04 Multimodal time-varying causal effect estimation foundation model (Agent)](../../ideas/I04-multimodal-time-varying-causal-fm.md) — `parked`
- [I05 Agent가 돕는 인과추론: DAG 탐색과 sensitivity analysis](../../ideas/I05-agent-assisted-causal-inference.md) — `seed`
- [I06 Plan evaluation: 순차 action의 인과효과를 추정하는 agent](../../ideas/I06-plan-evaluation-for-causal-agents.md) — `seed`
- [I08 Schrödinger Bridge × Causality: treatment에 따른 trajectory 모델링](../../ideas/I08-treatment-conditioned-trajectory-sb.md) — `seed`

<!-- auto:start -->
## 논문 계보 (발표 연도순)
✅ 읽음 · 📖 읽는 중 · 📌 읽을 예정

### 시계열 처치효과 (time-varying treatment)
| 연도 | 논문 | 상태 |
|---|---|---|
| 2018 | [Forecasting Treatment Responses Over Time Using Recurrent Marginal Structural Networks (RMSNs)](papers/2018-rmsn.md) | ✅ |
| 2020 | [Estimating Counterfactual Treatment Outcomes over Time through Adversarially Balanced Representations (CRN)](papers/2020-crn.md) | ✅ |
| 2021 | [G-Net: A Recurrent Network Approach to G-Computation for Counterfactual Prediction Under a Dynamic Treatment Regime](papers/2021-g-net.md) | ✅ |
| 2022 | [Causal Transformer for Estimating Counterfactual Outcomes (CT)](papers/2022-causal-transformer.md) | ✅ |
| 2022 | [Continuous-Time Modeling of Counterfactual Outcomes Using Neural Controlled Differential Equations (TE-CDE)](papers/2022-te-cde.md) | ✅ |
| 2024 | [Bayesian Neural Controlled Differential Equations for Treatment Effect Estimation (BNCDE)](papers/2024-bncde.md) | ✅ |
| 2024 | [G-Transformer: Counterfactual Outcome Prediction under Dynamic and Time-varying Treatment Regimes](papers/2024-g-transformer.md) | ✅ |
| 2025 | [Stabilized Neural Prediction of Potential Outcomes in Continuous Time (SCIP-Net)](papers/2025-scip-net.md) | ✅ |
| ? | [IGC-Net: CAPO Estimation over Time](papers/igc-net.md) | ✅ |
### PFN · 인과 foundation model
| 연도 | 논문 | 상태 |
|---|---|---|
| 2023 | [TabPFN: A Transformer That Solves Small Tabular Classification Problems in a Second](papers/2023-tabpfn.md) | ✅ |
| 2025 | [Accurate predictions on small data with a tabular foundation model (TabPFN v2)](papers/2025-tabpfn-v2.md) | ✅ |
| 2025 | [CausalPFN: Amortized Causal Effect Estimation via In-Context Learning](papers/2025-causalpfn.md) | ✅ |
| 2025 | [Do-PFN: In-Context Learning for Causal Effect Estimation](papers/2025-do-pfn.md) | ✅ |
| 2025 | [Foundation Models for Causal Inference via Prior-Data Fitted Networks (CausalFM)](papers/2025-causalfm.md) | ✅ |
| 2025 | [TimePFN: Effective Multivariate Time Series Forecasting with Synthetic Data](papers/2025-timepfn.md) | ✅ |
### 구조 학습 · 실험 설계 · 능동 학습
| 연도 | 논문 | 상태 |
|---|---|---|
| 2011 | [Bayesian Active Learning for Classification and Preference Learning (BALD)](papers/2011-bald.md) | ✅ |
| 2019 | [BatchBALD: Efficient and Diverse Batch Acquisition for Deep Bayesian Active Learning](papers/2019-batchbald.md) | ✅ |
| 2019 | [Review of Causal Discovery Methods Based on Graphical Models](papers/2019-causal-discovery-graphical-models.md) | ✅ |
| 2020 | [A Meta-Transfer Objective for Learning to Disentangle Causal Mechanisms](papers/2020-meta-transfer-objective.md) | ✅ |
| 2021 | [DiBS: Differentiable Bayesian Structure Learning](papers/2021-dibs.md) | ✅ |
| 2022 | [Bayesian Structure Learning with Generative Flow Networks (DAG-GFlowNet)](papers/2022-dag-gflownet.md) | ✅ |
| 2022 | [Interventions, Where and How? Experimental Design for Causal Models at Scale](papers/2022-cbed-interventions-where-and-how.md) | ✅ |
| 2023 | [Stochastic Batch Acquisition: A Simple Baseline for Deep Active Learning](papers/2023-stochastic-bald.md) | ✅ |
| 2023 | [iSCAN: Identifying Causal Mechanism Shifts among Nonlinear Additive Noise Models](papers/2023-iscan.md) | ✅ |
### 인과 표현 · 생성모델
| 연도 | 논문 | 상태 |
|---|---|---|
| 2023 | [Causal normalizing flows: from theory to practice](papers/2023-causal-normalizing-flows.md) | ✅ |
| ? | [Causal Representation Learning (2부작 정리)](papers/causal-representation-learning.md) | ✅ |
### Agent · LLM과 인과
| 연도 | 논문 | 상태 |
|---|---|---|
| 2024 | [Automating psychological hypothesis generation with AI: when large language models meet causal graph](papers/2024-llm-causal-graph-psych-hypothesis.md) | ✅ |
| 2024 | [Robust Agents Learn Causal World Models](papers/2024-robust-agents-causal-world-models.md) | ✅ |
### 불확실성
| 연도 | 논문 | 상태 |
|---|---|---|
| 2021 | [A Gentle Introduction to Conformal Prediction and Distribution-Free Uncertainty Quantification](papers/2021-conformal-prediction-gentle-intro.md) | ✅ |
| 2024 | [Large language model validity via enhanced conformal prediction methods](papers/2024-llm-validity-enhanced-conformal.md) | ✅ |

## 나의 생각 (최신순)
- [RL Agent와의 차이점](thoughts/2026-11-22-rl-agent-vs-causal-agent.md) — 2026-11-22
- [Causality (Judea Pearl) & What If (Hernán & Robins) 완독 회고](thoughts/2026-11-20-reading-pearl-and-what-if.md) — 2026-11-20
- [Time-varying treatment를 plan evaluation 문제로 보기](thoughts/2026-11-18-time-varying-treatment-as-plan-evaluation.md) — 2026-11-18
- [고전의 중요성 2탄](thoughts/2026-11-11-importance-of-classics-2.md) — 2026-11-11
- [여전한 믿음: 시계열 인과추론 foundation model](thoughts/2026-11-10-unchanged-belief-longitudinal-causal-fm.md) — 2026-11-10
- [고전의 중요성: LLM/Agent 기반 인과추론이라는 지향점](thoughts/2026-11-09-importance-of-classics.md) — 2026-11-09
- [causal inference를 공부하며 3탄: 참고서 비교와 LLM/Agent의 역할](thoughts/2026-11-08-studying-causal-inference-3.md) — 2026-11-08
- [[부치지 못한 편지 2] Causal effect under time-varying treatment](thoughts/2026-11-05-causal-effect-under-time-varying-treatment.md) — 2026-11-05
- [인과의 시작과 끝을 아는 이: 현상 이면의 mechanism](thoughts/2026-04-18-knowing-the-mechanism-behind-phenomena.md) — 2026-04-18
- [정말로 implicit하게 causal graph를 찾고 추론했을까?](thoughts/2026-01-14-did-pfn-find-causal-graph-implicitly.md) — 2026-01-14
- [복잡한 DAG 구조로 in-context learning을 하면?](thoughts/2026-01-06-complex-dag-in-context-learning.md) — 2026-01-06
- [여전히 풀리지 않은 숙제](thoughts/2025-12-22-still-unsolved-homework.md) — 2025-12-22
- [On-going thought: robust agent는 causal model을 알아야 한다](thoughts/2025-06-21-robust-agents-need-causal-models.md) — 2025-06-21

## 교재
- [Causality: Models, Reasoning, and Inference](books/pearl-causality.md)
- [Causal Inference: What If](books/hernan-robins-what-if.md)

## 강의
- [Introduction to Causal Inference (course & lecture notes)](lectures/brady-neal-causal-inference-course.md)
- [A First Course in Causal Inference (STA9083 lecture notes)](lectures/peng-ding-first-course-causal-inference.md)
- [Causal Inference for the Brave and True](lectures/causal-inference-brave-and-true.md)

## 영상
- (없음)

## 외부 글
- [Introducing TabFM: A zero-shot foundation model for tabular data](posts/google-tabfm.md)

## 개념 정리
- (없음)

## 다른 주제에서 온 관련 노트
- [그렇다면 Agent는 정말로 human보다 intelligent한가?](../../topics/agentic-ai/thoughts/2026-11-22-is-agent-more-intelligent-than-human.md) (agentic-ai)
- [그냥 문득 든 생각들: SB×causality, 그리고 AI의 '일머리'](../../topics/agentic-ai/thoughts/2026-11-14-random-thoughts-ontology-and-work-knowledge.md) (agentic-ai)
- [Why Agents Need Causal World Models](../../topics/agentic-ai/thoughts/2026-10-11-why-agents-need-causal-world-models.md) (agentic-ai)
- [Mechanistic Interpretability가 Causal Representation & Discovery에 답을 주었다](../../topics/mech-interp/thoughts/2026-01-09-mi-answers-causal-representation.md) (mech-interp)
- [그렇다면 MI는 LLM이 causal reasoning을 할 수 있다는 증거 아닌가?](../../topics/mech-interp/thoughts/2026-01-12-is-mi-evidence-of-causal-reasoning.md) (mech-interp)
- [생성모델 관점에서 생각해보더라도](../../topics/mech-interp/thoughts/2026-06-15-generative-model-view-of-mi.md) (mech-interp)
- [Training Large Language Models to Reason in a Continuous Latent Space (COCONUT)](../../topics/agentic-ai/papers/2024-coconut.md) (agentic-ai)
- [Causal Abstractions of Neural Networks](../../topics/mech-interp/papers/2021-causal-abstractions-of-neural-networks.md) (mech-interp)
- [Finding Alignments Between Interpretable Causal Variables and Distributed Neural Representations (DAS)](../../topics/mech-interp/papers/2023-das-finding-alignments.md) (mech-interp)
- [Mechanistic Interpretability Through the Lens of Causal Mediation Analysis (Right Mediator)](../../topics/mech-interp/papers/2024-mi-through-causal-mediation.md) (mech-interp)

*마지막 갱신: 2026-11-23*
<!-- auto:end -->
