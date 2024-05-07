# autonomous-wheelchair
[python] 데굴이: 자율주행 휠체어 제작 프로젝트

# :mega: 프로젝트 개요
2023 한양여자대학교 캡스톤 디자인 프로젝트로, **데굴이: 대형병원 내 자율주행 휠체어 로봇** 제작 프로젝트입니다. 
휠체어 로봇을 통해 **환자의 이동 자율성을 확보**하고 **간호인력을 효율적으로 운용**해 **병원 내 혼잡도 개선**을 목표로 합니다.

로봇과 서버PC간의 정보 전달 및 어플리케이션 연동이 주요 과제입니다.

# :computer: 개발 정보
### :clock10: 개발기간 : 2023.03 ~ 2023.11
### :busts_in_silhouette:	멤버 구성
- 인원: 4명
- :raising_hand: **팀장**(본인) :
  - 프로젝트 일정 관리, 문서 작성, 멘토링 회의 진행 
  - ROS 환경 구성(기여도 80%),  자율주행 rule 주행 로직 개발(기여도 80%),  서버PC-어플리케이션 publishing (기여도 70%),  어플리케이션 수동조작 로직 개발 (기여도 90%)


### ⚙️ 개발환경
- **OS** : Ubuntu 18.04
- **ROS** : melodic
- **개발언어** :python

# :page_with_curl: 프로젝트 내용
### 1. 개발 배경 및 필요성
<p align="left" width="100%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/bb86873d-8eb4-47d5-9aed-96554a0244a9.png" width="49%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/9f656564-dde4-4708-b9e1-6842cb6bd843.png" width="49%">
</p>

---

### 2. 프로젝트 개요 및 구조
- **개발환경**: ROS가 설치된 라즈베리파이(로봇), 서버(PC)로 구성됨. publisher를 통해 통신
- **프로세스**: 자율주행 휠체어 로봇에서 서버와 관제페이지로 정보 전달, 서버에서는 자율주행 경로 정보를 휠체어로 전달함. 관제 페이지에서는 휠체어 로봇의 정보를 받아 휠체어 로봇의 현황을 파악함

<p align="center" width="100%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/17204e6b-f054-4700-8917-976337a1c9f7.png" width="49%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/7a222de8-9189-4785-a761-65a5f3973723.png" width="49%">
</p>


---
### 3. 휠체어 로봇 기능

**1. 병원 지도 제작** : ROS의 SLAM 기능을 사용한 병원 내부 지도를 제작

**2. 자율주행** : 정해진 경로로 주행 해 안전사고를 예방한 자현
<p align="center" width="100%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/d3fd1cdb-2db0-4fdd-ad28-5fa8ed998129.png" width="49%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/3e6bc349-96f6-4fc9-9abd-ac743a71d8a1.png" width="49%">
</p>
<p align="center" width="100%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/6eb09447-829a-4c88-ac0c-8e53600f9222.png" width="49%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/022d3234-54cc-4629-a53c-796b8f240439.png" width="49%">
</p>
<p align="center" width="100%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/e7e94c63-25da-41ae-b7f3-03b75de82fb0.png" width="49%">
	<img src="https://github.com/Budayeong/autonomous-wheelchair/assets/115779162/e0c11786-72ff-4c8c-ac57-03ce22effb84.png" width="49%">
</p>
