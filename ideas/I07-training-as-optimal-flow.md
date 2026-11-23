---
type: idea
id: I07
title: "학습 과정을 optimal flow로: 효율적인 generative model 학습"
topics: [generative-models]
status: seed
proposed_by: me
origin: [1433, 1444, 1485]
date: 2026-08-04
updated: 2026-11-23
---

# I07. 학습 과정을 optimal flow로: 효율적인 generative model 학습

**출발점이 된 기록**
- [[thought] generative model의 training efficiency에 대해서](../topics/generative-models/thoughts/2026-08-15-training-efficiency-as-optimal-flow.md)
- [[thought 2] generative model의 training efficiency에 대해서](../topics/generative-models/thoughts/2026-08-15-training-efficiency-as-optimal-flow.md)
- [Wasserstein gradient flow](../topics/generative-models/concepts/wasserstein-gradient-flow.md)

## 질문
parameter update의 누적을 분포의 flow로 보면, **어떤 training algorithm이 $p_\theta$를 $p_{\text{data}}$로 optimal transport 경로를 따라 옮기는가?** 그렇게 만들면 학습이 효율적이 되는가?

## 연결
- Wasserstein gradient flow, natural gradient / information geometry 관점과 비교해 볼 것.

## 다음 한 걸음
- "parameter space gradient flow vs Wasserstein gradient flow" 관련 문헌 조사 (Research 에이전트)

## 에이전트 노트
- **[2026-11-23 · Management]** 기존 블로그 기록에서 추출해 아이디어로 정리했습니다. 문장은 연구자의 글에서 가져왔고, "접근 방법 후보"와 "다음 한 걸음"의 일부는 에이전트가 정리한 것입니다.
