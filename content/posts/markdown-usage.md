+++
title = "마크다운 사용법"
date = "2020-12-07T13:29:23+09:00"
author = ""
authorTwitter = "c1t1d0s7" #do not include @
cover = ""
tags = ["markdown"]
keywords = ["", ""]
description = ""
showFullContent = false
+++

마크다운(Markdown) 사용법
========================

## 마크다운 이란?  
**마크다운**은 글에 쉽게 서식을 지정할 수 있는 문법이다.

마크다운(Markdown)은 마크업(Markup)언어로 존 그루버(John Gruber)에 의해 디자인 되었으며 메일에서 글쓰기 형식에서 영감을 받아 만들어 졌으며 자신의 블로그에 마크다운 문법 소개와 함께 python으로 만든 마크다운을 html로 변환하는 변환기를 올림으써 알려지게 되었다. 실제 마크다운 문서에 html 테크를 사용할 수 있다. 마크다운은 html, pdf등 다른 형태의 문서로도 쉽게 변환이 가능하다.

존 그루버가 문법을 제시한 이후 각 커뮤니터에서 발전시켜 확장 문법등 새로운 문법을 제공하고 있다.

마크다운이 각광받기 시작한 이유는 GitHub의 저장소(Repository)에 관한 정보 및 사용법을 제공하기 위해 README.md를 사용하면서 부터이다.

마크다운은 웹에서 텍스트의 스타일을 지정하는 방법이다. 문서의 표현을 제어하며, 글자를 굵게 또는 기울임 꼴로 지정하고, 이미지 추가, 목록, 표를 만드는 작업 등을 쉽게 할 수 있다.
대부분의 마크다운은 # 또는 * 등 특수문자를 이용하여 표현한다.

마크다운 파일의 확장자는 `.md` 또는 `.markdown`을 사용한다.

> 참고  
> [markdownguide.org](https://www.markdownguide.org)

> 참고  
> 이 문서 또한 마크다운으로 작성되었다.
---

## 기본 문법(Basic Syntax)  
존 그루버가 마크다운 디자인 문서에 요약 된 요소들의 문법

### 1. 제목(Headers)  
제목을 만들기 위해 글자 앞에 # 기호를 사용한다.
##### - 마크다운  
```txt
# Header Level 1
## Header Level 2
### Header Level 3
#### Header Level 4
##### Header Level 5
###### Header Level 6
```
```txt
Header Level1
==============
Header Level2
--------------
```
##### - HTML  
```html
<h1>Header Level 1<h1>
<h2>Header Level 2<h2>
<h3>Header Level 3<h3>
<h4>Header Level 4<h4>
<h5>Header Level 5<h5>
<h6>Header Level 6<h6>
```
##### - 렌더링된 출력  
# Header Level 1  
## Header Level 2  
### Header Level 3  
#### Header Level 4  
##### Header Level 5  
###### Header Level 6  

### 2. 단락(Paragraphs)  
단락을 만들때는 하나 이상의 공백줄을 사용한다. 공백이나 탭을 들여쓰기는 지원하지 않는다.
##### - 마크다운  
```txt
I really like using markdown.

I think I'll use it to format all of my documents from now on.
```
##### - HTML  
```html
<p>I really like using markdown.</p>

<p>I think I'll use it to format all of my documents from now on.</p>
```
##### - 렌더링된 출력  
I really like using markdown.

I think I'll use it to format all of my documents from now on.

### 3. 줄 바꿈(Line Breaker)  
줄 바꿈 \<br\>을 하려면 줄 끝에 두칸 이상의 공백을 두고 엔터를 합니다.  
#### - 마크다운  
```txt
This is the first line.  <<-공백 두칸
And this is the second line.
```
#### - HTML  
```html
<p>This is the first line.<br>
And this is the second line.</p>
```
#### - 렌더링된 출력  
This is the first line.  
And this is the second line.

### 4. 강조(Emphasis)  
### 4-1. 기울임꼴(Italic)  
#### - 마크다운  
```txt
Italicized text is the *cat's meow*.
Italicized text is the _cat's meow_.
A*cat*meow
```
#### - HTML  
```html
Italicized text is the <em>cat's meow</em>.
Italicized text is the <em>cat's meow</em>.
A<em>cat</em>meow
```
#### - 렌더링된 출력  
Italicized text is the *cat's meow*.  
Italicized text is the _cat's meow_.  
A*cat*meow  

### 4-2. 볼드체(Bold)  
#### - 마크다운  
```txt
I just love **bold text**.
I just love __bold text__.
Love**is**bold
```
#### - HTML  
```html
I just love <strong>bold text</strong>.
I just love <strong>bold text</strong>.
Love<strong>is</strong>bold
```
#### - 렌더링된 출력    
I just love **bold text**.  
I just love __bold text__.  
Love**is**bold  

### 4-3. 볼드와 기울림꼴(Bold and Italic)  
#### - 마크다운  
```txt
This text is ***really important***.
This text is ___really important___.
This text is __*really important*__.
This text is **_really important_**.
```
#### - HTML  
```html
This text is <strong><em>really important</em></strong>.
This text is <strong><em>really important</em></strong>.
This text is <strong><em>really important</em></strong>.
This text is <strong><em>really important</em></strong>.
```
#### - 렌더링된 출력  
This text is ***really important***.  
This text is ___really important___.  
This text is __*really important*__.  
This text is **_really important_**.  

### 4-4. 인용문(Blockquotes)  
#### - 마크다운  
```txt
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```
#### - 렌더링된 출력  
> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 4-5. 중첩 인용문(Nested Blockquotes)  
#### - 마크다운  
```txt
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```
#### - 렌더링된 출력  
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

### 4-6. 다른 요소와 인용문(Blockquotes with Other Elements)  
#### - 마크다운  
```txt
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.
```
#### - 렌더링된 출력  
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.  

### 5. 목록(Lists)  
### 5-1. 순서 목록(Ordered Lists)  
#### - 마크다운  
```txt
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item
```
#### - HTML  
```html
<ol>
<li>First item</li>
<li>Second item</li>
<li>Third item
<ol>
<li>Indented item</li>
<li>Indented item</li>
</ol>
</li>
<li>Fourth item</li>
</ol>
```
#### - 렌더링된 출력  
1. First item
2. Second item
3. Third item
    1. Indented item
    2. Indented item
4. Fourth item

### 5-2. 비순서 목록(Unordered Lists)  
#### - 마크다운  
```txt
+ First item
* Second item
- Third item
    - Indented item
    - Indented item
+ Fourth item
```
#### - HTML  
```html
<ul>
<li>First item</li>
<li>Second item</li>
<li>Third item
<ul>
<li>Indented item</li>
<li>Indented item</li>
</ul>
</li>
<li>Fourth item</li>
</ul>
```
#### - 렌더링된 출력  
+ First item
* Second item
- Third item
    - Indented item
    - Indented item
+ Fourth item

### 5-3. 목록에 요소 추가(Adding Elements in Lists)  
목록을 계속 유지하면서 목록안에 다른 요소를 추가하려면 공백 4칸 또는 탭으로 들여쓰기를 한다.

### 5-3-1. 단락(Paragraphs)  
#### - 마크다운  
```txt
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.
```
#### - 렌더링된 출력  
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

### 5-3-2. 인용문(Blockquotes)  
#### - 마크다운  
```txt
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.
```
#### - 렌더링된 출력  
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.

### 5-3-4. 코드 블록(Code Blocks)  
#### - 마크다운  
```txt
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3.  Update the title to match the name of your website.
```
#### - 렌더링된 출력  
1.  Open the file.
2.  Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>
        </html>

3.  Update the title to match the name of your website.

### 5-3-5. 이미지(Images)  
#### - 마크다운  
```txt
1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](/img/tux.png)

3.  Close the file.
```
#### - 렌더링된 출력  
1.  Open the file containing the Linux mascot.
2.  Marvel at its beauty.

    ![Tux, the Linux mascot](/img/tux.png)

3.  Close the file.

### 6. 코드(Code)  
단어나 문장을 코드로 나타내려면 백틱(backtick, `)으로 단어나 문장을 묶는다.
#### - 마크다운  
```txt
At the command prompt, type `nano`.
```
#### - HTML  
```html
At the command prompt, type <code>nano</code>.
```
#### - 렌더링된 출력  
At the command prompt, type `nano`.

### 7. 코드 블록(Code Blocks) {#basic_code_block}  
코드 블록을 작성하려면 블록의 모든 행을 4칸 또는 탭으로 들여쓰기 한다.
> 참고  
> 기본 문법의 코드 블록은 사용이 불편하다. 펜스된 코드 블록은 [확장 문법의 펜스된 코드 블록](#fence_code_block)을 참고한다.

#### - 마크다운  
```txt
    <html>
      <head>
      </head>
    </html>
```
#### - 렌더링된 출력  

    <html>
      <head>
      </head>
    </html>

### 8. 수평줄(Horizontal Rules)  
수평줄을 만들려면 한줄에 3개 이상의 아스테리스크(*), 대시(-), 언더스코어(_)를 사용한다.
#### - 마크다운  
```txt
***
----
_____
```
#### - 렌더링된 출력  
세가지 방식다 아래와 같이 표현된다.
***

### 9. 링크(Links) {#basic_links}  
링크를 만들려면 대괄호([])를 사용하여 이름을 지정하고 URL 링크를 지정할 수 있다. 단순 URL 주소가 보이는 링크는 [확장 문법의 자동 URL 링크](#auto_url_links)를 참조한다.
#### - 마크다운  
```txt
[Duck Duck Go](https://duckduckgo.com).
[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").
```
#### - 렌더링된 출력  
[Duck Duck Go](https://duckduckgo.com).  
[Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").  

### 10. URL 및 Email 주소(URL and Email Address)  
#### - 마크다운  
```txt
<https://www.markdownguide.org>
<fake@example.com>
```
#### - 렌더링된 출력  
<https://www.markdownguide.org>
<fake@example.com>

### 11. 이미지(Images)  
#### - 마크다운  
```txt
![Tux, the Linux mascot](/img/tux.png)
```
#### - 렌더링된 출력  
![Tux, the Linux mascot](/img/tux.png)

### 11-1. 링크된 이미지(Linking Images)  
#### - 마크다운  
```txt
[![Tux, the Linux mascot](/img/tux.png "Tux, as originally drawn as raster image by Larry Ewing in 1996.")](https://upload.wikimedia.org/wikipedia/commons/a/af/Tux.png)
```
#### - 렌더링된 출력  
[![Tux, the Linux mascot](/img/tux.png "Tux, as originally drawn as raster image by Larry Ewing in 1996.")](https://upload.wikimedia.org/wikipedia/commons/a/af/Tux.png)

### 12. 탈출 문자(Escaping Characters)  
마크다운에서 서식을 지정하는데 사용되는 특수문자를 백슬레쉬(\\)를 이용하여 글자 그대로 표현할 수 있다.  
#### - 마크다운  
```txt
\* Without the backslash, this would be a bullet in an unordered list.
```
#### - 렌더링된 출력  
\* Without the backslash, this would be a bullet in an unordered list.
> 참고  
> 마크다운 서식을 지정하는 특수문자 
> \\ \` \* \_ \{} \[] \() \# \+ \- \. !

---

## 확장 문법(Extended Syntax)  
존 그루버가 디자인한 기본 구문이외 테이블, 코드블록, 구문 강조, URL 자동 링크 등 필요한 많은 요소를 확장 문법에서 제공한다. 이러한 확장 문법을 사용하기 위해서는 기본 마크다운 문법을 기반으로하는 **경량 마크업 랭귀지**를 사용하거나, 호환되는 마크다운 프로세스에 **확장기능**을 추가하여 사용할 수 있습니다.  

확장 문법은 모든 마크다운 어플리케이션이 지원하는 것은 아니며, 어플리케이션에서 사용되는 경량 마크업 랭귀지가 확장 문법을 지원하는지 여부를 확인해야한다.  

* 경량 마크업 랭귀지(Lightweight Markup Languages)  
  [CommonMark](http://commonmark.org/)  
  [GitHub Flavored Markdown(GFM)](https://github.github.com/gfm/)  
  [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/)  
  [MultiMarkdown](http://fletcherpenney.net/multimarkdown/)  

### 1. 테이블(Tables)  
테이블을 추가하려면 3개이상의 하이픈(---)을 사용하고, 각 열은 파이프(|)를 사용한다.

> 참고  
> [마크다운 테이블 생성기](http://www.tablesgenerator.com/markdown_tables)

#### - 마크다운  
```txt
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
```
#### - 렌더링된 출력  
| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

### 1-1. 정렬(Alignment)  
#### - 마크다운  
```txt
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |
```
#### - 렌더링된 출력  
| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

### 1-2. 테이블 내에서 서식 지정  
*링크, 코드, 강조*를 추가할 수 있다.  
*제목, 인용문, 목록, 수평줄, 이미지, HTML 태그*는 추가할 수 없다.  

### 1-3. 테이블에서 파이프 문자 사용하기  
테이블에서 파이프 문자는 HTML 문자 코드인 `&#124;`로 표현할 수 있다.  

### 2. 펜스된 코드 블록(Fenced Code Blocks) {#fence_code_block}  
[기본 문법의 코드 블록](#basic_code_block)은 4칸 또는 탭으로 들여쓰기 해야한다.
확장 문법에서는 3개의 백틱(```) 또는 3개의 딜데(~~~)를 사용하여 코드 앞줄과 뒷줄을 감싼다.  
#### - 마크다운  
>\```
>{
>  "firstName": "John",
>  "lastName": "Smith",
>  "age": 25
>}
>\```

#### - 렌더링된 출력  
```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### 2-1. 문법 강조(Syntax Highlighting)  
3개의 백틱(```) 뒤에 랭귀지를 지정하면 각 언어마다의 문법을 강조할 수 있다.  
#### - 마크다운
>\```json
>{
>  "firstName": "John",
>  "lastName": "Smith",
>  "age": 25
>}
>\```
#### - 렌더링된 출력  
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### 3. 각주(Footnotes)  
각주를 사용하면 문서 본문을 어지럽히지 않고 노트나 참조를 추가할 수 있다. 각주 참조는 링크가 있는 첨자 번호로 나타나며, 링크를 누르면 페이지 하단의 각주 내용으로 이동할 수 있다.  
#### - 마크다운  
```txt
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.
```
#### - 렌더링된 출력  
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the first footnote.

[^bignote]: Here's one with multiple paragraphs and code.

    Indent paragraphs to include them in the footnote.

    `{ my code }`

    Add as many paragraphs as you like.

### 4. 제목 ID(Heading ID)  
많은 마크다운 프로세서는 마크다운에서 제목(Header)에 대한 사용자 지정 ID를 사용할 수 있다.
#### - 마크다운  
```txt
### My Great Heading {#custom-id}
```
#### - HTML  
```html
<h3 id="custom-id">My Great Heading</h3>
```
#### - 렌더링된 출력  
### My Great Heading {#custom-id}  

### 4-1. 제목 ID 링크(Linking to Heading ID)  
사용자 지정 ID에 링크를 연결할 수 있다.  
#### - 마크다운  
```txt
[Heading IDs](#custom-id)
```
#### - HTML  
```html
<a href="#custom-id">Heading IDs</a>
```
#### - 렌더링된 출력  
[Heading IDs](#custom-id)  
> 참고  
> 위 링크를 누르면 "My Great Heading" 텍스트가 있는 줄로 이동한다.  

### 5. 정의 목록(Definition Lists)  
용어에 대한 정의 및 정의 목록을 작성할 수 있다.
#### - 마크다운  
```txt
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```
#### - HTML  
```html
<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term. </dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```
#### - 렌더링된 출력  
First Term  
: This is the definition of the first term.  

Second Term  
: This is one definition of the second term.  
: This is another definition of the second term.  

### 6. 취소선(Strikethrough)  
#### - 마크다운  
```txt
~~The world is flat.~~ We now know that the world is round.
```
#### - 렌더링된 출력  
~~The world is flat.~~ We now know that the world is round.

### 7. 작업 목록  
작업 목록을 사용하면 확인란이 있는 목록을 만들 수 있다.  
#### - 마크다운  
```txt
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```
#### - 렌더링된 출력  
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

### 8. 자동 URL 링크(Automatic URL Linking) {#auto_url_links}  
[기본 문법의 링크](#basic_links) 처럼 괄호([])를 사용하지 않아도 마크다운 프로세스는 자동으로 URL를 링크로 변환한다.  
#### - 마크다운  
```txt
http://www.example.com
```
#### - 렌더링된 출력  
http://www.example.com

### 8-1. 자동 URL 링크 비활성화(Disabling Automatic URL Linking)  
URL 주소를 자동으로 링크하지 않으려면 백틱(\`)으로 URL 주소를 감싼다.  
#### - 마크다운  
```txt
`http://www.example.com`
```
#### - 렌더링된 출력  
`http://www.example.com`
