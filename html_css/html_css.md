# HTML

## HTML Introduction

- HTML : Hyper Text MarKup Lnaguage 웹 문서를 표시하는 언어
  - Hyper Text : 하이퍼링크로 연결된 웹 문서 → 웹 문서(페이지)
  - MarKup Lnaguage : 표시 언어

-HTML 표시 내용

- Wep page의 contents
  - Text contents
  - Multimedia Contents : image, video, audio
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
    - taget="_blank" : 새탭열기
  - bookmark 기능
    - 목적지에 id attrbute를 사용해서 이름 지정
    - a 태그의 href 속성에 "#id"로 위치 지정
    