---
layout: distill
title: AlphaFold2 톺아보기 - (1) 들어가며
description: AlphaFold2에 대한 설명과 단상
date: 2021-08-18

authors:
  - name: Dohoon Lee
    url: "https://dohlee.github.io"
    affiliations:
      name: Bio & Health Informatics Lab, Seoul National University, South Korea
      url: "https://bhi-kimlab.github.io"

bibliography: 2018-12-22-distill.bib

---

## 들어가며

Structure-function relationship. 아미노산 서열로부터 단백질 구조 결정 어려운 문제. 

구글 딥마인드가 개발한 AlphaFold2는 2020년 말 CASP14로 불리는 단백질 구조 예측 경연에서 압도적인 차이로 우승하여 세상을 놀라게 한 모델입니다.
본 포스트에서는 AlphaFold2 모델의 구조와 그 구성 원리를 자세히 설명하고자 합니다.
생물정보학과 인공지능 두 분야에 관한 기본적인 지식이 필요하지만, 관련 분야 전공자가 아니더라도 이해할 수 있을 정도로 최대한 쉽게 풀어쓰고자 노력해 보겠습니다.

<div class="l-gutter">
  <img src="/assets/img/alphafold2-intro-1.gif" width="250%" />
  <div class="caption" style="width:250%" >
      실험적으로 결정된 단백질의 구조(초록)와 AlphaFold2가 예측한 단백질의 구조(파랑).
  </div>
</div>

## 요약

아미노산 residue들의 co-evolution, residue pair의 feature 및 두 요소 간의 상호작용을 deep learning 모델에 접목시켜 protein structure를 예측하기 위해서 self-attention과 그 variant들을 훌륭하게 design하여 활용함

