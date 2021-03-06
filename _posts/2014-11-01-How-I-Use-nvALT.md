---
layout: post
title: How I use nvALT
date: 2014-11-01 15:27:28
tags: app productivity note How-I-Use
---

1. nvALT 소개
2. nvALT의 특징
3. nvALT 기본 사용법
    1. 노트 검색/관리
    2. 새로운 노트 만들기
    3. 노트에 태그 지정하기
    4. 노트 즐겨찾기 이용하기
    5. 노트 미리보기
4. 노트 작성 팁
    1. 북마클릿을 이용해서 노트 작성
    2. 웹브라우저 익스텐션을 사용해서 노트 작성
    3. Keyboard Maestro Macro를 이용해서 빠른 노트 작성
5. 맺음말

---

## nvALT 소개

[nvALT][nv]는 [Brett Terpstra][brett]가 Notational Velocity를 기반으로 만든 맥용 plain text 글쓰기 앱이다. 겉으로 보기엔 정말 평범하고 어찌 보면 다른 유려한 디자인의 글쓰기 앱보다 이전 시대의 유물 같아 보일 수 있다. 유물이라는 표현은 조금 심했다. 어쨌든 nvALT는 일기를 잘 쓰지 않던 사람도 일기를 쓰고 싶어지게 한다는 [DayOne](http://dayoneapp.com/)과 같은 앱은 아니다. 하지만 nvALT는 사용자가 적어야 하는 글의 내용에 집중하도록 돕는다. 이미 작성한 노트를 관리, 검색하는 것도 매우 빠르다. 단순한 외형 속에 숨어 있는 기능을 사용하다 보면 어느새 뭔가 적을 일이 생기면 자연스레 nvALT를 실행하는 자신을 발견하게 된다.

> nvALT doesn’t just record your words; it’s specifically designed to make searching for and organizing your notes super-fast and easy. _from [Macworld](http://www.macworld.com/article/2047073/nvalt-review-makes-writing-and-finding-plain-text-notes-simple.html "nvALT review: Makes writing and finding plain-text notes simple | Macworld")

나는 아주 긴 호흡의 글이 아니라면 모든 글을 nvALT에서 쓴다. 긴 호흡의 글도 처음에는 nvALT에서 쓰기 시작해서 Scrivener로 옮겨 가는 경우가 많다. nvALT는 개발자의 [프로젝트 페이지][nv]에서 무료로 내려받을 수 있다.

## nvALT의 특징

* **[[ ]]사이에 들어 가는 단어들이 다른 노트들의 링크가 된다.** 많은 노트를 간단히 서로 연결할 수 있다. 특정 주제에 대해 많은 자료를 수집하는 경우 상당히 유용하다. [[ ]] 안에 노트 제목을 입력할 때 자동완성 기능을 지원한다(옵션에서 선택 가능, shortcut = ⌘⇧L).
* **막강한 태그 입력 & 동기화**
	* **nvALT에서 각 노트에 입력한 태그는 Dropbox를 통해 동기화되며 Spotlight에서 검색할 수 있다.**
	* **태그 입력 시 자동 완성** 기능은 기본이다.
	* **여러 노트를 다중 선택해서 태그 입력**이 가능하다.
* [**TaskPaper**][7184-001]를 사용하는 사람에겐 **"@done" 태그를 지원**하여 strikethrough 형식을 지원한다.
* **자동 저장 기능**이 있다. 실컷 적던 글을 날리고 중간중간 저장을 하지 않은 자신을 자책하지 않아도 된다.
* **Dropbox의 폴더 안에 문서 저장 폴더**를 두면 어디서나 맥에서 편집한 문서에 접근할 수 있다.
* **[Simplenote](http://simplenote.com/)와 동기화**할 수 있다. 태그도 동기화된다.
* **마크다운 문법을 지원한다.** 마크다운 완성 기능을 활성화하면 마크다운 글쓰기가 더 편해진다.
* 괄호와 따옴표([], (), "", '')의 **auto-pairing**을 지원한다.
* **외부 텍스트 편집기를 지원**한다. 설정에서 외부 텍스트 편집기를 지정한 후 "⌘⇧E"를 누르면 선택한 문서를 다른 편집 앱에서 열 수 있다. 나는 nvALT에서 마크다운으로 글을 작성하고 [Marked 2][7184-002]에서 글이 어떤 형식으로 보이는지 확인한다.
* **미리보기 창을 지원한다.** 외부편집기를 사용하지 않아도 마크다운으로 작성한 문서가 어떻게 보일지 확인할 수 있다.
	* HTML과 CSS를 커스터마이징 할 수 있다.
	* 미리보기에 "Pin"해두고 다른 노트를 편집할 때도 원하는 문서를 미리보기 창에서 볼 수 있다.
	* HTML 소스 탭이 있어 소스를 빠르게 복사/붙여넣을 수 있다.
* [Peggd](http://peg.gd/ "Peggd")를 통해 문서를 공유할 수 있다.
* 노트목록과 검색 필드를 접고/펼(Collapse/Expand) 수 있다.
* 스크롤바 토글이 가능하다.
* 단어 수 카운트 기능

## nvALT 기본 사용법

가장 먼저 노트를 저장할 폴더 − Dropbox 안의 폴더로 지정하면 다른 플랫폼에서의 접근성을 높일 수 있다 − 지정, 노트의 확장자와 유형 지정 등은 "⌘,"를 눌러 `환경설정 > Notes` 에서 설정할 수 있다. 외부에디터로 사용할 앱은 `환경설정 > Editing` 탭에서 지정 가능하며 그 외에 옵션 항목들과 "Fonts & Colors"도 개인이 사용하는 스타일에 맞도록 설정하면 된다.

### 노트 검색/관리

제일 위에 위치한 막대바가 검색필드이자 노트 작성의 시작이 되는 노트 제목 입력란이다. nvALT 내 어디서나 "⌘L"로 검색필드를 선택할 수 있다. 검색필드에 타이핑을 시작하면 마치 최근의 웹브라우저의 주소창처럼 검색어 자동 완성 기능이 활성화되고, 동시에 검색어 관련 노트들이 검색필드 아래에 노트목록으로 나타난다. 노트를 찾기 위해 "⌘+↑↓"으로 노트목록을 탐색할 수 있다. 원하는 노트가 선택되면 "Tab"키를 눌러 바로 편집할 수 있다.

노트의 이름을 변경하려면 "⌘R"을 눌러 변경하면 된다. 노트를 삭제하려면 "⌘⌫"을 누르면 된다.

### 새로운 노트 만들기

위에서 검색필드로 사용한 곳에 새로운 노트의 이름을 적고 리턴키를 누른다. 그리고 노트의 내용을 쓰면 된다. 노트를 작성하면 저장소로 지정한 폴더에 저절로 저장된다.

### 노트에 태그 지정하기

편집 중인 노트나 검색하여 선택한 노트에서 "⌘⇧T"를 누르면 태그를 입력할 수 있다. 자동완성 기능을 제공한다.

### 노트 즐겨찾기 이용하기

nvALT에서는 즐겨찾기(bookmark) 기능이 있다. "책갈피"라는 말이 더 어울리겠다. 원하는 노트를 즐겨찾기에 추가해두면 단축키(⌘+숫자)가 저절로 지정된다. 나중에 다른 노트를 다루다가 해당 단축키를 누르면 지정된 노트로 바로 이동할 수 있다.

nvALT 즐겨찾기 단축키는 다음과 같다.

* 노트를 즐겨찾기에 추가: ⌘⇧D
* 등록된 즐겨찾기 목록 보기: ⌘0

### 노트 미리보기

메뉴를 눌러서 접근할 수 있지만 나는 키보드 단축키를 이용한다.

* 미리보기 창 토글: ⌘\^P
* 소스 보기 토글: ⌘U
* 미리보기 창에 노트 고정: ⌥⇧⌘L
* 미리보기/PDF 프린트: ⌥⇧⌘P
* 미리보기 HTML 저장: ⇧⌘S

## 노트 작성 팁

### 북마클릿을 이용해서 노트 작성

사파리, 크롬, 파이어폭스 모든 웹브라우저에서 사용할 수 있다. 북마클릿을 즐겨찾기 막대에 끌어넣으면 바로 사용이 가능하다. 웹서핑을 하다가 노트에 넣고 싶은 페이지를 발견하면 북마클릿을 누른다. 그러면 보고 있는 웹페이지 전부가 nvALT에 새로운 노트로 저장된다. 물론 nvALT는 노트 앱이기에 이미지는 저장되지 않고 기본으로 Instapaper 모빌라이저를 사용해서 긁어 온다. 북마클릿을 수정하여 Instapaper 모빌라이저를 적용하지 않고 가져오도록 설정도 가능하다.

북마클릿은 [nvALT Bookmarklet :: think differently big](http://jots.mypopescu.com/post/8529405944/nvalt-bookmarklet) 에서 내려받을 수 있다.

### 웹브라우저 익스텐션을 사용해서 노트 작성

사파리와 크롬에서 사용할 수 있다. 선택한 링크, 텍스트나 페이지 전부를 nvALT로 옮긴다. Instapater Mobilizer 사용 여부도 선택할 수 있다.

### Keyboard Maestro Macro를 이용해서 빠른 노트 작성

[Keyboard Maestro 포럼의 글](http://forum.keyboardmaestro.com/t/sample-script-take-quick-note-with-nvalt/535/8 "Sample Script: Take Quick Note with NVAlt - Keyboard Maestro Discourse") 중 가장 마지막에 공유된 nvALT {Create New Note} 매크로가 흥미롭다. nvALT의 URL scheme을 이용해서 빠르게 노트를 작성하는 매크로다.

이 매크로를 실행하면 "2014-10-31-9:31:40 AM"처럼 "년-월-일-시간"이 제목으로 한 노트가 생성된다. "scratchx telephone call"이라는 태그도 자동으로 입력된다. 커서는 노트의 내용을 입력하는 영역에 위치하니 바로 원하는 글을 적으면 된다. 생성되는 제목의 형식이나 태그는 매크로를 받고 각자 필요에 따라 수정하면 된다. 사용해보니 매우 빠르게 메모하기 좋다. Keyboard Maestro와 nvALT를 모두 사용하는 사람이라면 한 번 받아보길 권한다.


## 맺음말

내가 맥을 사용할 때 nvALT는 거의 항상 켜져 있다. 그만큼 nvALT는 내 Maclife에 깊이 들어와 있는 앱이고 처음 접했을 때부터 지금까지 나를 실망시키지 않은 고마운 앱이다. 이 글을 읽는 당신에게도 좋은 친구가 되어줄 것이라 믿는다.



[nv]: http://brettterpstra.com/projects/nvalt/
[brett]: http://brettterpstra.com/about/
[7184-001]: http://www.hogbaysoftware.com/products/taskpaper
[7184-002]: http://marked2app.com/