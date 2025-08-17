# 사용자 클러스터 분석을 통한 익명 투표 기반 SNS 활성화 전략
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=Python&logoColor=white"> <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=MySQL&logoColor=white">


## 프로젝트 개요
### 분석 목적
우리 서비스 고활성화 학교의 성공 방정식을 찾아내 다른 학교에 적용함으로써, 서비스 전체의 사용자 활성화 수준을 상향 평준화한다
1) 서비스 활성화 패턴 분석 : 학교별로 서비스 이용 패턴을 클러스터링하여 활성화 패턴에 따라 학교를 분류하고, 각 클러스터의 특징을 파악한다
2) 고활성화 학교 특징 발굴 : 가장 활성화된 클러스터의 특징을 심층적으로 분석하여, 해당 학교들이 어떤 패턴을 보이는지 확인한다
3) 고활성화 학교의 특징을 저활성화 학교에도 적용하여 서비스 전체의 활성도를 높일 수 있는 A/B 테스트 아이디어를 제안한다

### 활용 데이터
**유저 이벤트 로그 데이터 (총 4,113개 학교 / 유저 98,789명)**
![data](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/data.png)

### 수행 역할
- pandas, matplotlib, seaborn을 활용한 데이터 분석 및 시각화
- 클러스터링 모델 선정 및 모델 학습
- A/B테스트 설계
---

## 분석 과정 및 주요 결과
![clustering_process](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering_process.png)
![preprocessing](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/preprocessing.png)
![clustering1](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering1.png)
![clustering2](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering2.png)
![clustering3](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering3.png)
![clustering4](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering4.png)
![clustering5](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering5.png)
![clustering6](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering6.png)
![clustering7](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/clustering7.png)

   
### 개선제안
- SNS 이용에 있어 우리 서비스가 고활성화된 학교는 그렇지 않은 학교 대비 '친구 초대', '질문 공유'와 같은 소셜 기능을 적극적으로 활용하고 있고, 이것이 메인 이벤트의 발생 빈도를 높이고 서비스 활성화에 기여하고 있는 것으로 확인됨
- 타 클러스터에도 확대적용을 위해 A/B테스트 설계함
![abtest](https://github.com/Myungbin-Choi/SNS_activation_project/blob/main/images/abtest.png)
---

## directory structure
```bash
├── README.md                     <- 프로젝트 요약 설명
├── SNS_activation.ipynb          <- 분석 통합 파일 (preview 용)
├── SNS_activation.py             <- 분석 통합 파일 (code 공유용)
├── SNS활성화 프로젝트_요약보고서.pdf    <- 프로젝트 3page 요약 파일
├── SNS활성화 프로젝트_보고서.pdf       <- 프로젝트 보고서 요약 파일
├── images                        <- 주요 이미지 파일        
```
