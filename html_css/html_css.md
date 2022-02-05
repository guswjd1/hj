# HTML

## HTML Introduction

- HTML : Hyper Text MarKup Lnaguage 웹 문서를 표시하는 언어
  - Hyper Text : 하이퍼링크로 연결된 웹 문서 → 웹 문서(페이지)
  - MarKup Lnaguage : 표시 언어

-HTML 표시 내용

- Wep page의 contents
  - Text contents
  - Multimedia Contents : image, video, audio
    -Embed(ed) contents : 이미만들어진 것을 끼워넣는 컨텐츠
- Wep page의 structure

- 학습내용
  - 문법
  - 활용

## HTML Basic

- 기본구조

※ ` : backick

```
<!DOCTYPE html>
<html>
  <head>
  웹 문서의 부가정보
  </head>
  <body>
  웹 문서의 내용
  </body>
</html>
```

## HTML Element

- Tag와 contents로 구성
- Tag는 시작태그와 종료태그로 구성

  - contents와 종료태그 없이 시작태그만 있는 요소 : 빈요소(Empty Element)

  ```
  <h1>제목</h1>

  <br> → 빈요소 (Empty Element)
  ```

## HTML Attribute

- HTML Tag의 추가정보

- syntax : name="value"

```
<img src="photo.jpg" alt="사진">
```

## Text Contents Element

### Headung

- 제목
  - h1 ~ h6

### Paragraph

- P(paregraph) : 단락

- hr (Horizontal Rules) : 수평선 (단락구분)

- br(Line Break) : 강제 줄바꿈
  (※ 강제 공백(Entity code) : &nbsp; - Nun-breaking soace)
  (※ & : ampersand)
  - HTML text 줄바꿈, 공백 인식
    - 공백 1칸으로 인식

### HTML List

- 순서없는 목록 : ul, li
- 순서있는 목록 : ol, li
- 설명있는 목록 : dl, dt, dd

※ 포함관계/중첩관계 (Nested Element)

- 포함하는 요소 : 부모요소(Parent), 조상요소(Ancestor)
- 포함되는 요소 : 자식요소(Child), 자손요소(Descendant)
- 이웃하는 요소 : 형제요소(sibling)

### HTML Link

- 하이퍼링크 연결

- a(anchor)

  - href(Hypertext reference) attribute : 연결되는 페이지의 주소 정보
  - target : 새탭열기 설정
    - taget="\_blank" : 새탭열기
  - Bookmark 기능

    - 목적지에 id attrbute를 사용해서 이름 지정
    - a 태그의 href 속성에 "#id"로 위치 지정

### HTML Table

- 표를 표시
- table(표 영역 표시)
- tr (table row) : 행
- th (table heading) : 열 제목
- td (table data) : 열(칸)
- table henerrator
  https://www.tablesgenerator.com/

## Multimedia contents

### HTML image

- img : image

- attribute
  - src(source) : 이미지 파일의 경로, 이름
  - alt(altanative) : 대체 텍스트

### HTML Video

- Video tag
- attribute (name만 사용하는 형태)

  - controls : 동영상 컨트롤 버튼 표시 여부
  - autoplay : 자동 재생
  - muted : 음소거
  - loop : 반복 재생
  - poster : 영상 대체 이미지 (썸네일)

  ## Semantic Element

  - 영역을 구분하는 Element를 의미있게 사용하는 것
  - header : 로고, 로그인, 언어변경
  - nav(navigation) : 메뉴(gnb-global navigation), lnb(local navigation bar)
  - section : 웹 페이지의 본문 / 영역 구분
  - article : 웹 페이지의 본문 / 독립된 글,내용
  - aside : 부수적인 내용 / 광고, 배너
  - footer : 웹 사이트의 위치, 정보, 관련 링크
  - figure : 다이어그램 / 이미지 시각 요소
  - main :웹 페이지 본문 전체

## URL / File Path

- URL (Uniform Resource Locator)

```
https://www.naver.com/video/movie.mp4

=> https://도메인이름/상세경로:포트번호

IP 주소 : Internet Potocol 주소 => 인터넷에서 사용하는 실제 주소

Ex) 192.168.0.1 : 0~255까지의 숫자 4개로 구성

도메인 네임 : 영어단어(줄임말)로 구성되어 있는 식별 이름
도메인 네임 서버(시스템) : 도메인 네임 => IP주소로 변환

```

- 경로(URL/File Path) 지정 방식
  - root : 해당 경로의 가장 시작 위치
  - 절대 경로
    - 파일 경로의 전체 URL을 표현하는 방식
  - 상대 경로
    - 현재 페이지를 기준으로 일부 URL을 표현하는 방식
    - root 상대 경로 방식 : root를 기준으로 상대적인 URL 표현

```

domain : www.abc.com

/(root) - html -index.html
        - images - photo.jpg

절대 방식 : http://www.abc.com/images/photo.jpg (어느위치에서도 찾아올 수 있음)

상대 방식 (현재페이지 : index.html) : ../images/photo.jpg
(주소가 짧으나 기준에 따라 주소가 달라짐)

root 상대방식 : /images/photo.jpg

```

## HTML Head

-head element

- title : 웹사이트 제목 (브라우저 탭에 표시)
- meta : 웹사이트 관련 정보
- link : css 파일 불러오기
- style : css 코드 작성
- script : js 코드 작성 / 파일 불러오기

- meta

  - charset (character set) : 문자 세트 - 글자(문자)를 표시하는 방식
  - 종류/개수 → 용량

    - bit : 0 또는 1 이 저장되는 공간
    - 1 bit가 저장/표현할 수 있는 개수(가짓수) : 2
    - 2 _ 2 _ 2 \* 2 : 4 bit → 16개
    - 1 byte = 8 bit → 256개(0~255) (bit < KB < MB < TB < PB ...)

  - UTF-8 : 문자 표기 방식 중 하나
    Universal Coded Character Set + Transformation Format – 8-bit
