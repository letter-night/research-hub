---
type: thought
title: "thought 1: persona agent는 왜 사람처럼 결정하는가"
topics: [agentic-ai, mech-interp]
tags: [persona-simulation, mech-interp, steering]
date: 2026-07-14
source_post: https://letter-night.tistory.com/1404
migration: summary
migrated: 2026-11-23
---

# thought 1: persona agent는 왜 사람처럼 결정하는가

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [thought 1](https://letter-night.tistory.com/1404) (2026-07-14)

## 나의 생각
- LLM Agent에 특정 집단이나 개인의 profile을 부여해 persona를 갖게 하고, 실제 human의 의사결정·행동을 얼마나 잘 재현하는지 시뮬레이션한 사례를 정리했다 (주로 voting behavior, political opinion, survey response).
- 모델은 상당히 잘 추론한다. 예측력은 prompt, attribute 선택, 정보 제시 형식에 따라 달라진다.
- Reasoning step은 어떤 attribute를 근거로 했는지 보여주지만, 모델 내부 기전을 정확히 설명하지는 못한다.
- 질문: LLM 내부에 다양한 인격체를 수용하고 있다고 해야 하나? (prototype, bias)
- 목표
  1. 기존 논문은 실험 결과만 보여주고 원리 설명이 없다 → **Mechanistic Interpretability로 기전을 규명**하고 싶다.
  2. persona agent 간 communication 조정의 단초가 될 수 있다. communication이 항상 성공적이지는 않으므로, 먼저 **agent를 steering하는 요소**를 파악해야 한다.

## 질문
-

## 연결된 자료
- awesome-llm-human-simulation: https://github.com/Persdre/awesome-llm-human-simulation
- PersonaLLM-Survey: https://github.com/MiuLab/PersonaLLM-Survey
- [Virtual Society](2026-07-12-virtual-society-persona-simulation.md)
- [thought 2](2026-07-14-persona-agents-thought-2-unbiased-judge.md)
- [thought 3](2026-07-15-persona-agents-thought-3-which-stimulus.md)

## 에이전트 노트
