---
layout: distill
title: AlphaFold2 톺아보기
description: AlphaFold2에 대한 자세한 설명과 단상
date: 2021-08-19

authors:
  - name: Dohoon Lee
    url: "https://dohlee.github.io"
    affiliations:
      name: Seoul National University, South Korea

bibliography: 2018-12-22-distill.bib

# Below is an example of injecting additional post-specific styles.
# If you use this post as a template, delete this _styles block.
_styles: >
  .fake-img {
    background: #bbb;
    border: 1px solid rgba(0, 0, 0, 0.1);
    box-shadow: 0 0px 4px rgba(0, 0, 0, 0.1);
    margin-bottom: 12px;
  }
  .fake-img p {
    font-family: monospace;
    color: white;
    text-align: left;
    margin: 12px 0;
    text-align: center;
    font-size: 16px;
  }

---

## 들어가며

본 포스트에서는 AlphaFold2 모델의 구조와 그 구성 원리를 자세히 설명하고자 한다.
생물정보학과 인공지능에 관한 기본적인 지식이 필요하지만, 관련 분야 전공자가 아니더라도 이해할 수 있을 정도로 최대한 쉽게 풀어쓰고자 노력해 보겠다.


