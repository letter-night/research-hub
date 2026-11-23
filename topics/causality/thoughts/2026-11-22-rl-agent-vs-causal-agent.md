---
type: thought
title: "RL Agent와의 차이점"
topics: [causality, agentic-ai]
tags: [agent, causal-world-model, exploration]
date: 2026-11-22
source_post: https://letter-night.tistory.com/1520
migration: summary
migrated: 2026-11-23
---

# RL Agent와의 차이점

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [[thought] RL Agent 와의 차이점](https://letter-night.tistory.com/1520) (2026-11-22)

## 나의 생각
- RL 에이전트는 보상을 최대화하도록 수천에서 수만 번 학습을 반복하면 결국 과제는 잘 수행하게 된다.
- 하지만 이것은 과제의 기저 메커니즘, 즉 "how things work, how things go"를 알고 추론한 행동이 아니다.
- 환경이 바뀌면 새 환경에 맞는 최적 행동을 다시 무수한 시행착오로 배워야 한다.
- 인과추론 능력을 갖춘 에이전트는 **다른 차원**이다. 시행착오로 정보를 노가다식으로 모을 필요도 없고, 그 과정의 training instability를 걱정할 필요도 없다.

$$
\text{RL Agent: } o \rightarrow a
\qquad\qquad
\text{인과추론 Agent: } o \rightarrow \hat{c} \rightarrow a
$$

  $o$: observation, $\hat{c}$: 추론된 인과관계(inferred causality), $a$: action.
  "내가 이렇게 행동하면 이렇게 되겠구나"라는 추론을 거쳐 행동을 고른다.
- 인과관계를 추론할 수 있으므로 새로운 환경에서도 추론이 가능하다.
- 탐색도 RL처럼 무작위 확률에 기대지 않고, **자신의 추론을 보강하는 데 필요한 정보를 모으는 능동적 탐색**을 한다.

## 질문
- $\hat{c}$를 어떻게 학습시키고, 틀렸을 때 어떻게 고치는가? (→ Bayesian structure learning, active learning 글들과 연결)

## 연결된 자료

- [time-varying treatments with time-varying confounders](2026-11-18-time-varying-treatment-as-plan-evaluation.md)
- memo — https://letter-night.tistory.com/1513
- [[thought] 그렇다면 Agent는 정말로 human보다 intelligent한가?](../../agentic-ai/thoughts/2026-11-22-is-agent-more-intelligent-than-human.md)

## 에이전트 노트
