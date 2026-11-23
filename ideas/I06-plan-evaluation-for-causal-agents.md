---
type: idea
id: I06
title: "Plan evaluation: 순차 action의 인과효과를 추정하는 agent"
topics: [causality, agentic-ai]
status: seed
proposed_by: me
origin: [1517, 1513, 1520, 1521]
date: 2026-11-11
updated: 2026-11-23
---

# I06. Plan evaluation: 순차 action의 인과효과를 추정하는 agent

**출발점이 된 기록**
- [time-varying treatments with time-varying confounders](../topics/causality/thoughts/2026-11-18-time-varying-treatment-as-plan-evaluation.md)
- [memo](../topics/causality/books/pearl-causality.md)
- [[thought] RL Agent 와의 차이점](../topics/causality/thoughts/2026-11-22-rl-agent-vs-causal-agent.md)
- [[thought] 그렇다면 Agent는 정말로 human보다 intelligent한가?](../topics/agentic-ai/thoughts/2026-11-22-is-agent-more-intelligent-than-human.md)

## 질문
Pearl의 plan evaluation(= Robins의 time-varying treatment)을 agent의 의사결정 문제로 보면, agent가 **자신이 추론한 causal diagram으로 plan $do(a_1,\dots,a_T)$의 결과를 예측해 action을 고르고**, 식별이 부분적일 때는 **정보를 얻기 위한 action**을 고를 수 있는가?

## 왜 중요한가
- RL agent: $o \rightarrow a$ (시행착오, 환경이 바뀌면 다시 학습) vs 인과 agent: $o \rightarrow \hat{c} \rightarrow a$
- Robust Agents Learn Causal World Models의 이론적 결과를 실제 agent 설계로 옮기는 다리.

## 접근 방법 후보
- 작은 grid/텍스트 환경에서 환경 메커니즘을 국소적으로 바꾸고 (Pearl의 remodeling flexibility), RL agent와 causal-model agent의 적응 속도 비교
- 능동 탐색: BALD / CBED 식의 정보 이득으로 개입 선택

## 다음 한 걸음
- 이미 이런 비교를 한 연구가 있는지 확인 (causal RL, causal world model 문헌)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
