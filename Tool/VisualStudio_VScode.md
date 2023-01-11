# VSCode
## Setup
- snippet : 명령 단축키 설정
  - Preferences > Configure User Snippets
  - global : 전역 / folder : 해당 폴더 하위 적용

## HotKey
### Command
- 도움말 : command + ?
- Ctrl + P : search file. : command
- Ctrl + shift + P : 기능 검색/실행 Command 열기. : command + > : F1
- Ctrl + G : search line number. : command + :

### SideBar
- Ctrl + B : Left Side Bar ON/OFF
- Ctrl + shift + E : Open Explorer
- Ctrl + shift + F : Open Search
- Ctrl + shift + G : Open Git
- Ctrl + shift + D : Open Debug
- Ctrl + shift + X : Open Expansion
- Ctrl + , : Setting

### FootBar
- Ctrl + ` : Terminal ON/OFF

### Typing
- Ctrl + k + c : 주석 묶기.
- Ctrl + k + u : 주석 풀기.
- Ctrl + Z : Undo
- Ctrl + Y : Redo

## Expansion
### Offline install
- [VSCode Extensions](https://marketplace.visualstudio.com/vscode)에서 필요한 Extensions 다운로드.
- 기능 검색/실행 Command 열기 > install from VSIX > 다운로드 파일 선택.

### Explorer
- vscode-icons : Explorer 출력되는 파일 앞에 해당 확장자에 맞는 아이콘 표시.
- Project Manager : 프로젝트 스위칭, 관리.

### Typing
- TabOut : [], {}, (), '', "", ;, <>, 등등... 블록 끝단에서 Tab으로 탈출 가능. / 자동완성에 문제 있을 수 있음.
- Todo Tree : TODO, FIXME 등... 해당 태그의 주석을 검색해서 Todo List 관리.
- Color Highlight : 색상 코드에 해당 색상으로 하이라이트 표시.
- Path Intellisense : 파일 경로 인텔리전스.
- Diff : 두 문서의 내용 비교.
- Auto Rename Tag : html Tag 양쪽 동시에 수정.
- prettier : 문서 양식을 정해진 규칙에 따라 정리한다.
  - ctrl + k + f : 선택한 구역 안에서 수동 정렬 실시.
  - setting
    - Format On Save : 저장과 동시에 포맷 정렬.
    - Default Formatter : 기본 정렬 기준... prettier으로 변경 해야 prettier 기준으로 포맷 변경 실시.
    - Require Config : root에 설정 파일이 존재하는 경우에만 Prettier가 적용된다.
    - 해당 확장자(파일)에서 적용이 안되는 경우.
      - F1 => Format Document With...
        => Configure Default Formatter...
        => Prettier - Code formatter
  - .prettierrc(설정 파일)
  ```
  {
  // 줄당 코드량 기준
  "printWidth": 80,
  // 홑 따옴표
  "singleQuote": true,
  // 세미콜론
  "semi": true,
  // 탭 띄우기 크기
  "tabWidth": 2,
  // 배열 등의 끝에 쉼표 붙는 기준
  "trailingComma": "es5",
  // [], {} 안에 띄어쓰기
  "bracketSpacing": true,
  // [], {}, <> 등의 마지막 기호의 위치
  "bracketSameLine": true,
  // 애로우 함수의 인자를 감싸는 () 삭제 유무
  "arrowParens": "avoid"
  }
  ```
- Error Lens : error 실시간 표시.
- Tailwind CSS IntelliSense : TailwindCSS 클래스 인텔리전스.
  - 정상 작동이 안될 경우, HTML CSS Support를 추가 설치.

### Command
- Output Colorizer : OUTPUT 창의 로그들에 구문 강조 기능.

### Web
- live server : 파일 저장과 동시에 브라우저 갱신 처리.
- REST Client : REST API 테스트.
- Thunder Client : REST API 테스트.

### Git
- GitLens
- Git History : git log 확인.
  - Alt + H : 해당 파일의 history
  - 전체 확인은 command 이용.
- Git Graph : git log 확인.
  - StatusBar의 Git Graph 버튼 이용.

## Issue
- 확장자 인식 문제 : Syntax Highlight나 Intellisense에 문제가 생길 수 있다.
  - Manage > Settings > File Associations > Add Item >  Item(현재), Value(목표)

# Visual Studio
## HotKey
### Command
