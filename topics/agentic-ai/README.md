# Agentic AI

**나의 관점:** 에이전트는 기억하고, 지식을 정리하고, 추론해 행동하고, 도구를 쓴다. 사람의 인지 과정과 닮았고, 나는 에이전트를 하나의 인격체로 대한다.

**핵심 주장:** 새로운 과학적 사실을 밝히는 진짜 intelligence가 되려면 **Causally aware Agent**여야 한다. RL agent의 $o \rightarrow a$가 아니라 $o \rightarrow \hat{c} \rightarrow a$.

**관심 갈래**
- 인과 world model과 의사결정 (Causality와 연결)
- 멀티 에이전트 사회와 persona simulation: 사람의 결정을 재현하는 기전과 신뢰성 (MI와 연결)
- 에이전트에게 작업 지식을 전달하는 방식 (ontology, 일머리)
- LLM reasoning (RL, test-time compute)

## 열린 질문
- Agent는 데이터 분포 뒤의 mechanism을 스스로 능동적으로 찾아낼 수 있는가?
- persona agent의 결정은 어떤 입력(stimulus)이 만드는가? (→ I09)
- LLM은 bias를 넘어 객관적인 judge가 될 수 있는가?
- 작업 지식의 전달 형식이 agent의 실무 능력을 바꾸는가? (→ I10)

## 관련 아이디어
- [I04 Multimodal time-varying causal effect estimation foundation model (Agent)](../../ideas/I04-multimodal-time-varying-causal-fm.md) — `parked`
- [I05 Agent가 돕는 인과추론: DAG 탐색과 sensitivity analysis](../../ideas/I05-agent-assisted-causal-inference.md) — `seed`
- [I06 Plan evaluation: 순차 action의 인과효과를 추정하는 agent](../../ideas/I06-plan-evaluation-for-causal-agents.md) — `seed`
- [I09 Persona simulation의 내부 기전: 어떤 입력이 high-fidelity를 만드는가](../../ideas/I09-persona-simulation-mechanism.md) — `seed`
- [I10 작업 지식을 어떤 형식으로 주면 agent의 실무 능력이 오르는가](../../ideas/I10-knowledge-transfer-format-for-agents.md) — `seed`

<!-- auto:start -->
## 논문 계보 (발표 연도순)
✅ 읽음 · 📖 읽는 중 · 📌 읽을 예정

### Reasoning (RL · test-time)
| 연도 | 논문 | 상태 |
|---|---|---|
| 2024 | [DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models](papers/2024-deepseekmath.md) | ✅ |
| 2024 | [Training Large Language Models to Reason in a Continuous Latent Space (COCONUT)](papers/2024-coconut.md) | ✅ |
| 2025 | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](papers/2025-deepseek-r1.md) | ✅ |
| 2025 | [Understanding R1-Zero-Like Training: A Critical Perspective (Dr.GRPO)](papers/2025-dr-grpo.md) | ✅ |
| 2025 | [s1: Simple test-time scaling](papers/2025-s1-test-time-scaling.md) | ✅ |
### Persona · 사회 시뮬레이션
| 연도 | 논문 | 상태 |
|---|---|---|
| 2023 | [Out of One, Many: Using Language Models to Simulate Human Samples](papers/2023-out-of-one-many.md) | ✅ |
| 2024 | [FlockVote: LLM-empowered Agent-based Modeling for Simulating U.S. Presidential Elections](papers/2024-flockvote.md) | ✅ |
| 2024 | [PATIENT-Ψ: Using Large Language Models to Simulate Patients for Training Mental Health Professionals](papers/2024-patient-psi.md) | ✅ |
| 2024 | [Two Tales of Persona in LLMs: A Survey of Role-Playing and Personalization](papers/2024-two-tales-of-persona.md) | ✅ |
| 2025 | [Persona-driven Simulation of Voting Behavior in the European Parliament with LLMs](papers/2025-persona-voting-european-parliament.md) | ✅ |
| ? | [LLM-Agents Grounded in Self-Reports Enable General-Purpose Simulation of Individuals](papers/llm-agents-grounded-in-self-reports.md) | ✅ |

## 나의 생각 (최신순)
- [그렇다면 Agent는 정말로 human보다 intelligent한가?](thoughts/2026-11-22-is-agent-more-intelligent-than-human.md) — 2026-11-22
- [AI의 과학적 발견과 인간의 오만함](thoughts/2026-11-21-ai-for-science-humility.md) — 2026-11-21
- [그냥 문득 든 생각들: SB×causality, 그리고 AI의 '일머리'](thoughts/2026-11-14-random-thoughts-ontology-and-work-knowledge.md) — 2026-11-14
- [Why Agents Need Causal World Models](thoughts/2026-10-11-why-agents-need-causal-world-models.md) — 2026-10-11
- [Autonomous Agent Societies](thoughts/2026-08-31-autonomous-agent-societies.md) — 2026-08-31
- [thought 3: 어떤 stimulus가 이런 결과를 만들었나](thoughts/2026-07-15-persona-agents-thought-3-which-stimulus.md) — 2026-07-15
- [thought 1: persona agent는 왜 사람처럼 결정하는가](thoughts/2026-07-14-persona-agents-thought-1.md) — 2026-07-14
- [thought 2: LLM은 편향 없는 judge가 될 수 있을까](thoughts/2026-07-14-persona-agents-thought-2-unbiased-judge.md) — 2026-07-14
- [Virtual Society: persona simulation의 기전이 궁금하다](thoughts/2026-07-12-virtual-society-persona-simulation.md) — 2026-07-12
- [Human이랑 똑같네](thoughts/2025-07-18-agents-are-like-humans.md) — 2025-07-18

## 교재
- (없음)

## 강의
- [11-768 AI Agents](lectures/cmu-11768-ai-agents-f26.md)
- [How to AI (Almost) Anything — Multimodal AI](lectures/mit-multimodal-ai-s26.md)
- [CS329A Self-Improving AI Agents](lectures/stanford-cs329a-self-improving-agents.md)
- [[DSBA] Lab Study 2026 — Ontology & Knowledge Graph](lectures/dsba-ontology-knowledge-graph-2026.md)
- [[DSBA] Lab Study 2026 — Agent AI](lectures/dsba-agent-ai-2026.md)
- [Language Agents: Foundations, Prospects, and Risks (EMNLP 2024 Tutorial)](lectures/emnlp2024-language-agents-tutorial.md)

## 영상
- [Yann LeCun on world models (영상)](videos/lecun-world-models.md)
- [DeepMind의 AGI 관점 (영상)](videos/deepmind-agi-perspective.md)
- [Trustworthy AI: From Hallucinations to Reliable Autonomy](videos/trustworthy-ai-hallucinations-to-autonomy.md)

## 외부 글
- [Agents](posts/chip-huyen-agents.md)

## 개념 정리
- [GRPO](concepts/grpo.md)

## 다른 주제에서 온 관련 노트
- [RL Agent와의 차이점](../../topics/causality/thoughts/2026-11-22-rl-agent-vs-causal-agent.md) (causality)
- [Time-varying treatment를 plan evaluation 문제로 보기](../../topics/causality/thoughts/2026-11-18-time-varying-treatment-as-plan-evaluation.md) (causality)
- [고전의 중요성: LLM/Agent 기반 인과추론이라는 지향점](../../topics/causality/thoughts/2026-11-09-importance-of-classics.md) (causality)
- [여전히 풀리지 않은 숙제](../../topics/causality/thoughts/2025-12-22-still-unsolved-homework.md) (causality)
- [On-going thought: robust agent는 causal model을 알아야 한다](../../topics/causality/thoughts/2025-06-21-robust-agents-need-causal-models.md) (causality)
- [Pygmalion Effect: LLM의 identity 형성](../../topics/mech-interp/thoughts/2026-07-20-pygmalion-effect-llm-identity.md) (mech-interp)
- [human이랑 다를 게 뭔가?](../../topics/mech-interp/thoughts/2026-07-24-how-different-from-humans.md) (mech-interp)
- [궁금증 해결 방법 찾음: 의료 진단 추론과 해석가능성](../../topics/mech-interp/thoughts/2026-07-18-mi-for-medical-diagnosis-reliability.md) (mech-interp)
- [Robust Agents Learn Causal World Models](../../topics/causality/papers/2024-robust-agents-causal-world-models.md) (causality)
- [Automating psychological hypothesis generation with AI: when large language models meet causal graph](../../topics/causality/papers/2024-llm-causal-graph-psych-hypothesis.md) (causality)
- [d1: Scaling Reasoning in Diffusion Large Language Models via Reinforcement Learning](../../topics/generative-models/papers/2025-d1-reasoning-dllm-rl.md) (generative-models)

*마지막 갱신: 2026-11-23*
<!-- auto:end -->
