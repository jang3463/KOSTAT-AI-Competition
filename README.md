# 통계데이터 인공지능 활용대회
## 1. 개요
https://data.kostat.go.kr/sbchome/contents/cntPage.do?cntntsId=CNTS_000000000000575&curMenuNo=OPT_09_03_00_0
  - 주제 : 자연어 기반 통계 데이터를 활용한 산업분류 자동화 인공지능 모델 개발
  - Task : Text Classification, Multi Label Classification
  - 기간 : 2022.3.14 ~ 2022.04.13
  - 결과 : 6등 / 395 => 수상
<!--  Other options to write Readme
  - [Deployment](#deployment)
  - [Used or Referenced Projects](Used-or-Referenced-Projects)
-->
## 2. 데이터셋 설명
<!--Wirte one paragraph of project description -->  
<img width="650" alt="image" src="https://github.com/jang3463/KOSTAT-AI-Competition/assets/70848146/9b302be6-ee3f-46a7-b902-de6827269b95">  


- train.csv : text_obj, text_mthd, text_deal, 대분류, 중분류, 소분류 (100만개)

- test.csv : text_obj, text_mthd, text_deal (10만개)


## 3. 수행방법
<!-- Write Overview about this project -->
- 본 과제는 전국사업체조사 텍스트 데이터를 가지고 한국표준산업분류(KSIC) 대분류, 중분류, 소분류로 나누는 AI 모델 개발
- Kobert, Roberta-Large 모델을 사용했고, 성능을 최대한 올리기 위해서 앙상블 기법 사용
- 데이터 불균형 문제가 있어서 불균형 해소를 위해 back translation 기법 사용
- 최종적으로 Accuraccy 91.25, F1-Score	81.31 달성  

**자세한 내용은 위의 코드 설명자료.pdf를 참조해 주시기 바랍니다.**

## 4. 한계점
<!-- Write Overview about this project -->
- 데이터 불균형 해소를 위해서 다른 다양한 기법을 좀 더 탐색해볼 필요 있음

## Team member
장종환, 손효은
