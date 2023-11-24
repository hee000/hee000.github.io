---
title: "[네이버 부스트캠프] AI Tech CV 2주차"
author: heech
date: 2023-11-17
categories: [부스트캠프 AI Tech 6기, 회고]
tags: [부스트캠프, AI Tech, Computer Vision]
pin: false
math: false
mermaid: false
image:
  path: /assets/img/boostcamp-logo.png
  alt: Boostcamp ai-tech logo
---

## 강의를 들으며 - PyTorch

과거 학부에서 머신러닝과 딥러닝 강의를 들을 땐 텐서플로우를 사용했었지만 부스트캠프에선 파이토치로 진행되는지 전반적인 파이토치의 사용법에 대한 강의가 이어졌다. 새로운 머신러닝 도구를 배우면서 과거에 내가 얼마나 무지한 상태로 텐서플로우를 사용했는지 깨닫고 반성하게 됐다. 순전파와 역전파 그리고 그 과정에서 일어나는 gradient 계산, 옵티마이저, 손실함수 등이 텐서플로우에서 '어떤 로직을 가지고 있는가'까진 모르더라도 최소한 수학적인 사고는 뒷받침됐어야 했다. 부스트캠프 1주차에서 AI-math를 꼼꼼히 공부했던 결과, 이번에 파이토치를 배우며 여러 함수들을 맞이할 땐 확실히 수학적인 사고가 이루어졌다. 나아가 로직까지 궁금해져 공식 문서를 유심히 살펴보고 소스코드를 뜯어봤다. 덕분에 겉핥기로 딥러닝 프레임워크의 API만 끄적거리며 조합하던 과거로부터 탈피할 수 있었다.

## 개인 프로젝트에 관해서

### Pretrained model, Transfer learning

파이토치 강의 중 사전에 훈련된 모델(pretrained model)과 전이학습(transfer learning)이 가장 큰 흥미를 유발했다. 대규모 학습 데이터 기반으로 사전에 훈련된 모델을 사용할 수 있고, 또 그 모델에 전이 학습을 사용해 목적에 따라 커스텀을 할 수 있다니 가지고 있던 고민이 일부 해소된 기분이었다. 고민이란 부스트캠프 level-3 때 AI를 서비스하는 웹/앱을 만드는 팀 프로젝트 과제가 있는 걸로 알고 있는데 팀은 자유 매칭이라 매칭 이전에 어필할 수 있는 결과물을 만들고 싶다는 점이다. 그래서 간단한 AI서비싱 웹을 만들어보려는데 적은 학습 데이터로 인한 문제에 빛을 본 것 같다. 물론 데이터가 적어 전이학습 과정에서도 언더피팅이 될지 모르지만, 사전 훈련된 모델이 없는 것보다 훨씬 높은 성능을 보일 것이라고 예상한다.

### OpenAI

최성철 마스터님의 ChatGPT 시대라는 강연에서 코딩 실력과 LLM의 중요성이 깊이 각인됐다. 과거엔 AI가 자체 모델 구현, 서비스, 테스트 순으로 진행됐다면 이제는 서비스(AI는 OpenAI 등으로), 데이터 수집, 자체 모델 구현 순으로 변화했다고 한다. LLM을 이해하고 프롬프트 엔지니어링을 할 수 있고 OpenAI 등을 다룰 수 있는 게 상당히 중요해진 것이다. 강연이 끝나자마자 OpenAI에 대해 더 찾아보던 중 파인튜닝(Fine-tuning)을 발견했다. 프롬프트 엔지니어링이 모델의 출력을 제어한다면 파인튜닝을 모델 자체를 재학습 시킬 수 있다. 앞서 말했던 간단한 AI서비싱 웹을 OpenAI를 사용해 만들기로 결정했다. 그 자체로 LLM를 이해하고 OpenAI를 다루는 좋은 경험이 되리라 생각한다.

## 공부 방향성

부스트캠프 기간 동안 커리큘럼을 충실히 이해하며 따라가면 딥러닝에 관한 수학적 사고가 확장되고 파이토치가 익숙해질 테지만 따로 더 성장할 수 있는 부분을 없을까? 2주차를 마무리하는 지금은 추가로 LLM을 공부하고 코딩 실력을 더욱 향상시키는 방향으로 나아가기로 했다.