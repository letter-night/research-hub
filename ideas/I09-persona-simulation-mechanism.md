---
type: idea
id: I09
title: "Persona simulation의 내부 기전: 어떤 입력이 high-fidelity를 만드는가"
topics: [agentic-ai, mech-interp]
status: seed
proposed_by: me
origin: [1403, 1404, 1408, 1405, 1412]
date: 2026-07-12
updated: 2026-11-23
---

# I09. Persona simulation의 내부 기전: 어떤 입력이 high-fidelity를 만드는가

**출발점이 된 기록**
- [Virtual Society](../topics/agentic-ai/thoughts/2026-07-12-virtual-society-persona-simulation.md)
- [thought 1](../topics/agentic-ai/thoughts/2026-07-14-persona-agents-thought-1.md)
- [thought 3](../topics/agentic-ai/thoughts/2026-07-15-persona-agents-thought-3-which-stimulus.md)
- [thought 2](../topics/agentic-ai/thoughts/2026-07-14-persona-agents-thought-2-unbiased-judge.md)
- [★ 궁금증 해결 방법 찾음 ★ Similar approach (but other domain)](../topics/mech-interp/thoughts/2026-07-18-mi-for-medical-diagnosis-reliability.md)

## 질문
LLM agent가 persona/self-report를 받아 사람의 결정을 재현할 때, **모델 내부에서 인구통계 변수와 그 상호작용이 어떻게 표현되고 쓰이는가?** 어떤 stimulus가 결과를 만드는가?

## 왜 중요한가
- 원리를 알면 high fidelity를 보장하는 입력을 설계할 수 있고, agent 시뮬레이션 기반 연구가 정당성을 얻는다.
- 같은 문제(prompt sensitivity, 신뢰성)가 의료 LLM에서도 나타난다.

## 접근 방법 후보
- persona 속성별 feature 찾기 → 속성 feature에 개입했을 때 응답 분포 변화
- self-report 요약본 vs 전체 스크립트의 내부 표현 비교

## 실행 가능성
- 사회과학 쪽은 journal 투고 경로도 있음 (시뮬레이션의 조사 예측 재현성, 결측치 대체)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
