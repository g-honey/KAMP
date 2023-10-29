# KAMP
## LPK
The code is copyrighted by LPK.   
The code in the guidebook is copyrighted by KAMP.   

It was running on a jupyter notebook.  
For outlier removal, I did not remove them by code, but by eye, as the values were not regular and the code had limitations.  
Put the original datasets together.   


I've also posted the actual presentation.  
I also added a watermark just in case, but if you need a watermark-free version, please email me.  
My email is g.hyeon@seoultech.ac.kr or other team member's email is dsekdls725@seoultech.ac.kr.
  
------------------------------------------------------------------------

2022년 제 2회 K-인공지능제조데이터 분석 경진대회  
실제 제조 현장의 용해 공정 데이터를 가지고 분석.  
데이터는 https://mdata.kamp-ai.kr/ 에 공개되어 있음. 

Feature Importance.ipynb :  
이상치를 직접 탐지하여 데이터를 수정하고, decision tree를 사용 해 feature importance를 뽑을 수 있었다.   
  
EDA, ML/이상치 제거_1 ... 이상치 제거_6 :  
이상치를 제거 한 데이터를 가지고 시계열 딥러닝 분석 방법 적용.  
LSTM, GRU, TCN등을 사용하여 각각 레이어를 다르게 쌓았을 때 정확도의 변화를 볼 수 있다.  
  
EDA, ML/이상치 제거_7 ... 이상치 제거_8 :  
가장 성능이 좋은 시계열 방법과 레이어를 가지고 전체 데이터에 대해 사후확률을 받아온다. 
2-fold 테스트를 수행하여 전체 데이터에 대한 사후확률을 받아오고 가공하여 새로운 데이터를 생성한다.  
새롭게 생성한 데이터를 가지고 decision tree를 만들어 규칙을 생성한다.  
이렇게 생성된 규칙은 딥러닝 모델을 설명한다.  
