---
type: paper
title: "TabPFN: A Transformer That Solves Small Tabular Classification Problems in a Second"
authors: "Hollmann, Müller, Eggensperger, Hutter"
year: 2023
venue: "ICLR 2023"
url: ""
topics: [causality]
tags: [pfn, tabular, foundation-model, synthetic-prior]
status: read
date: 2025-10-28
builds_on: []
my_rating:
source_post: https://letter-night.tistory.com/1075
migration: summary
migrated: 2026-11-23
---

# TabPFN: A Transformer That Solves Small Tabular Classification Problems in a Second

**기존 글**
- [TabPFN: A transformer that solves small tabular classification problems in a second](https://letter-night.tistory.com/1075) (2025-10-28)

## 한 줄 요약

## 핵심 내용

## 나의 리뷰
*(2025-10-28 글 "눈이 확 트이네", "이건 좀 별개인데"에서 옮김)*
- 새로운 지평을 열어주는 연구들이 있다. 이렇게 새롭게 문제를 재정의할 수가 있네!
- 새 기법을 들고 온 게 아니라, 검증된 방법을 적용해 복잡한 문제를 단순하게 해결한 점이 멋지다.
- (이번에 본 설명은) original version보다 훨씬 명확하고 깔끔해서 막연했던 부분이 이해되었다.
- GP prior, BNN prior에 익숙하다가 **SCM prior**를 보고 눈이 번쩍 뜨였다 → **causal inference foundation model이 가능하겠구나.**
- 같은 방식으로 학습하면 에이전트가 counterfactual 질의응답도 할 수 있지 않을까?
- 실험할 때 보통 synthetic data로 먼저 하고 real-world data로 추가 실험하는데, 정작 synthetic data를 어떻게 만들어야 할지는 잘 몰랐다. 이 논문 시리즈가 그 절차를 상세히 알려줘서 고맙다.

## 열린 질문 / 한계

## 연결

## 에이전트 노트
