# NanumSquare

> 반듯한 직선으로 제목에 잘 어울리며 모바일에서도 잘 보이는 글꼴입니다. 꼭 필요한 2,350자만을 추려 용량을 가볍게 줄였고 웹 환경에서 보다 편리하게 사용 가능합니다. http://hangeul.naver.com/2016/nanum

나눔스퀘어의 미싱 글리프 문제를 수정한 폰트입니다. 이 레포지토리는 [moonspam/NanumSquare](https://github.com/moonspam/NanumSquare)의 fork입니다.

## 어떤 것이 달라졌나요?
나눔스퀘어는 한글 상용글자 2350자, 알파벳, 숫자 및 일부 특수문자만 포함된 폰트입니다. 예를 들어 "샽"과 같은 글자는 포함되어 있지 않습니다. 이렇게 포함되지 않은 글자를 missing glyth라고 칭합니다.
하지만 기존 나눔스퀘어 폰트는 missing glyth가 없는 문제가 아니라 빈 문자로 들어있기 때문에 css등에서 대체 폰트를 지정해도 "샽"과 같은 문제가 그대로 빈 문자로 노출되는 문제가 있습니다.

이 레포지토리는 기존 나눔스퀘어 폰트에서 필요한 문자를 제외한 나머지 빈 문자를 없는 문자로 수정하여 프로그래머가 css 작성시 의도한 대체 폰트를 사용할 수 있도록 도와줍니다.

## 옵션

Regular(400), Bold(700), Extra Bold(800), Light(300) 지원됩니다.

## 사용방법

### link 방식 (권장)

    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/Chanki-Min/NanumSquare@1.1/nanumsquare.css">

### import 방식

    @import url(https://cdn.jsdelivr.net/gh/Chanki-Min/NanumSquare@1.1/nanumsquare.css);

## 적용

### css (예)

    body		{ font-family: 'NanumSquare', sans-serif; }
    .normal		{ font-weight: 400 }
    .bold		{ font-weight: 700 }
    .bolder		{ font-weight: 800 }
    .light		{ font-weight: 300 }
