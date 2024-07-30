# '아티팩트_집' (Artifacts_zip)

## 프로젝트 소개
'아티팩트_집'은 Claude AI의 '아티팩트' 기능을 활용하여 생성된 슬라이드를 쉽게 관리하고 표시할 수 있는 오픈소스 프로젝트입니다. 이 도구는 Claude가 생성한 여러 슬라이드를 하나의 프레젠테이션으로 통합하여 사용자가 더 긴 프레젠테이션을 만들 수 있도록 도와줍니다.

## 개발 배경
- Claude AI의 아티팩트 기능을 사용해 생성한 슬라이드를 효과적으로 활용하고자 하는 사용자들의 요구에 부응하기 위해 개발되었습니다.
- 텍스트를 시각적으로 보기 편한 레이아웃으로 변환하거나, 발표 자료로 쉽게 바꿀 수 있는 도구의 필요성에서 시작되었습니다.
- Claude의 아티팩트 생성 길이 한계를 보완하고, 여러 슬라이드를 하나의 프레젠테이션으로 통합하는 솔루션을 제공합니다.

## 주요 기능
- Claude AI가 생성한 슬라이드 아티팩트를 쉽게 통합하고 관리
- React 기술을 활용한 웹 기반 슬라이드 뷰어

## 설치 및 사용 방법

### 사전 요구사항
- 기본적인 코드 실행 경험
- VSCode, GitHub, Node.js가 설치되어 있어야 합니다.

### 설치 단계
1. 이 저장소를 클론하거나 다운로드합니다.
2. 터미널에서 프로젝트 디렉토리로 이동합니다.
3. 다음 명령어를 실행하여 필요한 패키지를 설치합니다:
   ```
   npm i
   ```

### 실행 방법
1. 터미널에서 다음 명령어를 실행하여 서버를 시작합니다:
   ```
   npm start
   ```
2. 웹 브라우저에서 `localhost:3000`으로 접속하여 애플리케이션을 사용할 수 있습니다.

### 새 슬라이드 추가하기
1. `/src/components/slides/` 폴더에 새 파일(예: `slideX.js`)을 생성합니다.
2. Claude에서 생성한 아티팩트 내용을 다음 형식에 맞춰 파일에 붙여넣습니다:
   ```javascript
   import React from 'react';
   class SlideX {
     static title = "슬라이드 제목";
     static chapterNumber = "X.X";
     static Content() {
       return (<> {/* 슬라이드 내용 */} </>);
     }
   }
   export default SlideX;
   ```
3. `App.js` 파일의 import 섹션에 새 슬라이드 컴포넌트를 추가합니다. (16번 라인)

## 기여 방법
이 프로젝트에 기여하고 싶으신 분들은 pull request를 보내주시기 바랍니다. 모든 기여를 환영합니다!

## 연락처
프로젝트에 대한 질문이나 제안이 있으시면 iksw9999@gmail.com 로 연락 주시기 바랍니다. 감사합니다.