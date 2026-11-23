---
type: thought
title: "J-lens와 attribution graph 비교"
topics: [mech-interp]
tags: [j-lens, attribution-graph, methods]
date: 2026-07-20
source_post: https://letter-night.tistory.com/1418
migration: summary
migrated: 2026-11-23
---

# J-lens와 attribution graph 비교

> 기존 블로그 글에서 옮긴 요약입니다. 원문 표현을 최대한 살렸지만 전문은 아닙니다.
- [thought](https://letter-night.tistory.com/1418) (2026-07-20)

## 나의 생각
- J-lens는 attribution graph보다 접근이 쉽지만, feature 간 causal structure를 보여주지 않는다. **생각이 흘러가는 경로**를 보여주지 않는다.
- 예비 단계로 모델이 어떤 생각으로 output을 냈는지 보는 데는 쓸 수 있다.
- 내 궁극적 질문인 **"어떤 추론 과정을 거쳐서 답변을 내놓았는가?"** 에 답하려면 attribution graph가 최선이다.
- 방법 비교 (논문 related work를 내 말로 정리)
  | 방법 | 장점 | 한계 |
  |---|---|---|
  | Linear probe | 저렴 | 지도학습, 상관적 |
  | Sparse dictionary learning | 비지도 | 학습 비용 큼 |
  | Attribution graph | 특정 계산의 회로도 | activation이 무엇을 말하려는지는 안 보여줌 |
  | 자유 텍스트 설명 | 표현력 높음 | 비용 큼, confabulation 위험 |
  | J-lens | 저렴하고 근거 있음 | 출력이 단일 토큰 순위 목록 |

## 질문
-

## 연결된 자료
- Transcoders find interpretable LLM feature circuits (NeurIPS 2024)
- Sparse Feature Circuits (ICLR 2025)
- Circuit Tracing (2025)
- On the Biology of a Large Language Model (2025)
- [Thought on Mechanistic interpretability](2026-07-19-thought-on-mechanistic-interpretability.md)
- A global workspace in language models — https://letter-night.tistory.com/1415

## 에이전트 노트
