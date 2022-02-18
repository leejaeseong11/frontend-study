# HTML

---

## Learn the basics

https://www.w3schools.com/html/html_intro.asp

### HTML Basics 👉 [코드](https://github.com/leejaeseong11/frontend-study/tree/main/HTML/HTML%20Basics)

**Introduction**
HTML(Hyper Text Markup Language)은 웹 페이지를 만들기 위한 표준 마크업 언어이다. HTML 요소는 시작 태그, 요소의 내용, 종료 태그로 정의된다.

메모장, 텍스트 편집기로도 코드 작성이 가능하지만 VSCode를 이용해 HTML을 배운다. VSCode 설치 후 추가로 설치해두면 좋은 Extensions이 있다.

- open in browser: `option + B`를 눌러서 바로 HTML을 웹 브라우저로 띄울 수 있다.
- Prettier - Code formatter: `option + shift + f`를 눌러 코드 컨벤션을 보기 좋게 만든다.
  - File > Preferences > Settings 에서 기본 포맷터를 Prettier로 설정해주어야 한다.
  - Format On Save 옵션을 키면 저장할 때마다 포맷을 맞춰준다.

**URL Encoding**
URL은 웹 주소의 다른 단어이다.
단어 또는 IP로 구성되는데, 숫자(IP)보다는 기억하기 쉬운 이름을 사용한다.

URL의 구성은 아래와 같다.

- 체계: 인터넷 서비스의 유형(http/https)
- 접두사: 도메인 접두사(www)
- 도메인: 인터넷 도메인 이름(w3schools.com)
- 포트: 호스트의 포트 번호(기본값은 80)
- 경로: 서버의 경로(생략된 경우 사이트의 루트 디렉토리)
- 파일 이름: 문서 또는 리소스의 이름

URL은 아스키 문자 집합을 사용하여 인터넷을 통해서만 보낼 수 있다.
아스키 이외의 문자는 변환해야 한다.
URL 인코딩은 아스키가 아닌 문자를 인터넷을 통해 전송할 수 있는 형식인 16진수가 뒤따르는 "%"로 변환한다.
URL은 공백을 포함할 수 없어 공백을 더하기(+) 또는 %20으로 바꾼다.

**XHTML**
XHTML은 더 엄격한 XML 기반의 HTML 버전이다.

- EXTensible Hyper Text Markup Language를 나타낸다.
- XML 응용 프로그램으로 정의된 HTML이다.
- 모든 주요 브라우저에서 지원된다.

HTML을 다른 데이터 형식과 함께 사용할 수 있도록 확장성과 유연성을 높이기 위해 개발되었다.
브라우저는 HTML 페이지의 오류를 무시하고 마크업에 약간의 오류가 있더라도 웹 사이트를 표시하려고 하지만, XHTML은 훨씬 엄격한 오류 처리와 함께 제공된다.

HTML과의 차이는 아래와 같다.

- `<!DOCTYPE>`은 필수 항목이다.
- `<html>`의 xmlns 속성은 필수이다.
- `<html>`, `<head>`, `<title>`, `<body>` 모두 필수이다.

```html
<!DOCTYPE html>
<html xmlns="http://www.w3.org/1999/xhtml">
  <head>
    <title>Title of document</title>
  </head>
  <body>
    contents
  </body>
</html>
```

- 요소는 항상 적절하게 중첩되어야 한다.

```html
<b><i>Some text</i></b>
```

- 요소는 항상 닫혀 있어야 한다.

```html
<p>This is a paragraph</p>
<br />
```

- 요소는 항상 소문자여야 한다.

```html
<body>
  <p>Lower Case</p>
</body>
```

- 속성의 이름은 항상 소문자여야 한다.

```html
<a href="https://blog.naver.com/easeon11k">blog</a>
```

- 속성의 값은 항상 따옴표로 묶여야 한다.

```html
<a href="https://github.com/leejaeseong11/frontend-study">github</a>
```

- 속성 최소화는 금지되어 있다.

```html
<input type="checkbox" name="vehicle" value="car" checked="checked" />
```

### HTML Forms 👉 [코드](https://github.com/leejaeseong11/frontend-study/tree/main/HTML/HTML%20Basics/HTML%20Forms)

<form> 요소는 정보를 제출하기 위한 대화형 컨트롤을 포함하는 문서 구획이다.

### HTML Forms 👉 [코드](https://github.com/leejaeseong11/frontend-study/tree/main/HTML/HTML%20Basics/HTML%20Graphics)

HTML에서 그래픽을 그리기 위한 <canvas>와 vector 기반 그래픽을 나타내는 <svg>를 다룬다.

### HTML Media 👉 [코드](https://github.com/leejaeseong11/frontend-study/tree/main/HTML/HTML%20Basics/HTML%20Media)

멀티미디어는 다양한 형식으로 제공되어 이미지, 음악, 사운드, 비디오, 레코드, 영화, 애니메이션 등 듣거나 볼 수 있는 모든 것이다.
웹 페이지에는 다양한 유형과 형식의 멀티미디어가 포함되어 있다.

최초의 웹 브라우저는 단일 색상, 단일 글꼴의 텍스트만 지원했지만, 나중에 색상, 글꼴, 이미지, 멀티미디어를 지원하기 시작했다.

멀티미디어 요소는 미디어 파일에 저장된다.
파일 확장자로 파일 유형을 검사하며 .wav, .mp3, .mp4, .mpg, .wmv, .avi와 같은 형식과 확장자가 있다.

비디오 형식

- MP4, WebM, OGG형식은 HTML에서 지원된다.
- 유튜브는 MP4를 권장한다.

오디오 형식

- MP3는 압축된 녹음 음악에 적합하다.
- 웹 사이트가 녹음된 음악과 관련되어 있다면 MP3가 적합하다.
