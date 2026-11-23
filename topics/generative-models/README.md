# Generative Models

**나의 관점:** 생성 모델링은 모델 분포의 확률 질량을 데이터 분포로 **어떻게 옮길 것인가**의 문제다. DM과 FM은 모두 OT/EOT(Schrödinger Bridge)를 풀고 싶었지만 현실적인 타협점을 찾은 것이다 ("꿩 대신 닭").

**통일된 그림**
- SB의 해는 forward/backward potential로 떨어진다 → 한쪽을 고정한 half-bridge = DM, 독립 coupling의 선형 보간 = FM
- controllability(steering)는 결국 score 문제: $\nabla_x \log \phi(x)$
- SB와 DPG(controlled text generation)는 같은 형태: $\min_{p\in\mathcal{C}} D(p\,\|\,p_{\text{ref}})$ — Maximum Entropy Principle의 일반화

**응용 관심:** single-cell trajectory (unbalanced OT, RUOT), diffusion language models, inverse problems. 그리고 treatment에 따른 trajectory (→ Causality와 연결)

## 열린 질문
- 어떤 training algorithm이 optimal flow가 되는가? (→ I07)
- 고차원 state에서 SB 학습 비용을 어떻게 줄이는가? (latent space 시뮬레이션)
- SB에 인과적 개입을 결합할 수 있는가? (→ I08)
- Lipschitz condition, error analysis (수치해석 복습 필요)

## 관련 아이디어
- [I07 학습 과정을 optimal flow로: 효율적인 generative model 학습](../../ideas/I07-training-as-optimal-flow.md) — `seed`
- [I08 Schrödinger Bridge × Causality: treatment에 따른 trajectory 모델링](../../ideas/I08-treatment-conditioned-trajectory-sb.md) — `seed`

<!-- auto:start -->
## 논문 계보 (발표 연도순)
✅ 읽음 · 📖 읽는 중 · 📌 읽을 예정

### Diffusion LM
| 연도 | 논문 | 상태 |
|---|---|---|
| 2022 | [Diffusion-LM Improves Controllable Text Generation](papers/2022-diffusion-lm.md) | ✅ |
| 2023 | [Likelihood-Based Diffusion Language Models](papers/2023-likelihood-based-diffusion-lms.md) | ✅ |
| 2024 | [Simple Guidance Mechanisms for Discrete Diffusion Models (D-CFG)](papers/2024-discrete-diffusion-guidance.md) | ✅ |
| 2024 | [Simple and Effective Masked Diffusion Language Models (MDLM)](papers/2024-mdlm.md) | ✅ |
| 2025 | [LLaDA 1.5: Variance-Reduced Preference Optimization for Large Language Diffusion Models](papers/2025-llada-1-5-vrpo.md) | ✅ |
| 2025 | [Large Language Diffusion Models (LLaDA)](papers/2025-llada.md) | ✅ |
| 2025 | [d1: Scaling Reasoning in Diffusion Large Language Models via Reinforcement Learning](papers/2025-d1-reasoning-dllm-rl.md) | ✅ |
| ? | [Continuous diffusion language models](papers/continuous-diffusion-language-models.md) | ✅ |
| ? | [Diffusion Language Models (정리)](papers/diffusion-language-models-overview.md) | 📖 |
### Controlled generation · distribution matching
| 연도 | 논문 | 상태 |
|---|---|---|
| 2021 | [A Distributional Approach to Controlled Text Generation (KL-Adaptive DPG)](papers/2021-distributional-approach-controlled-generation.md) | ✅ |
| 2022 | [Controlling Conditional Language Models without Catastrophic Forgetting (CDPG)](papers/2022-cdpg.md) | ✅ |
| 2022 | [On Reinforcement Learning and Distribution Matching for Fine-Tuning Language Models with no Catastrophic Forgetting](papers/2022-rl-vs-distribution-matching-finetuning.md) | ✅ |
### Schrödinger Bridge · OT · single-cell
| 연도 | 논문 | 상태 |
|---|---|---|
| 2022 | [Deep Generalized Schrödinger Bridge](papers/2022-deep-generalized-sb.md) | ✅ |
| 2024 | [Reconstructing growth and dynamic trajectories from single-cell transcriptomics data](papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) | ✅ |
| 2025 | [Foundations of Schrödinger Bridges for Generative Modeling](papers/2025-foundations-of-sb-generative-modeling.md) | 📖 |
| 2025 | [Learning Stochastic Dynamics from Snapshots through Regularized Unbalanced Optimal Transport](papers/2025-ruot-stochastic-dynamics-snapshots.md) | ✅ |
### Diffusion · Flow 기초와 응용
| 연도 | 논문 | 상태 |
|---|---|---|
| 2022 | [Improving Diffusion Models for Inverse Problems using Manifold Constraints (MCG)](papers/2022-mcg-manifold-constraints.md) | 📌 |
| 2023 | [Diffusion Posterior Sampling for General Noisy Inverse Problems (DPS)](papers/2023-diffusion-posterior-sampling.md) | 📌 |
| 2025 | [The Principles of Diffusion Models](papers/2025-principles-of-diffusion-models.md) | 📖 |
| ? | [Flow Map Models](papers/flow-map-models.md) | ✅ |
| ? | [Flow Matching & Diffusion Models (강의노트 정리)](papers/flow-matching-and-diffusion-models-notes.md) | 📖 |

## 나의 생각 (최신순)
- [[소소한 의문들] Lipschitz condition과 error analysis](thoughts/2026-10-07-small-questions-lipschitz-error-analysis.md) — 2026-10-07
- [DM/FM/SB를 공부하며: controllability는 결국 score 문제](thoughts/2026-09-12-steering-as-score-dm-fm-sb.md) — 2026-09-12
- [알아가는 즐거움](thoughts/2026-08-28-joy-of-learning.md) — 2026-08-28
- [아쉬움, 미련: Generalized SB를 공부하며](thoughts/2026-08-25-sb-study-reflection.md) — 2026-08-25
- [SB를 알아가고 있다](thoughts/2026-08-19-getting-to-know-sb.md) — 2026-08-19
- [SB framework 안에서 DM와 FM의 탄생 비화](thoughts/2026-08-18-birth-of-dm-and-fm-within-sb.md) — 2026-08-18
- [흥미로운 공통점: SB와 DPG는 같은 형태 (Distribution Matching)](thoughts/2026-08-17-sb-and-dpg-same-form.md) — 2026-08-17
- [generative model의 training efficiency: 학습을 optimal flow로 볼 수 있을까 (thought 1, 2)](thoughts/2026-08-15-training-efficiency-as-optimal-flow.md) — 2026-08-15

## 교재
- (없음)

## 강의
- (없음)

## 영상
- (없음)

## 외부 글
- (없음)

## 개념 정리
- [Derivation of continuity eqn & Fokker-Planck eqn](concepts/continuity-and-fokker-planck.md)
- [Push-forward](concepts/push-forward.md)
- [Understanding Girsanov's theorem intuitively](concepts/girsanov-theorem.md)
- [Schrödinger Bridge solution as two space-time potentials](concepts/sb-two-space-time-potentials.md)
- [Feynman–Kac formula](concepts/feynman-kac-formula.md)
- [SB와 score-based diffusion model의 차이](concepts/sb-vs-score-based-diffusion.md)
- [Doob's h-transform](concepts/doobs-h-transform.md)
- [SB Cheat Sheet (#1–#3, Figures)](concepts/sb-cheat-sheet.md)
- [Waddington landscape](concepts/waddington-landscape.md)
- [논문을 읽기 위해 필요한 사전지식 (cell trajectory)](concepts/background-for-cell-trajectory-papers.md)
- [Wasserstein gradient flow](concepts/wasserstein-gradient-flow.md)
- [DM Cheat Sheet](concepts/dm-cheat-sheet.md)
- [Useful mental picture for Flow Map Models (TD learning)](concepts/flow-map-mental-picture.md)
- [ELBO approximation (diffusion LM)](concepts/elbo-approximation-diffusion-lm.md)

## 다른 주제에서 온 관련 노트
- [그냥 문득 든 생각들: SB×causality, 그리고 AI의 '일머리'](../../topics/agentic-ai/thoughts/2026-11-14-random-thoughts-ontology-and-work-knowledge.md) (agentic-ai)
- [생성모델 관점에서 생각해보더라도](../../topics/mech-interp/thoughts/2026-06-15-generative-model-view-of-mi.md) (mech-interp)
- [Causal normalizing flows: from theory to practice](../../topics/causality/papers/2023-causal-normalizing-flows.md) (causality)

*마지막 갱신: 2026-11-23*
<!-- auto:end -->
