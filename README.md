# lecture_6_timeseries_AnomalyDetection
GAN, Tranformer, GRU based Tire-series Anomaly Detection with HAI dataset


### 1_dataset
[HAI dataset](https://dacon.io/competitions/official/235757/data)

## Run model in Colab
### 1. GAN based model colab code
- run Timeseries_Anomaly_Detection_GAN_colab.ipynb at colab
- This GAN is 
  - [code](https://github.com/manigalati/usad)
  - [Youtube explaination](https://www.youtube.com/watch?v=gCleQ9JxibI&ab_channel=%EA%B3%A0%EB%A0%A4%EB%8C%80%ED%95%99%EA%B5%90%EC%82%B0%EC%97%85%EA%B2%BD%EC%98%81%EA%B3%B5%ED%95%99%EB%B6%80DSBA%EC%97%B0%EA%B5%AC%EC%8B%A4)
- You have to adjust the threshold to your model result


### 2. GAN based model colab code
- run Timeseries_Anomaly_Detection_Transformer_colab.ipynb at colab
- You can choice the model in Transformer or GRU.
  - model_type='transformer' or model_type='gru'




## Term 프로젝트를 소개합니다!!

Time-Series Anomaly detection을 수행하는데는 여러가지 모델이 있습니다.

Transformer, GRU 기반으로 다음 step의 값을 예측하여 실제 값과 차이가 크면 anomal이다 라고 예측하는 방법이 있고

GAN(USAD) 모델로 12step의 센서값들을 인식 한 후 예측값과 실제값의 차이가 크면 anomal이라고 예측하는 방식이 있습니다.

본 텀프로젝트에선 다양한 모델들을 돌려보고 튜닝 해보면서 최종 metric인 TaPR를 비교합니다

TaPR점수가 가장 높은분이 우승입니다

https://github.com/airobotlab/lecture_6_timeseries_AnomalyDetection에 접속해서 두 ipynb 파일을 colab에서 돌리고 튜닝해서 최고의 TaPR 점수를 획득해보세요

GAN 기반 Anomaly detection의 설명 유튜브 링크입니다.
https://www.youtube.com/watch?v=gCleQ9JxibI&ab_channel=%EA%B3%A0%EB%A0%A4%EB%8C%80%ED%95%99%EA%B5%90%EC%82%B0%EC%97%85%EA%B2%BD%EC%98%81%EA%B3%B5%ED%95%99%EB%B6%80DSBA%EC%97%B0%EA%B5%AC%EC%8B%A4

- 데이터 준비
  - 1) 데이터를 dacon에서 다운받은 후(https://dacon.io/competitions/official/235757/data)
  - 2) 구글 드라이브에 업로드 합니다
  - 3) colab을 수행하며 로그인 밑 구글드라이브를 colab에 연동합니다

- 학습

- 결과
실제 anomal이 발생했을 때(주황색 그래프가 솟은 부분)를 잡기 위해 THRESHOLD를 지정해 줍니다(빨간선)
