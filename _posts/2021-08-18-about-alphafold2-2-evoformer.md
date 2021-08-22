---
layout: distill
title: AlphaFold2 톺아보기 - (2) 개요
description: AlphaFold2에 대한 설명과 단상
date: 2021-08-18

authors:
  - name: Dohoon Lee
    url: "https://dohlee.github.io"
    affiliations:
      name: Seoul National University, South Korea

bibliography: 2018-12-22-distill.bib


---

본 포스트에서는 AlphaFold2의 핵심 아이디어와, 그 아이디어를 딥 러닝 모델에 어떻게 녹여내었는지를 개괄적으로 설명합니다. 딥 러닝 모델의 구현을 비롯한 보다 자세한 내용은 추후 게시될 포스트들에서 다루고자 하며, 여기서는 큰 흐름을 먼저 다루어 전체적인 이해를 돕고자 합니다. 이후 다룰 복잡한 내용들에 매몰되어 막힐 때마다, 다시 모델의 전체적인 그림을 보고 큰 흐름을 잡는 길잡이로서 이 글이 활용되었으면 좋겠습니다. 

## AlphaFold2를 아주 간단히 설명하자면...

개인적으로, AlphaFold2 모델의 **핵심 기술 중 가장 중요한 하나**를 꼽아야 한다면 단연

<center><h3>Attention</h3></center><br/>

이라고 생각합니다. 그 **본질**을 좀 더 길게 한 구절로 설명하자면

<center><h3>Attention</h3></center><br/>



다음 한 문장으로 설명할 수 있다고 생각합니다.

> 아미노산 잔기(residue)들의 공진화(co-evolution), 잔기쌍(residue pair)의 feature 및 두 요소 간의 상호작용을 딥 러닝 모델에 접목시켜 단백질 구조를 예측하기 위해서 self-attention과 이를 변형한 연산들을 훌륭하게 디자인 및 구현하여 활용한 모델.



<div class="l-page">
  <img src="/assets/img/alphafold2-overview-1.png" width="100%" />
  <div class="caption" >
    AlphaFold2 모델 개요.
  </div>
</div>

## AlphaFold2를 구성하는 4가지 요소.

AlphaFold2는 크게 (1) 입력 임베딩(Input embedding), (2) Evoformer block, (3) 구조 모듈(Structure module), 그리고 (4) 재활용(Recycling)의 4가지 요소로 구성됩니다. 여기서는 각 요소를 어떤 이유에서 모델에 사용하였는지, 그 동기를 생각해보고 각각을 간단히 설명하고자 합니다.

### 1. 입력 임베딩(Input embedding).

#### 왜 사용하는가?

아미노산 서열 데이터베이스와 이미 알려진 단백질 구조 정보 데이터베이스의 도움을 받아서, 입력 아미노산 서열에 대한 적절한 입력 임베딩 혹은 입력 표현(input representation) 들을 구성합니다. 

#### 개요.



### 2. Evoformer blocks.

#### 왜 사용하는가?

Evoformer block은 AlphaFold2에서 제안된 특별한 딥 러닝 연산 모듈로서, 이름에서 암시하는 바와 같이 진화적인 관계(Evolution)과 최근 각광받고 있는 딥러닝 연산 모듈인 트랜스포머(Transformer)

#### 개요.



### 3. 구조 모듈(Structure module).

#### 왜 사용하는가?



#### 개요.



### 4. 재활용(Recycling).

#### 왜 사용하는가?



#### 개요.
