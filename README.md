# Vue.js



## Vue.js의 특징

- vue.js는 Evan you가 UI를 빠르게 개발하기 위해 만들었다. 
- 웹 화면 작성에 최적화된 프레임워크.
- 최근 가장 빠르게 발전하고 확산하는 프레임 워크.
- Vue.js는 다른 프레임워크와 달리 유연하고 가볍다.
- Anuglar와 달리 웹 애플리케이션의 일부 UI 화면만 적용하는 것이 가능하다.
- Vue.js는 learning curve가 완만하다. 
- Vue.js MVVM 패턴을 따른다. Model - View - ViewModel
- MVVM 패턴은 애플리케이션 로직과 UI를 분리하는 패턴이다.
- View는 HTML과 CSS로 작성된다.
- ViewModel은 View의 실제 논리와 데이터 흐름을 담당한다.
- View는 ViewModel만 알고 있으면 된다.
- 비즈니스 로직에서는 ViewModel의 상태 데이터만 변경하면 즉시 View에 반영된다.
- MVVM 아키텍쳐
- ![1-1](.\images\1-1.png)



- Vue.js는 가상 DOM을 지원하므로 아주 빠른 UI 렌더링 속도를 제공한다.

  

## 개발환경 세팅

- Node.js : 서버 측 자바스크립트 언어이자 플랫폼이다.

- npm : 앱의 의존성 관리를 위해 사용하는 노드 패키지 관리자이다.

- Visual Studio Code : 코드 편집 도구.

- 크롬 브라우저 + Vue.js devtools : 크롬 브라우저 기반에서 작동하는 Vue.js 전용 디버깅 개발 도구.

- Vue-CLI : 앱 작성을 위한 기본 틀을 제공하는 도구.

### Node.js 설치



- Node.js는 Google V8 엔진을 기반으로 만들어진 서버 측 자바스크립트 언어이자 플랫폼.

- npm을 활용하여 Vue.js 관련 도구를 설치하고 앱의 의존성 라이브러리를 관리.

- Express 웹 프레임워크를 이용해 Vue.js 애플리케이션이 액세스하는 API 서비스를 작성.

https://nodejs.org/ko/ 에서 LTS 버전 설치.

설치 후 cmd 창에서 npm을 최신버전으로 업그레이드.

```cmd
npm install -g npm
# -g는 Global 옵션이다. 어디서든 실행가능 하도록 설치.
```



### Visual Studio Code 설치

http://code.visualstudio.com 에서 다운로드.

추천 플러그인

- view-in-browser : html 파일을 기본 브라우저로 볼 수 있게 한다.
- vetur : Vue.js 코드에 대한 문법, 코드 자동완성, 디버깅, 린팅 기능을 제공.
- HTML Snippets : HTML 태그 조각을 빠르게 작성할 수 있도록 도와준다.
- JS-CSS-HTML Formatters : JS, CSS, HTML의 코드 자동완성 기능을 제공. 에디터 창에서 CTRL + SPACE를 눌러 사용.
- Vue 3 Snippets : Vue.js 3.0의 코드 조각 지원과 문법 강조 기능을 제공.
- Vue-beautify : Vue.js 코드에 대한 정리 배치 기능을 제공.
- ESLint : 자바스크립트 코드 스타일, 문법 체크 기능 제공.



### Vue.js devtools 설치

대규모 애플리케이션을 개발할 땐 디버깅이 필수이다. 

디버깅시 유용한 Vue.js devtools를 설치하자.

크롬 웹스토어에서 Vue.js 검색 후 설치. 



### Vue-CLI 설치

- Vue-CLI는 에반 유가 공식적으로 관리하는 커맨드라인 인터페이스 기반의 스캐폴딩 도구이다.

- Vue.js 앱을 개발할 떄 프로젝트 폴더 구조를 어떻게 잡을 것인지 테스트, 빌드 의존성 부분은 어떻게 설정할 것인지 프로젝트의 기본 템플릿을 설정해주는 도구.

- cmd 창에서 npm을 이용해 Vue-CLI 설치.

  ```
  npm install -g yarn @vue/cli
  ```

- Vue CLI 3.x 버전에서는 npm 대신 yarn 패키지 매니저를 사용한다.

- yarn이 npm보다 실행속도가 빠르기 때문.
