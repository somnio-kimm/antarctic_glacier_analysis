# time_series_analysis

[ESTsoft AI 모델 개발자 부트캠프 8기 두번째 진행 프로젝트]
프로젝트 목표 : 과거 남극 빙하 이미지 시계열 데이터 학습을 통해 미래 빙하 분포 예측 모델 개발
프로젝트 기간 : 2025.04.28 ~ 2025.05.16
프로젝트 인원 : 4명 (최환규, 김수민, 박준호, 김시환)
프로젝트 키워드 : 시계열데이터, CNN, LSTM, AutoEncoder

프로젝트 내용 :
(데이터 전처리)
National Snow and Ice Data Center (NSIDC)에서 배포한 1978.11~2025.04(558개) 월간 남극 빙하 면적 자료를 이용하여 GrayScale 변환 및 256*256 리사이징

(데이터 시각화)
수집한 데이터를 통해 describe, Extend 분포, 빙하 면적 이동평균, 시계열 분해 등 EDA

(모델학습)
ConvLSTM2D 기반 생성기(Generator) 모델학습 진행

(웹)
생성된 미래 2년치 이미지를 통해 사용자가 날짜를 입력하면 해당 날짜에 맞는 빙하이미지를 출력해주는 간단한 웹페이지 구현
Backend : Flask / Frontend : HTML,Bootstrap
