# Tistory 이전 기록 (1차)

- 원본: https://letter-night.tistory.com/
- 범위: Generative Models_2 (41), AgenticAI (13), LLMs (86), Causality (48) — 총 188편
- 이전일: 2026-11-23
- 원칙: 개인적인 생각, 연구 과정, 논문 리뷰는 옮기고, 논문을 그대로 붙여넣은 글은 본문을 옮기지 않음

## 처리 방식
- **요약 이전**: 생각 글의 핵심을 원문 표현을 살려 옮김 (`migration: summary`)
- **논문 노트 (스텁)**: 메타데이터와 원문 링크만. 원문에 본인 리뷰가 있으면 "나의 리뷰"로 옮겨야 함 (`migration: stub`)
- **리뷰 병합**: 논문에 대한 생각 글을 해당 논문 노트의 "나의 리뷰"로 합침
- **개념 노트 (스텁)**: 수식·그림 위주 글. 링크만 옮김

## 처리 결과 요약 (글 기준 첫 번째 처리)
| 처리 | 글 수 |
|---|---|
| 논문 노트 | 88 |
| 요약 이전 | 40 |
| 개념 노트 | 32 |
| 강의 노트 | 6 |
| 리뷰 병합 | 4 |
| 프로젝트 기록 | 4 |
| 보류/이전 실패 | 2 |
| 스텁 | 2 |
| 영상 노트 | 2 |
| 목록 병합 | 2 |
| 아이디어로 이전 | 2 |
| 외부 글 노트 | 2 |
| 링크만 | 1 |
| 읽기 메모 병합 | 1 |

## 남은 일
- [ ] 논문 노트 스텁: 원문에 본인 리뷰가 있는지 확인하고 채우기 (특히 time-varying treatment 계열 9편, PFN 계열)
- [ ] 이미지 위주 글 텍스트화: Research Proposal(1331), 논문 정주행 bucket list(1492), time-varying confounders 도식(1517)
- [ ] 개념 노트: 다시 볼 때 LaTeX로 정리 (SB cheat sheet, Girsanov, Feynman-Kac, Doob's h-transform)
- [ ] 다른 카테고리 이전: Mathematics, NeuralDiffEqn, STA9132, Paper Writing, RL, NLP, Multimodal
- [ ] 2025-03-19, 2025-05-03 글 (On-going thought에서 언급) 찾기

## Generative Models_2 (41)
| 작성일 | 원문 | 원 카테고리 | 새 위치 · 처리 |
|---|---|---|---|
| 2026-10-12 | [useful mental picture for Flow Map Models](https://letter-night.tistory.com/1500) | Generative Models_2 | [flow-map-mental-picture.md](../topics/generative-models/concepts/flow-map-mental-picture.md) · 개념 노트 (스텁) |
| 2026-10-11 | [DM Cheat Sheet](https://letter-night.tistory.com/1498) | Generative Models_2 | [dm-cheat-sheet.md](../topics/generative-models/concepts/dm-cheat-sheet.md) · 개념 노트 (스텁) |
| 2026-10-07 | [[소소한 의문들]](https://letter-night.tistory.com/1496) | Generative Models_2 | [2026-10-07-small-questions-lipschitz-error-analysis.md](../topics/generative-models/thoughts/2026-10-07-small-questions-lipschitz-error-analysis.md) · 요약 이전 |
| 2026-09-29 | [Impressive works!](https://letter-night.tistory.com/1494) | Generative Models_2 | [2022-mcg-manifold-constraints.md](../topics/generative-models/papers/2022-mcg-manifold-constraints.md) · 논문 노트 (스텁)<br>[2023-diffusion-posterior-sampling.md](../topics/generative-models/papers/2023-diffusion-posterior-sampling.md) · 논문 노트 (스텁) |
| 2026-09-27 | [논문 정주행 bucket list](https://letter-night.tistory.com/1492) | Generative Models_2 | 이전 실패 — 논문 목록이 텍스트로 읽히지 않음 (표·이미지 추정). 수동 확인 필요 |
| 2026-09-23 | [Flow Map Models](https://letter-night.tistory.com/1490) | Generative Models_2 | [flow-map-models.md](../topics/generative-models/papers/flow-map-models.md) · 논문 노트 (스텁) |
| 2026-09-13 | [Wasserstein gradient flow](https://letter-night.tistory.com/1485) | Generative Models_2 | [wasserstein-gradient-flow.md](../topics/generative-models/concepts/wasserstein-gradient-flow.md) · 개념 노트 (스텁) |
| 2026-09-12 | [[잡담] DM/FM/SB를 공부하며](https://letter-night.tistory.com/1484) | Generative Models_2 | [2026-09-12-steering-as-score-dm-fm-sb.md](../topics/generative-models/thoughts/2026-09-12-steering-as-score-dm-fm-sb.md) · 요약 이전 |
| 2026-08-31 | [(5/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](https://letter-night.tistory.com/1476) | Generative Models_2 | [2024-reconstructing-growth-dynamic-trajectories-scrna.md](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) · 논문 노트 (스텁) |
| 2026-08-30 | [(4/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](https://letter-night.tistory.com/1474) | Generative Models_2 | [2024-reconstructing-growth-dynamic-trajectories-scrna.md](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) · 논문 노트 (스텁) |
| 2026-08-30 | [(3/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](https://letter-night.tistory.com/1473) | Generative Models_2 | [2024-reconstructing-growth-dynamic-trajectories-scrna.md](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) · 논문 노트 (스텁) |
| 2026-08-30 | [(2/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](https://letter-night.tistory.com/1472) | Generative Models_2 | [2024-reconstructing-growth-dynamic-trajectories-scrna.md](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) · 논문 노트 (스텁) |
| 2026-08-30 | [(1/5) Reconstructing Growth and Dynamic Trajectories from Single-Cell Transcriptomics Data](https://letter-night.tistory.com/1470) | Generative Models_2 | [2024-reconstructing-growth-dynamic-trajectories-scrna.md](../topics/generative-models/papers/2024-reconstructing-growth-dynamic-trajectories-scrna.md) · 논문 노트 (스텁) |
| 2026-08-29 | [Learning Stochastic Dynamics from Snapshots through Regularized Unbalanced OT](https://letter-night.tistory.com/1469) | Generative Models_2 | [2025-ruot-stochastic-dynamics-snapshots.md](../topics/generative-models/papers/2025-ruot-stochastic-dynamics-snapshots.md) · 논문 노트 |
| 2026-08-29 | [SB Cheat Sheet # 3 (section 5)](https://letter-night.tistory.com/1468) | Generative Models_2 | [sb-cheat-sheet.md](../topics/generative-models/concepts/sb-cheat-sheet.md) · 개념 노트 (스텁) |
| 2026-08-28 | [알아가는 즐거움](https://letter-night.tistory.com/1467) | Generative Models_2 | [2026-08-28-joy-of-learning.md](../topics/generative-models/thoughts/2026-08-28-joy-of-learning.md) · 스텁 |
| 2026-08-26 | [[background information] 논문을 읽기 위해 필요한 사전지식](https://letter-night.tistory.com/1466) | Generative Models_2 | [background-for-cell-trajectory-papers.md](../topics/generative-models/concepts/background-for-cell-trajectory-papers.md) · 개념 노트 (스텁) |
| 2026-08-26 | [[thought] Deep RUOT를 보고 든 생각](https://letter-night.tistory.com/1465) | Generative Models_2 | [2025-ruot-stochastic-dynamics-snapshots.md](../topics/generative-models/papers/2025-ruot-stochastic-dynamics-snapshots.md) · 리뷰 병합 |
| 2026-08-26 | [Waddington landscape](https://letter-night.tistory.com/1464) | Generative Models_2 | [waddington-landscape.md](../topics/generative-models/concepts/waddington-landscape.md) · 개념 노트 (스텁) |
| 2026-08-26 | [Learning Stochastic Dynamics from Snap-shots through Regularized Unbalanced OT](https://letter-night.tistory.com/1463) | Generative Models_2 | [2025-ruot-stochastic-dynamics-snapshots.md](../topics/generative-models/papers/2025-ruot-stochastic-dynamics-snapshots.md) · 논문 노트 |
| 2026-08-25 | [아쉬움, 미련..](https://letter-night.tistory.com/1462) | Generative Models_2 | [2026-08-25-sb-study-reflection.md](../topics/generative-models/thoughts/2026-08-25-sb-study-reflection.md) · 요약 이전 |
| 2026-08-25 | [Deep Generalized SB](https://letter-night.tistory.com/1461) | Generative Models_2 | [2022-deep-generalized-sb.md](../topics/generative-models/papers/2022-deep-generalized-sb.md) · 논문 노트 (스텁) |
| 2026-08-22 | [SB Cheat Sheet # 2 (section 4, 6, 8, 9)](https://letter-night.tistory.com/1458) | Generative Models_2 | [sb-cheat-sheet.md](../topics/generative-models/concepts/sb-cheat-sheet.md) · 개념 노트 (스텁) |
| 2026-08-22 | [SB Cheat Sheet - Figures](https://letter-night.tistory.com/1457) | Generative Models_2 | [sb-cheat-sheet.md](../topics/generative-models/concepts/sb-cheat-sheet.md) · 개념 노트 (스텁) |
| 2026-08-22 | [SB Cheat Sheet # 1 (section 1, 2, 3)](https://letter-night.tistory.com/1456) | Generative Models_2 | [sb-cheat-sheet.md](../topics/generative-models/concepts/sb-cheat-sheet.md) · 개념 노트 (스텁) |
| 2026-08-20 | [Doob's h-transform](https://letter-night.tistory.com/1455) | Generative Models_2 | [doobs-h-transform.md](../topics/generative-models/concepts/doobs-h-transform.md) · 개념 노트 (스텁) |
| 2026-08-20 | [SB와 score-based diffusion model의 차이](https://letter-night.tistory.com/1454) | Generative Models_2 | [sb-vs-score-based-diffusion.md](../topics/generative-models/concepts/sb-vs-score-based-diffusion.md) · 개념 노트 (스텁) |
| 2026-08-19 | [SB를 알아가고 있다](https://letter-night.tistory.com/1453) | Generative Models_2 | [2026-08-19-getting-to-know-sb.md](../topics/generative-models/thoughts/2026-08-19-getting-to-know-sb.md) · 스텁 |
| 2026-08-18 | [Feynman Kac Formula](https://letter-night.tistory.com/1452) | Generative Models_2 | [feynman-kac-formula.md](../topics/generative-models/concepts/feynman-kac-formula.md) · 개념 노트 (스텁) |
| 2026-08-18 | [SB framework 안에서 DM와 FM의 탄생 비화를 깨닫고 있다](https://letter-night.tistory.com/1451) | Generative Models_2 | [2026-08-18-birth-of-dm-and-fm-within-sb.md](../topics/generative-models/thoughts/2026-08-18-birth-of-dm-and-fm-within-sb.md) · 요약 이전 |
| 2026-08-17 | [흥미로운 공통점 찾음! (Distribution Matching)](https://letter-night.tistory.com/1449) | Generative Models_2 | [2026-08-17-sb-and-dpg-same-form.md](../topics/generative-models/thoughts/2026-08-17-sb-and-dpg-same-form.md) · 요약 이전 |
| 2026-08-16 | [[on-going] Foundations of SBs for Generative Modeling](https://letter-night.tistory.com/1447) | Generative Models_2 | [2025-foundations-of-sb-generative-modeling.md](../topics/generative-models/papers/2025-foundations-of-sb-generative-modeling.md) · 논문 노트 (스텁) |
| 2026-08-15 | [Schrodinger Bridge solution as two space-time potentials](https://letter-night.tistory.com/1445) | Generative Models_2 | [sb-two-space-time-potentials.md](../topics/generative-models/concepts/sb-two-space-time-potentials.md) · 개념 노트 (스텁) |
| 2026-08-15 | [[thought 2] generative model의 training efficiency에 대해서](https://letter-night.tistory.com/1444) | Generative Models_2 | [2026-08-15-training-efficiency-as-optimal-flow.md](../topics/generative-models/thoughts/2026-08-15-training-efficiency-as-optimal-flow.md) · 요약 이전 |
| 2026-08-13 | [Understanding Girsanov's theorem intuitively](https://letter-night.tistory.com/1442) | Generative Models_2 | [girsanov-theorem.md](../topics/generative-models/concepts/girsanov-theorem.md) · 개념 노트 (스텁) |
| 2026-08-04 | [[thought] generative model의 training efficiency에 대해서](https://letter-night.tistory.com/1433) | Generative Models_2 | [2026-08-15-training-efficiency-as-optimal-flow.md](../topics/generative-models/thoughts/2026-08-15-training-efficiency-as-optimal-flow.md) · 요약 이전 |
| 2026-08-02 | [[on-going] The Principles of Diffusion Models](https://letter-night.tistory.com/1431) | Generative Models_2 | [2025-principles-of-diffusion-models.md](../topics/generative-models/papers/2025-principles-of-diffusion-models.md) · 논문 노트 (스텁) |
| 2026-07-31 | [push forward](https://letter-night.tistory.com/1429) | Generative Models_2 | [push-forward.md](../topics/generative-models/concepts/push-forward.md) · 개념 노트 (스텁) |
| 2026-07-30 | [Derivation of continuity eqn & Fokker-Planck eqn](https://letter-night.tistory.com/1428) | Generative Models_2 | [continuity-and-fokker-planck.md](../topics/generative-models/concepts/continuity-and-fokker-planck.md) · 개념 노트 (스텁) |
| 2026-04-26 | [[on-going] Diffusion Language Models](https://letter-night.tistory.com/1309) | Generative Models_2 | [diffusion-language-models-overview.md](../topics/generative-models/papers/diffusion-language-models-overview.md) · 논문 노트 (스텁) |
| 2026-04-25 | [[on-going] Flow Matching & Diffusion Models](https://letter-night.tistory.com/1308) | Generative Models_2 | [flow-matching-and-diffusion-models-notes.md](../topics/generative-models/papers/flow-matching-and-diffusion-models-notes.md) · 논문 노트 (스텁) |

## AgenticAI (13)
| 작성일 | 원문 | 원 카테고리 | 새 위치 · 처리 |
|---|---|---|---|
| 2026-11-22 | [[thought] 그렇다면 Agent는 정말로 human보다 intelligent한가?](https://letter-night.tistory.com/1521) | AgenticAI | [2026-11-22-is-agent-more-intelligent-than-human.md](../topics/agentic-ai/thoughts/2026-11-22-is-agent-more-intelligent-than-human.md) · 요약 이전 |
| 2026-11-21 | [[One dawn across science] Riemann hypothesis solved by Claude](https://letter-night.tistory.com/1519) | AgenticAI | [2026-11-21-ai-for-science-humility.md](../topics/agentic-ai/thoughts/2026-11-21-ai-for-science-humility.md) · 요약 이전 |
| 2026-11-14 | [그냥 문득 든 생각들](https://letter-night.tistory.com/1515) | AgenticAI | [2026-11-14-random-thoughts-ontology-and-work-knowledge.md](../topics/agentic-ai/thoughts/2026-11-14-random-thoughts-ontology-and-work-knowledge.md) · 요약 이전 |
| 2026-10-11 | [Why Agents Need Causal World Models](https://letter-night.tistory.com/1497) | AgenticAI | [2026-10-11-why-agents-need-causal-world-models.md](../topics/agentic-ai/thoughts/2026-10-11-why-agents-need-causal-world-models.md) · 요약 이전 |
| 2026-09-11 | [[CMU Fall 2026] AI Agents](https://letter-night.tistory.com/1483) | AgenticAI | [cmu-11768-ai-agents-f26.md](../topics/agentic-ai/lectures/cmu-11768-ai-agents-f26.md) · 강의 노트 |
| 2026-09-11 | [[MIT Spring 2026] Multimodal AI](https://letter-night.tistory.com/1482) | AgenticAI | [mit-multimodal-ai-s26.md](../topics/agentic-ai/lectures/mit-multimodal-ai-s26.md) · 강의 노트 |
| 2026-08-31 | [Autonomous Agent Societies](https://letter-night.tistory.com/1477) | AgenticAI | [2026-08-31-autonomous-agent-societies.md](../topics/agentic-ai/thoughts/2026-08-31-autonomous-agent-societies.md) · 요약 이전 |
| 2026-08-09 | [Ontology & Knowledge Graph](https://letter-night.tistory.com/1439) | AgenticAI | [dsba-ontology-knowledge-graph-2026.md](../topics/agentic-ai/lectures/dsba-ontology-knowledge-graph-2026.md) · 강의 노트 |
| 2026-08-09 | [Self-Improving AI Agents](https://letter-night.tistory.com/1438) | AgenticAI | [stanford-cs329a-self-improving-agents.md](../topics/agentic-ai/lectures/stanford-cs329a-self-improving-agents.md) · 강의 노트 |
| 2026-05-08 | [Agent AI 좋은 영상](https://letter-night.tistory.com/1326) | AgenticAI | [dsba-agent-ai-2026.md](../topics/agentic-ai/lectures/dsba-agent-ai-2026.md) · 강의 노트 |
| 2025-07-18 | [Human이랑 똑같네](https://letter-night.tistory.com/925) | AgenticAI | [2025-07-18-agents-are-like-humans.md](../topics/agentic-ai/thoughts/2025-07-18-agents-are-like-humans.md) · 요약 이전 |
| 2025-07-18 | [AI Agents](https://letter-night.tistory.com/924) | AgenticAI | [emnlp2024-language-agents-tutorial.md](../topics/agentic-ai/lectures/emnlp2024-language-agents-tutorial.md) · 강의 노트 |
| 2025-07-17 | [Agents](https://letter-night.tistory.com/922) | AgenticAI | [chip-huyen-agents.md](../topics/agentic-ai/posts/chip-huyen-agents.md) · 링크만 (원문이 외부 글 전재) |

## LLMs (86)
| 작성일 | 원문 | 원 카테고리 | 새 위치 · 처리 |
|---|---|---|---|
| 2026-10-13 | [Continuous diffusion language models](https://letter-night.tistory.com/1501) | LLMs/Diffusion | [continuous-diffusion-language-models.md](../topics/generative-models/papers/continuous-diffusion-language-models.md) · 논문 노트 (스텁) |
| 2026-08-30 | [The mathematics of AI uncertainty](https://letter-night.tistory.com/1475) | LLMs | [mathematics-of-ai-uncertainty.md](../background/videos/mathematics-of-ai-uncertainty.md) · 영상 노트 |
| 2026-08-30 | [[취향저격 3] The mathematics of AI uncertainty](https://letter-night.tistory.com/1471) | LLMs | [mathematics-of-ai-uncertainty.md](../background/videos/mathematics-of-ai-uncertainty.md) · 영상 노트 |
| 2026-07-27 | [빠른 포기 & 공부 그만](https://letter-night.tistory.com/1424) | LLMs/Interpretability | 보류 — 개인 회고(연구 중단 결심). 연구 기록과 성격이 달라 이전하지 않음. 원하면 journal 폴더로 이전 |
| 2026-07-26 | [그간의 생각 정리, 근데 너무 어려움](https://letter-night.tistory.com/1423) | LLMs/Interpretability | [2026-07-26-research-process-proposal-is-hard.md](../topics/mech-interp/thoughts/2026-07-26-research-process-proposal-is-hard.md) · 요약 이전 |
| 2026-07-24 | [human이랑 다를 게 뭔가?](https://letter-night.tistory.com/1421) | LLMs/Etc | [2026-07-24-how-different-from-humans.md](../topics/mech-interp/thoughts/2026-07-24-how-different-from-humans.md) · 요약 이전 |
| 2026-07-20 | [Pygmalion Effect - LLM의 identity 형성](https://letter-night.tistory.com/1419) | LLMs/Interpretability | [2026-07-20-pygmalion-effect-llm-identity.md](../topics/mech-interp/thoughts/2026-07-20-pygmalion-effect-llm-identity.md) · 요약 이전 |
| 2026-07-20 | [thought](https://letter-night.tistory.com/1418) | LLMs/Interpretability | [2026-07-20-j-lens-vs-attribution-graph.md](../topics/mech-interp/thoughts/2026-07-20-j-lens-vs-attribution-graph.md) · 요약 이전 |
| 2026-07-19 | [Thought on Mechanistic interpretability](https://letter-night.tistory.com/1416) | LLMs/Interpretability | [2026-07-19-thought-on-mechanistic-interpretability.md](../topics/mech-interp/thoughts/2026-07-19-thought-on-mechanistic-interpretability.md) · 요약 이전 |
| 2026-07-18 | [A global workspace in language models](https://letter-night.tistory.com/1415) | LLMs/Interpretability | [2026-global-workspace-in-language-models.md](../topics/mech-interp/papers/2026-global-workspace-in-language-models.md) · 논문 노트 (스텁) |
| 2026-07-18 | [Natural Language Autoencoders: Turning Claude's thoughts into text](https://letter-night.tistory.com/1414) | LLMs/Interpretability | [2026-natural-language-autoencoders.md](../topics/mech-interp/papers/2026-natural-language-autoencoders.md) · 논문 노트 (스텁) |
| 2026-07-18 | [[★circuit tracing tools★] what's going on inside LMs?](https://letter-night.tistory.com/1413) | LLMs/Interpretability | [circuit-tracing-tools.md](../topics/mech-interp/concepts/circuit-tracing-tools.md) · 개념 노트 (스텁) |
| 2026-07-18 | [★ 궁금증 해결 방법 찾음 ★ Similar approach (but other domain)](https://letter-night.tistory.com/1412) | LLMs/Etc | [2026-07-18-mi-for-medical-diagnosis-reliability.md](../topics/mech-interp/thoughts/2026-07-18-mi-for-medical-diagnosis-reliability.md) · 요약 이전 |
| 2026-07-15 | [[★on-going★] Anthropic publications 정주행](https://letter-night.tistory.com/1410) | LLMs/Interpretability | [README.md](../topics/mech-interp/README.md) · 목록 병합 (논문 노트로 분리) |
| 2026-07-15 | [LLM-Agents Grounded in Self-Reports Enable General-Purpose Simulation of Individuals](https://letter-night.tistory.com/1409) | LLMs/Etc | [llm-agents-grounded-in-self-reports.md](../topics/agentic-ai/papers/llm-agents-grounded-in-self-reports.md) · 논문 노트 (스텁) |
| 2026-07-15 | [thought 3](https://letter-night.tistory.com/1408) | LLMs/Etc | [2026-07-15-persona-agents-thought-3-which-stimulus.md](../topics/agentic-ai/thoughts/2026-07-15-persona-agents-thought-3-which-stimulus.md) · 요약 이전 |
| 2026-07-14 | [PATIENT-Ψ: Using Large Language Models to Simulate Patients for Training Mental Health Professionals](https://letter-night.tistory.com/1407) | LLMs/Etc | [2024-patient-psi.md](../topics/agentic-ai/papers/2024-patient-psi.md) · 논문 노트 (스텁) |
| 2026-07-14 | [Two Tales of Persona in LLMs: A Survey of Role-Playing and Personalization](https://letter-night.tistory.com/1406) | LLMs/Etc | [2024-two-tales-of-persona.md](../topics/agentic-ai/papers/2024-two-tales-of-persona.md) · 논문 노트 (스텁) |
| 2026-07-14 | [thought 2](https://letter-night.tistory.com/1405) | LLMs/Etc | [2026-07-14-persona-agents-thought-2-unbiased-judge.md](../topics/agentic-ai/thoughts/2026-07-14-persona-agents-thought-2-unbiased-judge.md) · 요약 이전 |
| 2026-07-14 | [thought 1](https://letter-night.tistory.com/1404) | LLMs/Etc | [2026-07-14-persona-agents-thought-1.md](../topics/agentic-ai/thoughts/2026-07-14-persona-agents-thought-1.md) · 요약 이전 |
| 2026-07-12 | [Virtual Society](https://letter-night.tistory.com/1403) | LLMs/Etc | [2026-07-12-virtual-society-persona-simulation.md](../topics/agentic-ai/thoughts/2026-07-12-virtual-society-persona-simulation.md) · 요약 이전 |
| 2026-07-12 | [FlockVote: LLM-empowered Agent-based Modeling for Simulating U.S. Presidential Elections](https://letter-night.tistory.com/1402) | LLMs/Etc | [2024-flockvote.md](../topics/agentic-ai/papers/2024-flockvote.md) · 논문 노트 (스텁) |
| 2026-07-12 | [Persona-driven Simulation of Voting Behavior in the European Parliament with LLMs](https://letter-night.tistory.com/1401) | LLMs/Etc | [2025-persona-voting-european-parliament.md](../topics/agentic-ai/papers/2025-persona-voting-european-parliament.md) · 논문 노트 (스텁) |
| 2026-07-11 | [Out of One, Many: Using LMs to Simulate Human Samples](https://letter-night.tistory.com/1400) | LLMs/Etc | [2023-out-of-one-many.md](../topics/agentic-ai/papers/2023-out-of-one-many.md) · 논문 노트 (스텁) |
| 2026-06-19 | [A Circuit for Indirect Object Identification in GPT-2 Small](https://letter-night.tistory.com/1384) | LLMs/Interpretability | [2022-ioi-circuit-gpt2-small.md](../topics/mech-interp/papers/2022-ioi-circuit-gpt2-small.md) · 논문 노트 (스텁) |
| 2026-06-18 | [Finding Alignments Between Interpretable Causal Variables and Distributed Neural Representations](https://letter-night.tistory.com/1383) | LLMs/Interpretability | [2023-das-finding-alignments.md](../topics/mech-interp/papers/2023-das-finding-alignments.md) · 논문 노트 (스텁) |
| 2026-06-18 | [How to use and interpret activation patching](https://letter-night.tistory.com/1382) | LLMs/Interpretability | [2024-activation-patching-how-to.md](../topics/mech-interp/papers/2024-activation-patching-how-to.md) · 논문 노트 (스텁) |
| 2026-06-18 | [The Hydra Effect: Emergent Self-repair in LM Computations](https://letter-night.tistory.com/1381) | LLMs/Interpretability | [2023-hydra-effect.md](../topics/mech-interp/papers/2023-hydra-effect.md) · 논문 노트 (스텁) |
| 2026-06-18 | [Causal Abstractions of Neural Networks](https://letter-night.tistory.com/1380) | LLMs/Interpretability | [2021-causal-abstractions-of-neural-networks.md](../topics/mech-interp/papers/2021-causal-abstractions-of-neural-networks.md) · 논문 노트 (스텁) |
| 2026-06-17 | [Features](https://letter-night.tistory.com/1378) | LLMs/Interpretability | [features.md](../topics/mech-interp/concepts/features.md) · 개념 노트 (스텁) |
| 2026-06-17 | [Causal Abstraction](https://letter-night.tistory.com/1377) | LLMs/Interpretability | [causal-abstraction.md](../topics/mech-interp/concepts/causal-abstraction.md) · 개념 노트 (스텁) |
| 2026-06-17 | [Circuits](https://letter-night.tistory.com/1376) | LLMs/Interpretability | [circuits.md](../topics/mech-interp/concepts/circuits.md) · 개념 노트 (스텁) |
| 2026-06-17 | [Activation Patching](https://letter-night.tistory.com/1375) | LLMs/Interpretability | [activation-patching.md](../topics/mech-interp/concepts/activation-patching.md) · 개념 노트 (스텁) |
| 2026-06-15 | [생성모델 관점에서 생각해보더라도](https://letter-night.tistory.com/1371) | LLMs/Interpretability | [2026-06-15-generative-model-view-of-mi.md](../topics/mech-interp/thoughts/2026-06-15-generative-model-view-of-mi.md) · 요약 이전 |
| 2026-06-15 | [어떻게 보면, LLM은 거대한 graph database retrieval system 같기도 해](https://letter-night.tistory.com/1370) | LLMs/Interpretability | [2026-06-15-llm-as-graph-database-retrieval.md](../topics/mech-interp/thoughts/2026-06-15-llm-as-graph-database-retrieval.md) · 요약 이전 |
| 2026-06-14 | [(2/2) Right Mediator: MI Through the Lens of Causal Mediation Analysis](https://letter-night.tistory.com/1369) | LLMs/Interpretability | [2024-mi-through-causal-mediation.md](../topics/mech-interp/papers/2024-mi-through-causal-mediation.md) · 논문 노트 (스텁) |
| 2026-06-14 | [(1/2) Right Mediator: MI Through the Lens of Causal Mediation Analysis](https://letter-night.tistory.com/1368) | LLMs/Interpretability | [2024-mi-through-causal-mediation.md](../topics/mech-interp/papers/2024-mi-through-causal-mediation.md) · 논문 노트 (스텁) |
| 2026-06-13 | [(3/3) A Primer on the Inner Workings of Transformer-based LMs](https://letter-night.tistory.com/1367) | LLMs/Interpretability | [2024-primer-inner-workings-transformer-lms.md](../topics/mech-interp/papers/2024-primer-inner-workings-transformer-lms.md) · 논문 노트 (스텁) |
| 2026-06-13 | [(2/3) A Primer on the Inner Workings of Transformer-based LMs](https://letter-night.tistory.com/1366) | LLMs/Interpretability | [2024-primer-inner-workings-transformer-lms.md](../topics/mech-interp/papers/2024-primer-inner-workings-transformer-lms.md) · 논문 노트 (스텁) |
| 2026-06-12 | [(1/3) A Primer on the Inner Workings of Transformer-based LMs](https://letter-night.tistory.com/1365) | LLMs/Interpretability | [2024-primer-inner-workings-transformer-lms.md](../topics/mech-interp/papers/2024-primer-inner-workings-transformer-lms.md) · 논문 노트 (스텁) |
| 2026-06-11 | [[흥미로운 예시] Automating psychological hypothesis generation with AI: when LLMs meet causal graph](https://letter-night.tistory.com/1363) | LLMs/Interpretability | [2024-llm-causal-graph-psych-hypothesis.md](../topics/causality/papers/2024-llm-causal-graph-psych-hypothesis.md) · 논문 노트 |
| 2026-06-11 | [(Review) Mechanistic Interpretability](https://letter-night.tistory.com/1362) | LLMs/Interpretability | [README.md](../topics/mech-interp/README.md) · 목록 병합 (필수 읽기 경로) |
| 2026-06-10 | [[Draft] Testing SCM Faithfulness in LLM Internals](https://letter-night.tistory.com/1361) | LLMs/Interpretability | [I01-scm-faithfulness-in-llm-internals.md](../ideas/I01-scm-faithfulness-in-llm-internals.md) · 아이디어로 이전 (요약) |
| 2026-06-10 | [[on-going (until next week)] research question](https://letter-night.tistory.com/1360) | LLMs/Interpretability | [I01-scm-faithfulness-in-llm-internals.md](../ideas/I01-scm-faithfulness-in-llm-internals.md) · 아이디어로 이전 (요약) |
| 2026-06-04 | [Project presentation](https://letter-night.tistory.com/1356) | LLMs/Diffusion | [README.md](../projects/diffusion-lm-distributional-failure/README.md) · 프로젝트 기록 (스텁) |
| 2026-06-04 | [[on-going] The Geometry of Categorical & Hierarchical Concepts in LLMs](https://letter-night.tistory.com/1355) | LLMs/Interpretability | [2024-geometry-categorical-hierarchical-concepts.md](../topics/mech-interp/papers/2024-geometry-categorical-hierarchical-concepts.md) · 논문 노트 (스텁) |
| 2026-06-03 | [Training Compute-Optimal Large Language Models](https://letter-night.tistory.com/1352) | LLMs/Etc | [2022-chinchilla-compute-optimal.md](../background/papers/2022-chinchilla-compute-optimal.md) · 논문 노트 (스텁) |
| 2026-06-02 | [Diagnostic Study of Distributional Failure in Diffusion LMs](https://letter-night.tistory.com/1350) | LLMs/Diffusion | [README.md](../projects/diffusion-lm-distributional-failure/README.md) · 프로젝트 기록 (스텁) |
| 2026-05-27 | [Proposal presentation](https://letter-night.tistory.com/1344) | LLMs/Diffusion | [README.md](../projects/diffusion-lm-distributional-failure/README.md) · 프로젝트 기록 (스텁) |
| 2026-05-15 | [ELBO approximation](https://letter-night.tistory.com/1338) | LLMs/Diffusion | [elbo-approximation-diffusion-lm.md](../topics/generative-models/concepts/elbo-approximation-diffusion-lm.md) · 개념 노트 (스텁) |
| 2026-05-10 | [[VRPO] LLaDA 1.5: Variance-Reduced Preference Optimization for Large Language Diffusion Models](https://letter-night.tistory.com/1333) | LLMs/Diffusion | [2025-llada-1-5-vrpo.md](../topics/generative-models/papers/2025-llada-1-5-vrpo.md) · 논문 노트 (스텁) |
| 2026-05-09 | [Research Proposal](https://letter-night.tistory.com/1331) | LLMs/Diffusion | [README.md](../projects/diffusion-lm-distributional-failure/README.md) · 프로젝트 기록 (스텁) |
| 2026-05-09 | [[CDPG] Controlling Conditional Language Models](https://letter-night.tistory.com/1330) | LLMs/Diffusion | [2022-cdpg.md](../topics/generative-models/papers/2022-cdpg.md) · 논문 노트 (스텁) |
| 2026-05-09 | [[KL-Adaptive DPG w/ baseline] RL and DM for Fine-tuning LMs](https://letter-night.tistory.com/1329) | LLMs/Diffusion | [2022-rl-vs-distribution-matching-finetuning.md](../topics/generative-models/papers/2022-rl-vs-distribution-matching-finetuning.md) · 논문 노트 (스텁) |
| 2026-05-09 | [[KL-Adaptive DPG] Distributional Approach to Controlled Text Generation](https://letter-night.tistory.com/1328) | LLMs/Diffusion | [2021-distributional-approach-controlled-generation.md](../topics/generative-models/papers/2021-distributional-approach-controlled-generation.md) · 논문 노트 (스텁) |
| 2026-05-08 | [[D-CFG] Simple Guidance Mechanism for Discrete Diffusion Models](https://letter-night.tistory.com/1327) | LLMs/Diffusion | [2024-discrete-diffusion-guidance.md](../topics/generative-models/papers/2024-discrete-diffusion-guidance.md) · 논문 노트 (스텁) |
| 2026-05-07 | [[d1] Scaling Reasoning in dLLMs via RL](https://letter-night.tistory.com/1325) | LLMs/Diffusion | [2025-d1-reasoning-dllm-rl.md](../topics/generative-models/papers/2025-d1-reasoning-dllm-rl.md) · 논문 노트 (스텁) |
| 2026-05-07 | [[LLaDA] Large Language Diffusion Models](https://letter-night.tistory.com/1324) | LLMs/Diffusion | [2025-llada.md](../topics/generative-models/papers/2025-llada.md) · 논문 노트 (스텁) |
| 2026-05-05 | [[MDLMs] Simple and Effective Masked Diffusion Language Models](https://letter-night.tistory.com/1323) | LLMs/Diffusion | [2024-mdlm.md](../topics/generative-models/papers/2024-mdlm.md) · 논문 노트 (스텁) |
| 2026-04-28 | [GRPO](https://letter-night.tistory.com/1312) | LLMs/Reasoning | [grpo.md](../topics/agentic-ai/concepts/grpo.md) · 개념 노트 (스텁) |
| 2026-01-12 | [그렇다면 Mechanistic Interpretability는 LLM이 causal reasoning을 할 수 있다는 증거 아닌감?](https://letter-night.tistory.com/1190) | LLMs/Interpretability | [2026-01-12-is-mi-evidence-of-causal-reasoning.md](../topics/mech-interp/thoughts/2026-01-12-is-mi-evidence-of-causal-reasoning.md) · 요약 이전 |
| 2026-01-09 | [!! Mechanistic Interpretability가 Causal Representation & discovery에 답을 주었다!!](https://letter-night.tistory.com/1187) | LLMs/Interpretability | [2026-01-09-mi-answers-causal-representation.md](../topics/mech-interp/thoughts/2026-01-09-mi-answers-causal-representation.md) · 요약 이전 |
| 2026-01-09 | [[Circuit Tracing Examples 1] Multi-Step Reasoning](https://letter-night.tistory.com/1186) | LLMs/Interpretability | [2025-biology-of-a-large-language-model.md](../topics/mech-interp/papers/2025-biology-of-a-large-language-model.md) · 논문 노트 (스텁) |
| 2026-01-09 | [[Circuit Tracing Examples 0] Methodology](https://letter-night.tistory.com/1185) | LLMs/Interpretability | [2025-biology-of-a-large-language-model.md](../topics/mech-interp/papers/2025-biology-of-a-large-language-model.md) · 논문 노트 (스텁) |
| 2026-01-09 | [Circuit Tracing: Revealing Computational Graphs in Language Models](https://letter-night.tistory.com/1183) | LLMs/Interpretability | [2025-circuit-tracing.md](../topics/mech-interp/papers/2025-circuit-tracing.md) · 논문 노트 (스텁) |
| 2026-01-08 | [[Crosscoders] Sparse Crosscoders for Cross-Layer Features and Model Diffing](https://letter-night.tistory.com/1182) | LLMs/Interpretability | [2024-crosscoders.md](../topics/mech-interp/papers/2024-crosscoders.md) · 논문 노트 (스텁) |
| 2026-01-08 | [[Transcoders] Find Interpretable LLM Feature Circuits](https://letter-night.tistory.com/1181) | LLMs/Interpretability | [2024-transcoders.md](../topics/mech-interp/papers/2024-transcoders.md) · 논문 노트 (스텁) |
| 2026-01-07 | [Scaling Monosemanticity: Extracting Interpretable Features from Claude 3 Sonnet](https://letter-night.tistory.com/1180) | LLMs/Interpretability | [2024-scaling-monosemanticity.md](../topics/mech-interp/papers/2024-scaling-monosemanticity.md) · 논문 노트 (스텁) |
| 2026-01-06 | [Towards Monosemanticity: Decomposing Language Models With Dictionary Learning](https://letter-night.tistory.com/1179) | LLMs/Interpretability | [2023-towards-monosemanticity.md](../topics/mech-interp/papers/2023-towards-monosemanticity.md) · 논문 노트 (스텁) |
| 2026-01-06 | [Superposition](https://letter-night.tistory.com/1178) | LLMs/Interpretability | [superposition.md](../topics/mech-interp/concepts/superposition.md) · 개념 노트 (스텁) |
| 2026-01-06 | [Why induction head in Transformer is important for meta-learning?](https://letter-night.tistory.com/1176) | LLMs/Interpretability | [induction-heads-and-meta-learning.md](../topics/mech-interp/concepts/induction-heads-and-meta-learning.md) · 개념 노트 (스텁) |
| 2026-01-06 | [Transformer Circuits](https://letter-night.tistory.com/1175) | LLMs/Interpretability | [transformer-circuits.md](../topics/mech-interp/concepts/transformer-circuits.md) · 개념 노트 (스텁) |
| 2026-01-05 | [Circuits](https://letter-night.tistory.com/1174) | LLMs/Interpretability | [circuits.md](../topics/mech-interp/concepts/circuits.md) · 개념 노트 (스텁) |
| 2026-01-05 | [(Gentle Intro..) [Interpretability] how LLMs really work](https://letter-night.tistory.com/1172) | LLMs/Interpretability | [gentle-intro-how-llms-work.md](../topics/mech-interp/concepts/gentle-intro-how-llms-work.md) · 개념 노트 (스텁) |
| 2026-01-05 | [Misc](https://letter-night.tistory.com/1171) | LLMs/Etc | [llm-misc.md](../background/concepts/llm-misc.md) · 개념 노트 (스텁) |
| 2026-01-04 | [[COCONUT] Training LLMs to Reason in a Continuous Latent Space](https://letter-night.tistory.com/1170) | LLMs/Reasoning | [2024-coconut.md](../topics/agentic-ai/papers/2024-coconut.md) · 논문 노트 (스텁) |
| 2026-01-04 | [s1: Simple test-time scaling](https://letter-night.tistory.com/1169) | LLMs/Reasoning | [2025-s1-test-time-scaling.md](../topics/agentic-ai/papers/2025-s1-test-time-scaling.md) · 논문 노트 (스텁) |
| 2026-01-03 | [LoRA Without Regret](https://letter-night.tistory.com/1168) | LLMs/Etc | [lora-without-regret.md](../background/posts/lora-without-regret.md) · 외부 글 노트 (스텁) |
| 2026-01-03 | [Speculative Decoding](https://letter-night.tistory.com/1167) | LLMs/Etc | [speculative-decoding.md](../background/concepts/speculative-decoding.md) · 개념 노트 (스텁) |
| 2026-01-02 | [[Dr.GRPO] Understanding R1-Zero-Like Training: A Critical Perspective](https://letter-night.tistory.com/1166) | LLMs/Reasoning | [2025-dr-grpo.md](../topics/agentic-ai/papers/2025-dr-grpo.md) · 논문 노트 (스텁) |
| 2026-01-02 | [[DeepSeek-R1] Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://letter-night.tistory.com/1165) | LLMs/Reasoning | [2025-deepseek-r1.md](../topics/agentic-ai/papers/2025-deepseek-r1.md) · 논문 노트 (스텁) |
| 2026-01-02 | [[DeepSeekMath] Pushing the Limits of Mathematical Reasoning in Open LMs](https://letter-night.tistory.com/1164) | LLMs/Reasoning | [2024-deepseekmath.md](../topics/agentic-ai/papers/2024-deepseekmath.md) · 논문 노트 (스텁) |
| 2026-01-01 | [Likelihood-Based Diffusion Language Models](https://letter-night.tistory.com/1163) | LLMs/Diffusion | [2023-likelihood-based-diffusion-lms.md](../topics/generative-models/papers/2023-likelihood-based-diffusion-lms.md) · 논문 노트 (스텁) |
| 2025-12-31 | [Diffusion-LM Improves Controllable Text Generation](https://letter-night.tistory.com/1162) | LLMs/Diffusion | [2022-diffusion-lm.md](../topics/generative-models/papers/2022-diffusion-lm.md) · 논문 노트 (스텁) |
| 2025-12-31 | [(On-going) Mixture-of-Experts](https://letter-night.tistory.com/1160) | LLMs/Reasoning | [mixture-of-experts.md](../background/concepts/mixture-of-experts.md) · 개념 노트 (스텁) |
| 2025-12-30 | [(On-going) Review of LLM](https://letter-night.tistory.com/1158) | LLMs/Etc | [review-of-llm.md](../background/concepts/review-of-llm.md) · 개념 노트 (스텁) |

## Causality (48)
| 작성일 | 원문 | 원 카테고리 | 새 위치 · 처리 |
|---|---|---|---|
| 2026-11-22 | [[thought] RL Agent 와의 차이점](https://letter-night.tistory.com/1520) | Causality/thought | [2026-11-22-rl-agent-vs-causal-agent.md](../topics/causality/thoughts/2026-11-22-rl-agent-vs-causal-agent.md) · 요약 이전 |
| 2026-11-20 | [Causality (Judea Pearl) & What If (Hernan & Robins)](https://letter-night.tistory.com/1518) | Causality/thought | [2026-11-20-reading-pearl-and-what-if.md](../topics/causality/thoughts/2026-11-20-reading-pearl-and-what-if.md) · 요약 이전 |
| 2026-11-18 | [time-varying treatments with time-varying confounders](https://letter-night.tistory.com/1517) | Causality/Judea Pearl | [2026-11-18-time-varying-treatment-as-plan-evaluation.md](../topics/causality/thoughts/2026-11-18-time-varying-treatment-as-plan-evaluation.md) · 요약 이전 |
| 2026-11-11 | [★ 고전의 중요성 2탄 ★](https://letter-night.tistory.com/1514) | Causality/thought | [2026-11-11-importance-of-classics-2.md](../topics/causality/thoughts/2026-11-11-importance-of-classics-2.md) · 요약 이전 |
| 2026-11-11 | [memo](https://letter-night.tistory.com/1513) | Causality/Judea Pearl | [pearl-causality.md](../topics/causality/books/pearl-causality.md) · 읽기 메모 병합 |
| 2026-11-10 | [여전한 믿음 ㅎㅎ](https://letter-night.tistory.com/1512) | Causality/thought | [2026-11-10-unchanged-belief-longitudinal-causal-fm.md](../topics/causality/thoughts/2026-11-10-unchanged-belief-longitudinal-causal-fm.md) · 요약 이전 |
| 2026-11-09 | [★ 고전의 중요성 ★](https://letter-night.tistory.com/1511) | Causality/thought | [2026-11-09-importance-of-classics.md](../topics/causality/thoughts/2026-11-09-importance-of-classics.md) · 요약 이전 |
| 2026-11-08 | [causal inference 를 공부하며 3탄](https://letter-night.tistory.com/1510) | Causality/thought | [2026-11-08-studying-causal-inference-3.md](../topics/causality/thoughts/2026-11-08-studying-causal-inference-3.md) · 요약 이전 |
| 2026-11-05 | [[부치지 못한 편지 2] Causal effect under time-varying treatment](https://letter-night.tistory.com/1508) | Causality/thought | [2026-11-05-causal-effect-under-time-varying-treatment.md](../topics/causality/thoughts/2026-11-05-causal-effect-under-time-varying-treatment.md) · 요약 이전 |
| 2026-08-09 | [TabFM](https://letter-night.tistory.com/1440) | Causality/paper | [google-tabfm.md](../topics/causality/posts/google-tabfm.md) · 외부 글 노트 |
| 2026-04-18 | [몇 번이나 쓴 적이 있지만 오랜만에 또 쓰는 글..ㅎ](https://letter-night.tistory.com/1302) | Causality/thought | [2026-04-18-knowing-the-mechanism-behind-phenomena.md](../topics/causality/thoughts/2026-04-18-knowing-the-mechanism-behind-phenomena.md) · 요약 이전 |
| 2026-03-30 | [[IGC-Net] CAPO Estimation over Time](https://letter-night.tistory.com/1271) | Causality/paper | [igc-net.md](../topics/causality/papers/igc-net.md) · 논문 노트 (스텁) |
| 2026-03-01 | [[GT] G-Transformer: Counterfactual Outcome Prediction under Dynamic and Time-varying Treatment Regimes](https://letter-night.tistory.com/1234) | Causality/paper | [2024-g-transformer.md](../topics/causality/papers/2024-g-transformer.md) · 논문 노트 (스텁) |
| 2026-02-19 | [[SCIP-Net] Stabilized Neural Prediction of Potential Outcomes in Continuous Time](https://letter-night.tistory.com/1227) | Causality/paper | [2025-scip-net.md](../topics/causality/papers/2025-scip-net.md) · 논문 노트 (스텁) |
| 2026-02-19 | [[G-Net] a Recurrent Network Approach to G-Computation for Counterfactual Prediction Under a Dynamic Treatment Regime](https://letter-night.tistory.com/1226) | Causality/paper | [2021-g-net.md](../topics/causality/papers/2021-g-net.md) · 논문 노트 (스텁) |
| 2026-02-19 | [[RMSNs] Forecasting Treatment Responses Over Time Using Recurrent Marginal Structural Networks](https://letter-night.tistory.com/1225) | Causality/paper | [2018-rmsn.md](../topics/causality/papers/2018-rmsn.md) · 논문 노트 (스텁) |
| 2026-02-19 | [[CT] Causal Transformer for Estimating Counterfactual Outcomes](https://letter-night.tistory.com/1224) | Causality/paper | [2022-causal-transformer.md](../topics/causality/papers/2022-causal-transformer.md) · 논문 노트 (스텁) |
| 2026-02-18 | [[CRN] Estimating Counterfactual Treatment Outcomes over Time through Adversarially Balanced Representations](https://letter-night.tistory.com/1223) | Causality/paper | [2020-crn.md](../topics/causality/papers/2020-crn.md) · 논문 노트 (스텁) |
| 2026-01-19 | [[BNCDE] Bayesian Neural CDEs for Treatment Effect Estimation](https://letter-night.tistory.com/1196) | Causality/paper | [2024-bncde.md](../topics/causality/papers/2024-bncde.md) · 논문 노트 (스텁) |
| 2026-01-19 | [Continuous-Time Modeling of Counterfactual Outcomes Using Neural CDEs](https://letter-night.tistory.com/1195) | Causality/paper | [2022-te-cde.md](../topics/causality/papers/2022-te-cde.md) · 논문 노트 (스텁) |
| 2026-01-17 | [[TimePFN] MTS Forecasting with Synthetic Data](https://letter-night.tistory.com/1194) | Causality/paper | [2025-timepfn.md](../topics/causality/papers/2025-timepfn.md) · 논문 노트 (스텁) |
| 2026-01-14 | [[CausalFM] Foundation Models for Causal Inference via PFNs](https://letter-night.tistory.com/1193) | Causality/paper | [2025-causalfm.md](../topics/causality/papers/2025-causalfm.md) · 논문 노트 (스텁) |
| 2026-01-14 | [정말로 implicit하게 causal graph를 찾고, 추론하였을까?](https://letter-night.tistory.com/1192) | Causality/thought | [2026-01-14-did-pfn-find-causal-graph-implicitly.md](../topics/causality/thoughts/2026-01-14-did-pfn-find-causal-graph-implicitly.md) · 요약 이전 |
| 2026-01-10 | [[CausalPFN] Amortized Causal Effect Estimation via In-Context Learning](https://letter-night.tistory.com/1189) | Causality/paper | [2025-causalpfn.md](../topics/causality/papers/2025-causalpfn.md) · 논문 노트 (스텁) |
| 2026-01-06 | [복잡한 DAG-structure로 in-context learning 하면..?](https://letter-night.tistory.com/1177) | Causality/thought | [2026-01-06-complex-dag-in-context-learning.md](../topics/causality/thoughts/2026-01-06-complex-dag-in-context-learning.md) · 요약 이전 |
| 2025-12-25 | [[DAG-GFlowNet] Bayesian Structure Learning with Generative Flow Networks](https://letter-night.tistory.com/1154) | Causality/paper | [2022-dag-gflownet.md](../topics/causality/papers/2022-dag-gflownet.md) · 논문 노트 (스텁) |
| 2025-12-24 | [A Meta-Transfer Objective for Learning to Disentangle Causal Mechanisms](https://letter-night.tistory.com/1153) | Causality/paper | [2020-meta-transfer-objective.md](../topics/causality/papers/2020-meta-transfer-objective.md) · 논문 노트 (스텁) |
| 2025-12-22 | [여전히 풀리지 않은 숙제](https://letter-night.tistory.com/1151) | Causality/thought | [2025-12-22-still-unsolved-homework.md](../topics/causality/thoughts/2025-12-22-still-unsolved-homework.md) · 요약 이전 |
| 2025-12-22 | [[DiBS] Differentiable Bayesian Structure Learning](https://letter-night.tistory.com/1150) | Causality/paper | [2021-dibs.md](../topics/causality/papers/2021-dibs.md) · 논문 노트 (스텁) |
| 2025-12-22 | [[Stochastic BALD] Stochastic Batch Acquisition: A Simple Baseline for Deep Active Learning](https://letter-night.tistory.com/1148) | Causality/paper | [2023-stochastic-bald.md](../topics/causality/papers/2023-stochastic-bald.md) · 논문 노트 (스텁) |
| 2025-12-21 | [[BatchBALD] Efficient and Diverse Batch Acquisition for Deep Bayesian Active Learning](https://letter-night.tistory.com/1147) | Causality/paper | [2019-batchbald.md](../topics/causality/papers/2019-batchbald.md) · 논문 노트 (스텁) |
| 2025-12-21 | [[BALD] Bayesian Active Learning](https://letter-night.tistory.com/1146) | Causality/paper | [2011-bald.md](../topics/causality/papers/2011-bald.md) · 논문 노트 (스텁) |
| 2025-12-21 | [[CBED] Interventions, Where and How? Experimental Design for Causal Models at Scale](https://letter-night.tistory.com/1145) | Causality/paper | [2022-cbed-interventions-where-and-how.md](../topics/causality/papers/2022-cbed-interventions-where-and-how.md) · 논문 노트 (스텁) |
| 2025-12-18 | [Causal normalizing flows](https://letter-night.tistory.com/1144) | Causality/paper | [2023-causal-normalizing-flows.md](../topics/causality/papers/2023-causal-normalizing-flows.md) · 논문 노트 (스텁) |
| 2025-12-16 | [[iSCAN] Identifying Causal Mechanism Shifts among Nonlinear Additive Noise Models](https://letter-night.tistory.com/1143) | Causality/paper | [2023-iscan.md](../topics/causality/papers/2023-iscan.md) · 논문 노트 (스텁) |
| 2025-10-29 | [[Do-PFN] In-Context Learning for Causal Effect Estimation](https://letter-night.tistory.com/1079) | Causality/paper | [2025-do-pfn.md](../topics/causality/papers/2025-do-pfn.md) · 논문 노트 |
| 2025-10-29 | [예상대로 흥미진진한데](https://letter-night.tistory.com/1078) | Causality/thought | [2025-do-pfn.md](../topics/causality/papers/2025-do-pfn.md) · 리뷰 병합 |
| 2025-10-28 | [[TabPFN v2] Accurate predictions on small data with a tabular foundation model](https://letter-night.tistory.com/1077) | Causality/paper | [2025-tabpfn-v2.md](../topics/causality/papers/2025-tabpfn-v2.md) · 논문 노트 (스텁) |
| 2025-10-28 | [TabPFN: A transformer that solves small tabular classification problems in a second](https://letter-night.tistory.com/1075) | Causality/paper | [2023-tabpfn.md](../topics/causality/papers/2023-tabpfn.md) · 논문 노트 |
| 2025-10-28 | [이건 좀 별개인데](https://letter-night.tistory.com/1074) | Causality/thought | [2023-tabpfn.md](../topics/causality/papers/2023-tabpfn.md) · 리뷰 병합 |
| 2025-10-28 | [눈이 확 트이네](https://letter-night.tistory.com/1073) | Causality/thought | [2023-tabpfn.md](../topics/causality/papers/2023-tabpfn.md) · 리뷰 병합 |
| 2025-07-24 | [(2/2) Causal Representation Learning](https://letter-night.tistory.com/933) | Causality/paper | [causal-representation-learning.md](../topics/causality/papers/causal-representation-learning.md) · 논문 노트 (스텁) |
| 2025-07-24 | [(1/2) Causal Representation Learning](https://letter-night.tistory.com/932) | Causality/paper | [causal-representation-learning.md](../topics/causality/papers/causal-representation-learning.md) · 논문 노트 (스텁) |
| 2025-07-23 | [Causal Discovery Methods Based on Graphical Models](https://letter-night.tistory.com/931) | Causality/paper | [2019-causal-discovery-graphical-models.md](../topics/causality/papers/2019-causal-discovery-graphical-models.md) · 논문 노트 (스텁) |
| 2025-06-21 | [On-going thought(!)](https://letter-night.tistory.com/887) | Causality/thought | [2025-06-21-robust-agents-need-causal-models.md](../topics/causality/thoughts/2025-06-21-robust-agents-need-causal-models.md) · 요약 이전 |
| 2025-06-21 | [Robust Agents Learn Causal World Models](https://letter-night.tistory.com/884) | Causality/paper | [2024-robust-agents-causal-world-models.md](../topics/causality/papers/2024-robust-agents-causal-world-models.md) · 논문 노트 |
| 2025-06-15 | [Large language model validity via enhanced conformal prediction methods](https://letter-night.tistory.com/876) | Causality/paper | [2024-llm-validity-enhanced-conformal.md](../topics/causality/papers/2024-llm-validity-enhanced-conformal.md) · 논문 노트 (스텁) |
| 2025-06-14 | [Conformal Prediction & Distribution-Free Uncertainty Quantification](https://letter-night.tistory.com/874) | Causality/paper | [2021-conformal-prediction-gentle-intro.md](../topics/causality/papers/2021-conformal-prediction-gentle-intro.md) · 논문 노트 (스텁) |
