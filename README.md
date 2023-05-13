# 통계데이터 인공지능 활용대회
## 1. 개요
https://data.kostat.go.kr/sbchome/contents/cntPage.do?cntntsId=CNTS_000000000000575&curMenuNo=OPT_09_03_00_0
  - 주제 : 자연어 기반 인공지능 산업분류 자동화
  - Task : Text Classification
  - 기간 : 2022.3.14 ~ 2022.04.13
  - 결과 : 6등 / 395 => 수상
<!--  Other options to write Readme
  - [Deployment](#deployment)
  - [Used or Referenced Projects](Used-or-Referenced-Projects)
-->
## 2. 데이터셋 설명
<!--Wirte one paragraph of project description -->  
- train.csv : 학습 데이터셋은 뉴스 기사 Text와 label 제공 (47399개)
  - id : 샘플 고유 id
  - text : 뉴스 기사 전문
  - label : 카테고리


- test.csv : 테스터 데이터셋은 뉴스 기사 Text만 제 (83344개)
  - id : 샘플 고유 id
  - text : 뉴스 기사 전문

## 3. 수행방법
<!-- Write Overview about this project -->
- 본 과제는 ChatGPT가 제공하는 코드로만 AI 코드를 작성하여 생성된 모델의 추론 결과를 제출
- ChatGPT가 코드를 잘짜도록 질문을 잘하는 것이 중요. (간결하고, 핵심적인 내용을 잘 전달하는 것이 중요)
- pytorch를 사용하고, Pretrained-Roberta-Large 모델을 사용하도록 지시
- 데이터 불균형 문제가 있으므로 Focal-Loss를 사용하도록 지시
- 최종적으로 F1-score 0.63423 달성

## 4. 한계점
<!-- Write Overview about this project -->
- ChatGPT로만 코드를 짜야하기에 하이퍼파라미터 조정이 어렸웠음
- back translation과 같은 augmentation 기법을 쓰도록 지시했지만, 어려운 지시는 코드로 잘 짜지 못함

## Team member
장종환 (개인 참가)
