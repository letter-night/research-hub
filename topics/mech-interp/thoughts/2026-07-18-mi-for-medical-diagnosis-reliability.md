---
type: thought
title: "궁금증 해결 방법 찾음: 의료 진단 추론과 해석가능성"
topics: [mech-interp, agentic-ai]
tags: [medical, reliability, prompt-sensitivity, cot-faithfulness]
date: 2026-07-18
source_post: https://letter-night.tistory.com/1412
migration: summary
migrated: 2026-11-23
---

# 궁금증 해결 방법 찾음: 의료 진단 추론과 해석가능성

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [★ 궁금증 해결 방법 찾음 ★ Similar approach (but other domain)](https://letter-night.tistory.com/1412) (2026-07-18)

## 나의 생각
- 사회과학에서 LLM으로 피험자를 simulate할 때 신뢰성의 조건은 다양한 실험 결과를 재현하는 것이고, 이를 위해 **interpretability가 중요**하다.
- 의료 분야에서도 모델 추론의 해석가능성과, 우리가 깨닫지 못한 한계를 밝히는 연구가 필요하다.
  - 의료 적용에서도 사회과학처럼 prompt sensitivity 문제가 나타난다.
  - CoT로 추론 과정을 살피려는 시도가 있지만, **CoT는 모델의 실제 내부 추론 과정과 일치하지 않는다.**
- *On the Biology of a LLM*의 Medical Diagnoses 사례: 임신, 혈압 같은 환자 상태 feature가 자간전증(preeclampsia) feature를 활성화하고, 이 feature를 억제하면 응답이 다른 질환 쪽으로 바뀐다 → 인과적 역할 확인.
- 의료 LLM 성능 연구는 결과가 엇갈린다 (전문가보다 높다는 보고 vs 구조화된 데이터에서 성능 저하, 버전 간 변동).
- 질문: 사회과학 simulation에서 본 sensitivity, reliability(stability) 문제가 의료에서도 비슷하게 논의된다. **해석가능성 연구는 이런 문제를 어디까지 드러낼 수 있을까?**

## 질문
-

## 연결된 자료
- On the Biology of a LLM, Medical Diagnoses: https://transformer-circuits.pub/2025/attribution-graphs/biology.html
- Accuracy of a generative AI model in a complex diagnostic challenge (2023)
- Chatbot vs medical student performance on free-response clinical reasoning examinations (2023)
- Large language model influence on diagnostic reasoning: a randomized clinical trial (2024)
- Towards accurate differential diagnosis with large language models (2023)
- [thought 1](../../agentic-ai/thoughts/2026-07-14-persona-agents-thought-1.md)
- [thought 3](../../agentic-ai/thoughts/2026-07-15-persona-agents-thought-3-which-stimulus.md)

## 에이전트 노트
