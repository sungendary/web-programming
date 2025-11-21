# web-programming


이 프로젝트는 서울의 다양한 장소를 사용자 특성에 따라 추천해주는 반응형 웹사이트입니다.
아래는 사용된 주요 기술과 코드 내 반영 위치에 대한 설명입니다.

───────────────────────────────
1. CSS3를 사용해 수평 정렬하는 방법
→ `.place`, `.category`, `.subcategory` 등은 `display: inline-block` 스타일을 통해 버튼들을 수평 정렬합니다.

2. CSS3를 사용해 중앙 정렬하는 방법
→ `body { text-align: center; }`, `#title-container`, `#video-container`는 `display: flex` 및 `justify-content: center` 등으로 중앙 정렬 처리.

3. CSS3를 사용해 One True 레이아웃을 구성
→ `#map-wrapper`는 `display: flex`로 구성되어, 지도와 정보 패널이 한 줄에 나란히 배치됩니다.

4. CSS3의 절대 좌표를 활용
→ `.sidebar`는 `position: fixed`로 지정되어 페이지 스크롤과 무관하게 고정 위치에 배치됩니다.

5. 반응형 웹을 구현하는 방법
→ `@media (max-width: 768px)` 미디어 쿼리를 통해 모바일 환경에 맞는 UI를 별도로 구성했습니다. (ex. 사이드바 숨김)

6. 자바스크립트, 객체, 문서객체모델(DOM), jQuery 라이브러리, jQuery 플러그인 사용
→ JS 함수 `showSubcategories`, `showPlaces`, `searchPlaceOnMap` 등은 DOM 조작 기반이며,
   jQuery는 Slick Carousel 초기화 및 이벤트 처리에 사용됩니다.
   - jQuery 사용 예: `$(document).ready()`, `$('#title-container').slick()`

7. 효과적인 디자인 구성 적용
→ 버튼에 hover/active 시 shadow, 색상 변경 등으로 사용자의 인터랙션 피드백을 제공합니다.
→ `box-shadow`, `border-radius` 등의 스타일도 디자인 효과를 고려하여 적용.

8. 오디오 및 동영상 활용 가능(option)
→ `<iframe id="youtube-video" src="...">` 요소로 유튜브 영상을 임베딩하여 멀티미디어 요소를 추가했습니다.

───────────────────────────────
사용 방법

1. 웹 페이지를 열면 유튜브 소개 영상과 카테고리 버튼이 표시됩니다.
2. 카테고리를 선택하면 관련 서브카테고리 버튼이 동적으로 생성됩니다.
3. 서브 카테고리를 선택하면 추천 장소 리스트가 버튼 형태로 생성됩니다.
4. 장소를 클릭하면 지도와 함께 주소, 소개, 경로 등의 정보가 표시됩니다.
