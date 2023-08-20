# SW_HACK43
## 프로젝트 
### 개요
- "걷기 좋은 길 추천 웹"은 지도 API를 활용하여 사용자의 위치 정보에 기반한 개인화된 산책로를 제안하는 서비스입니다.
- 사용자의 취향, 원하는 거리, 활동 수준 등을 고려하여 매일 다양한 산책로를 제공하며, 사용자의 건강과 웰빙을 증진합니다.
- 이 웹은 또한 다른 사용자들의 리뷰와 평점, 사진을 통해 다양한 산책로의 풍경과 분위기를 공유하고, 좋은 산책로를 발견하는 데 도움을 줍니다.

### 배경

## 개발인원(Member)
|이름|역할|담당|이름|역할|담당|
|--|--|--|--|--|--|
|장태환|BE 팀장| 지도 API를 통한 적도,경도 계산, API CRUD |조서우|디자이너| 페이지 디자인 |
|윤건우|BE 팀원| JS로 지도그리기 |김동영|FE 팀원| 페이지 작성 |
|조원지|FE 팀원| 페이지 담당 

## 프로젝트 기술 스택
### Environments
<img src="https://img.shields.io/badge/intellij-000000?style=for-the-badge&logo=intellijidea&logoColor=white"><img src="https://img.shields.io/badge/visualstudiocode-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white"><img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white"><img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">

### Development Stack
#### BackEnd

<img src="https://img.shields.io/badge/springboot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white">

#### FrontEnd
<img src="https://img.shields.io/badge/JSP-F7DF1E?style=for-the-badge&logo=jsp&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=white">
<img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white">

### Communicatoin
<img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white"><img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"><img src="https://img.shields.io/badge/notion-000000?style=for-the-badge&logo=notion&logoColor=white"><img src="https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=Discord&logoColor=white">

## 프로젝트 진행 과정
- 피그마를 이용해 목업 디자인 스케치와 메인 디자인 
- 페이지 별 역할 분담
- 기능 구현


## 프로젝트 구현 내용

<img width="765" alt="스크린샷 2023-08-20 오후 11 49 19" src="https://github.com/Taehwan2/SW_HACK43/assets/97010824/15660b52-70cf-40f4-8bf0-7805630f9357">

1. 사용자가 난이도랑 원하는 KM를 입력하면 그 정보를 JSON을 통해서 받고, 사용자의 현재 위치를 받아와서 저장한다. 

<img width="556" alt="스크린샷 2023-08-20 오후 11 50 12" src="https://github.com/Taehwan2/SW_HACK43/assets/97010824/cac11161-db8d-4eaf-ae80-378467876c38">

2. TMAP API를 사용하여 주변 KM의 목적지에 있는 장소를 불러오고, GOOGLE MAP API를 사용하여 목적지 까지 가는 경도와 위도를 계산하여 오르막길이나 내리막길을 판단해 난이도를 설정해 준다.
   
<img width="974" alt="스크린샷 2023-08-20 오후 11 50 30" src="https://github.com/Taehwan2/SW_HACK43/assets/97010824/1ead720a-9bd1-4150-9d94-f5fa40a1e400">

## 프로젝트 한계 및 개선 방안
- Google MAP은 보안 때문에 한국 지도에서 걷기에 대한 정보를 얻어 올 수 없었다 -> TMAP을 사용하여 해결
- TMAP은 다중 경로를 받아올 수 없었다 -> GOOGLE MAP을 사용하였다.
- JSON파일로 수많은 정보가 들어와서 확인이 어려웠다 -> JSON 파싱을 통해 JSON의 계층구조를 확인하고 경도 위도를 파악했다.
- front를 다룰 수 있는 사람이 부족했다. -> 지도를 위주로 JS를 사용하여 웹 페이지를 구현했다.

