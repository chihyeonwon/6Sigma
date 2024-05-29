# 6Sigma
Minitab 3급, 6시그마 GB 자격취득과정      
Minitab 6시그마 데이터 분석         
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/62771206-5cc5-42d5-a8bd-6c1c82db71b7)
```
연속형, 히스토그램, 정규형 분포 곡선
PPM 총계 기대 성능 8986 -> 89.86% 가 불량률임

평균 : 357.2초 표준편차 92.0129

단기 시그마 수준 Zst = Zlt + 1.5 = -1.27 + 1.5 = 0.23
장기 시그마 수준 Zlt = -1.27


시그마 수준은 2가지
Zst (단기 시그마 수준 = 최고 능력, 잠재 역량)
Zlt (장기 시그마 수준 = 현수준)

Zst = Zlt + 1.5(경험치,차이)

현수준에 1.5 더하면 최고 능력과 유사하다.

z = -1.27 + 1.5 => 0.23

0.23 단기
-1.27 장기, 현수준

공정이 최적화된다면 경험으로보아 0.23

합격률은 100 - 89.86 = 10.14 %

분석 결과 및 분석계획 : 불량률 89.86 % z = -1.27으로 매우 심각한 수준이므로 프로세스 개선과 임직원
역량 강화가 필요하다.
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/cb2f1dcb-b36e-499e-941a-990906346f79)
```
2라운드 제조
z(시그마수준) = 1.67 불량률 = 47415 -> 4.7%

평균 113.567, 표준편차 : 39.7698
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/bdadc29c-e17b-4aab-b294-31040258a19d)
```
공정 z = 73.51 zlt 가 0.7351

zst = zlt + 1.5 = 2.23 까지 가능

불량률 23.11% z=0.73 으로 다소 미흡한 수준으로 숙련도 향상이 필요
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/e926ca28-9fa8-4128-bdaa-5b64afe3e259)
```
5점 만점에 평균 3.78 z 시그마 수준이 -0.22 이므로 다소 미흡하다.

```
## 정규성 검증

x 평균 중심 좌우 대칭 -> 정규분포    
x 값의 분포가 정규분포와 같은지를 판단   

비정규분포 : 공정 매우 불안정, 샘플링 오류 -> 데이터 신뢰 어렵 -> 샘플링 달리하거나 or 추가 수집     
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/f7dcead9-a4d5-4f1f-b74f-4b4e1ccfd0eb)
```
1라운드 총 시간 귀무가설 H0, p>0.05 p=.0.492, 정규성을 따른다.  

빨간색 선 -> 정규분포
점 -> x값 분포

만약에 1라운드 총 시간이 100% 정규분포와 일치한다면 x평균과 좌우대칭

P=0.492 > a = 0.05 
1-총시간분포 = 정규분포
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/05b2af64-8967-49e5-9187-4da344b99228)

```
2라운드 총 시간 귀무가설 H0, p>0.05 p=.0.429, 정규성을 따른다.  
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/e94fd09d-e15c-46d2-93c9-bde830a38c11)
```
2표본 분산 검정

1 라운드 총시간, 2 라운드 총시간 두 개 다 정규성을 따를 때 -> F 검정으로 검증한다.

정규 분포를 바탕으로 하는 검정 및 신뢰 구간 사용에 체크

P = 0.002 일 때 a = 0.05 보다 작으므로 h1 대립 가설 V1 != V2, 차이가 있다. (차이는 개선되서, 개선X)

1라운드 -> 2라운드 가면서 산포가 줄어듬 -> 개선이 되어서 차이가 있다.

* -> 이상치 -> Q3 + 1.5 * IQR 보다 큰 값 이 이상치
이상치는 삭제

삭제하고 다시 분석 해야 한다.
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/0ebcdb20-1803-45de-85dc-aa38d0eb10e5)
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/d9022511-f301-4de7-8f8c-77205fdb144d)
```
1 라운드 22 셀 delete로 삭제하고 다시 분석
```
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/1b23f764-a471-46cd-92a3-85d51619d3fd)
```
이상치 하고 다시 분석 p = 0.036 < 0.05 v1 != v2

산포는 확실히 개선되었다.
```
















## 개발에서의 6 Sigma
#### Work(Quick Action) VS Project 
```
프로젝트와 단순 Work를 구분하여 사용자의 needs, seeds, wants를 개선 improve하는 방법 method를 논리적 logical 하게 해결하기 위함
단순 UI나 View, widget 배치같은 경우 work quick action으로 구분
사용자들의 불편사항 중 project를 장기간 프로젝트로 구성

회사가 원하는 USL 보다 높은 이상치를 목표 의지 -> 승인
너무 과해도 적정수준을 찾는다.

목표, 범위, 일정, TFT 구성
목표  reject 1순위
일정 GB- 1 ~ 3개월 reject 2순위
TFT 팀원 멤버 구성의 문제 3순위

평상시에 의중 -> 보고서 반영 => 커뮤니케이션
```
```
5월 27일~30일 6to10

시간은 30문제(5지선다) 30분간 진행되며 GB 60점
시험은 Google 설문지 폼 양식을 통해 진행되며, 이메일로 시험지가 예약 발송됩니다.교육 수료증 및 자격증 교부 절차

-.실습과제 제출:  jobkcdi@naver.com , 이메일제목: 대학명-과정명-성명
-.수료증은 교육과정 이수 후 실습과제 파일을 1주일 이내에 제출자에 한함
-,자격증은 교육수료 및 실습과제 제출, 시험합격자에 한하여 취득할 수 있습니다. 
-.교육수료증과 자격증은 한국커리어개발원 마이페이지에서 JPG  파일로 다운로드
```
#### Minitab 18
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/c49cb25a-c552-4999-aac5-2505d7cb5ad9)
![image](https://github.com/chihyeonwon/6Sigma/assets/58906858/dc4f2f4a-1de8-4bd4-b481-c5e6c0a65585)


#### 고용노동부 지정 직업교육(NCS코드) 수료증 
#### 한국직업능력개발원 등록 직무자격증
