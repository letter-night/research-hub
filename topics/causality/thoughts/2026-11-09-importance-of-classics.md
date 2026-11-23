---
type: thought
title: "고전의 중요성: LLM/Agent 기반 인과추론이라는 지향점"
topics: [causality, agentic-ai, mech-interp]
tags: [agent-for-causal-inference, dag-discovery, sensitivity-analysis, multimodal]
date: 2026-11-09
source_post: https://letter-night.tistory.com/1511
migration: summary
migrated: 2026-11-23
---

# 고전의 중요성: LLM/Agent 기반 인과추론이라는 지향점

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [★ 고전의 중요성 ★](https://letter-night.tistory.com/1511) (2026-11-09)

## 나의 생각
- *What If*는 계속 업데이트되고 있어 엄밀한 의미의 고전은 아니지만, 인과추론 논문에서 거의 항상 인용되고 기초부터 치밀하게 다루는 **classic**한 참고서다.
- 이 책을 보며 **연구 지향점이 매우 분명해졌다**: LLM/Agent 기반 인과추론.
- 인과추론은 기법을 바로 적용하기 전에 데이터를 만들어낸 data generating mechanism을 추론하는 데서 출발해야 한다. 인간의 지식은 항상 옳지 않으므로, Agent가 **DAG 구조의 타당성**을 높이는 데 도움을 줄 수 있다.
- 모든 인과분석에는 DAG와 **sensitivity analysis**가 반드시 함께 제시되어야 한다. Agent가 여러 가설과 시나리오를 검토해 추정이 틀렸을 때의 bias 정도를 정량화할 수 있다.
- 전통적 기법도 linear functional form 같은 가정에 의존한다. Agent 기반 접근이 덜 엄밀해 보여도 본질적 한계는 같다. 고차원 데이터에 ML이 필수가 되었듯, 인과추론에서도 Agent가 핵심 요소가 될 것이다.
- Agent가 할 수 있는 것
  1. DAG structure discovery
  2. Sensitivity analysis (uncertainty quantification)
  3. Multimodality(image, text, table)를 활용한 추론
- 내 관심은 양방향이다.
  - (→) Agent의 추론 능력으로 **인과추론 자체를 개선**
  - (←) Agent의 인과추론 능력을 **보이거나**(mechanistic interpretability 등), 인과추론 능력을 **심어서** 더 나은 연구자형 Agent를 만드는 것
- 참고 사례: John Snow의 콜레라 원인 규명

## 질문
-

## 연결된 자료

- [causal inference 를 공부하며 3탄](2026-11-08-studying-causal-inference-3.md)
- [★ 고전의 중요성 2탄 ★](2026-11-11-importance-of-classics-2.md)

## 에이전트 노트
