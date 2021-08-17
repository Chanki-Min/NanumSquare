# NanumSquare_MissingGlyphsFix

> 반듯한 직선으로 제목에 잘 어울리며 모바일에서도 잘 보이는 글꼴입니다. 꼭 필요한 2,350자만을 추려 용량을 가볍게 줄였고 웹 환경에서 보다 편리하게 사용 가능합니다. http://hangeul.naver.com/2016/nanum

나눔스퀘어의 미싱 글리프 문제를 수정한 폰트입니다. 이 레포지토리는 [moonspam/NanumSquare](https://github.com/moonspam/NanumSquare)의 fork입니다.


## 어떤 것이 달라졌나요?

나눔스퀘어는 한글 상용글자 2350자, 알파벳, 숫자 및 일부 특수문자만 포함된 폰트입니다. 예를 들어 "샽"과 같은 글자는 포함되어 있지 않습니다. 이렇게 포함되지 않은 글자를 missing glyph라고 칭합니다.
하지만 기존 나눔스퀘어 폰트는 missing glyph가 null 문자가 아니라 공백 문자로 들어있기 때문에 css등에서 대체 폰트를 지정해도 "샽"과 같은 문제가 공백으로 노출되는 문제가 있습니다.

이 레포지토리는 기존 나눔스퀘어 폰트에서 필요한 문자를 제외한 나머지 빈 문자를 null 문자로 수정하여 프로그래머가 css 작성시 의도한 대체 폰트를 사용할 수 있도록 도와줍니다.


## 어떤 글자들을 지원하나요?

지원하는 글자들의 리스트는 [glyphs.txt](https://github.com/Chanki-Min/NanumSquare/blob/master/glyphs.txt) 파일에서 확인해보실 수 있습니다.

## 옵션

Regular(400), Bold(700), Extra Bold(800), Light(300)가 지원됩니다.

## 사용방법

### link 방식 (권장)

    <link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/gh/Chanki-Min/NanumSquare@1.3/nanumsquare.css">

### import 방식

    @import url(https://cdn.jsdelivr.net/gh/Chanki-Min/NanumSquare@1.3/nanumsquare.css);

## 적용

### css (예)

    body		{ font-family: 'NanumSquare', sans-serif; }
    .normal		{ font-weight: 400 }
    .bold		{ font-weight: 700 }
    .bolder		{ font-weight: 800 }
    .light		{ font-weight: 300 }
    
## Licence
이 폰트는 네이버에서 제공한 나눔글꼴이 적용되어 있습니다.

Copyright (c) 2010, NAVER Corporation (https://www.navercorp.com/),



with Reserved Font Name Nanum, Naver Nanum, NanumGothic, Naver NanumGothic, NanumMyeongjo, Naver NanumMyeongjo, NanumBrush, Naver NanumBrush, NanumPen, Naver NanumPen, Naver NanumGothicEco, NanumGothicEco, Naver NanumMyeongjoEco, NanumMyeongjoEco, Naver NanumGothicLight, NanumGothicLight, NanumBarunGothic, Naver NanumBarunGothic, NanumSquareRound, NanumBarunPen, MaruBuri



This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at: http://scripts.sil.org/OFL



SIL OPEN FONT LICENSE
Version 1.1 - 26 February 2007 


PREAMBLE
The goals of the Open Font License (OFL) are to stimulate worldwide
development of collaborative font projects, to support the font creation
efforts of academic and linguistic communities, and to provide a free and
open framework in which fonts may be shared and improved in partnership
with others.

The OFL allows the licensed fonts to be used, studied, modified and
redistributed freely as long as they are not sold by themselves. The
fonts, including any derivative works, can be bundled, embedded,
redistributed and/or sold with any software provided that any reserved
names are not used by derivative works. The fonts and derivatives,
however, cannot be released under any other type of license. The
requirement for fonts to remain under this license does not apply
to any document created using the fonts or their derivatives.


DEFINITIONS
"Font Software" refers to the set of files released by the Copyright
Holder(s) under this license and clearly marked as such. This may
include source files, build scripts and documentation.

"Reserved Font Name" refers to any names specified as such after the
copyright statement(s).

"Original Version" refers to the collection of Font Software components as
distributed by the Copyright Holder(s).

"Modified Version" refers to any derivative made by adding to, deleting,
or substituting - in part or in whole - any of the components of the
Original Version, by changing formats or by porting the Font Software to a
new environment.

"Author" refers to any designer, engineer, programmer, technical
writer or other person who contributed to the Font Software.


PERMISSION & CONDITIONS
Permission is hereby granted, free of charge, to any person obtaining
a copy of the Font Software, to use, study, copy, merge, embed, modify,
redistribute, and sell modified and unmodified copies of the Font
Software, subject to the following conditions:

1) Neither the Font Software nor any of its individual components,
in Original or Modified Versions, may be sold by itself.

2) Original or Modified Versions of the Font Software may be bundled,
redistributed and/or sold with any software, provided that each copy
contains the above copyright notice and this license. These can be
included either as stand-alone text files, human-readable headers or
in the appropriate machine-readable metadata fields within text or
binary files as long as those fields can be easily viewed by the user.

3) No Modified Version of the Font Software may use the Reserved Font
Name(s) unless explicit written permission is granted by the corresponding
Copyright Holder. This restriction only applies to the primary font name as
presented to the users.

4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
Software shall not be used to promote, endorse or advertise any
Modified Version, except to acknowledge the contribution(s) of the
Copyright Holder(s) and the Author(s) or with their explicit written
permission.

5) The Font Software, modified or unmodified, in part or in whole,
must be distributed entirely under this license, and must not be
distributed under any other license. The requirement for fonts to
remain under this license does not apply to any document created
using the Font Software.


TERMINATION
This license becomes null and void if any of the above conditions are
not met.


DISCLAIMER
THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
OTHER DEALINGS IN THE FONT SOFTWARE.
