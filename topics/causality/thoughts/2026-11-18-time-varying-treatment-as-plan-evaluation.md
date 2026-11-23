---
type: thought
title: "Time-varying treatment를 plan evaluation 문제로 보기"
topics: [causality, agentic-ai]
tags: [time-varying-treatment, plan-evaluation, sequential-backdoor, agent]
date: 2026-11-18
source_post: https://letter-night.tistory.com/1517
migration: summary
migrated: 2026-11-23
---

# Time-varying treatment를 plan evaluation 문제로 보기

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [time-varying treatments with time-varying confounders](https://letter-night.tistory.com/1517) (2026-11-18)

## 나의 생각
- "Dynamic treatment with time-varying confounders" 문제는 Robins의 G-computation 대신 Pearl의 **sequential back-door adjustment**로도 접근할 수 있다.
- Robins의 time-varying treatment 문제를 Pearl처럼 **plan evaluation problem**으로 재정의한다.
  - intervention을 action으로 보고, action의 순서열, 즉 plan의 effect를 추정한다: $do(a_1, \dots, a_T)$
- 순차적 action의 인과효과를 추정할 수 있다면, Agent는 경험과 지식으로부터 추론한 causal diagram으로 plan의 결과를 예측하고 optimal action을 고를 수 있다.
- 부분적으로만 식별 가능(partially identifiable)한 상황에서는 **적극적인 action으로 필요한 DAG 구조를 추가로 추론**할 수 있다.
- 따라서 Agent에게 dynamic treatment effect estimation 같은 causal inference 능력이 필요하다는 근거가 된다.

> 원문에는 도식 이미지가 여러 장 있으나 이전하지 않았습니다. 원문을 참고하세요.

## 질문
-

## 연결된 자료

- memo — https://letter-night.tistory.com/1513
- [[thought] RL Agent 와의 차이점](2026-11-22-rl-agent-vs-causal-agent.md)
- [[부치지 못한 편지 2] Causal effect under time-varying treatment](2026-11-05-causal-effect-under-time-varying-treatment.md)

## 에이전트 노트
