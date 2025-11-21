# 🐯 SEOULINONE (서울인원)

**SEOULINONE**은 인원 구성(혼자, 연인, 가족, 친구, 단체, 외국인)에 맞춰 서울의 핫플레이스를 추천해주는 웹 서비스입니다.
사용자 맞춤형 장소 추천과 함께 네이버 지도 API를 활용하여 위치 정보를 직관적으로 제공합니다.

<br>

## 📸 주요 기능

* **👥 인원별 맞춤 추천**: 방문 인원 및 목적에 따른 최적의 장소 카테고리 제공
* **🗺️ 지도 위치 확인**: 네이버 지도를 통해 선택한 장소의 위치 및 경로 확인
* **⭐ 상세 정보 제공**: 장소별 한 줄 소개, 주소, 별점 정보 표시
* **🎥 소개 영상 연동**: 서울 관광 관련 유튜브 영상 재생 기능

<br>

## 🛠️ 기술 스택 (Tech Stack)

* **Frontend**: HTML5, CSS3, JavaScript (Vanilla JS + jQuery)
* **API**: [Naver Maps API v3](https://www.ncloud.com/product/applicationService/maps) (Geocoding 포함)

<br>

## 🚀 설치 및 실행 방법 (Getting Started)

이 프로젝트는 **네이버 지도 API**를 사용하므로, 실행 전에 **API 키(Client ID) 발급 및 설정**이 필수입니다.

### 1단계: 네이버 지도 API 키 발급받기
1.  [네이버 클라우드 플랫폼](https://www.ncloud.com/)에 접속하여 로그인합니다.
2.  우측 상단의 **[Console]** 버튼을 클릭하여 콘솔로 이동합니다.
3.  좌측 메뉴에서 **Services** > **Maps**를 선택합니다.
4.  **[Application 등록]** 버튼을 클릭합니다.
5.  **Service 선택** 항목에서 **Web Dynamic Map**을 체크합니다. (필요 시 Geocoding도 체크)
6.  **서비스 URL** 설정:
    * **로컬에서 테스트할 경우**: `http://localhost` 또는 `http://127.0.0.1`을 추가합니다. (VS Code의 Live Server 등을 이용할 때 필요)
    * **웹에 배포할 경우**: 실제 배포될 도메인 주소를 입력합니다.
7.  등록 완료 후, 해당 앱의 **인증 정보(Client ID)** 값을 복사해 둡니다.

<br>
<br>

### 2단계: 프로젝트 클론 및 설정
터미널에서 아래 명령어를 입력하여 프로젝트를 다운로드합니다.

git clone [https://github.com/your-username/SEOULINONE.git](https://github.com/your-username/SEOULINONE.git)

<br>
<br>

### 3단계: API 키 입력 (Client ID 설정)

1. index.html 파일을 열고, <head> 태그 내의 약 6번째 줄에 있는 아래 코드를 찾습니다.

2. ncpClientId= 뒤에 있는 YOUR_CLIENT_ID_HERE 문자열을 발급받은 본인의 Client ID로 정확하게 교체합니다.

<br>
<br>

### 4단계: 실행하기

VS Code에서 index.html 파일을 열고, Open with Live Server를 통해 실행합니다.

주소창이 http://127.0.0.1:5500/... 형태인지 확인하세요.
