# Markdown記法 チートシート<!-- omit from toc -->

- [Block Elements](#block-elements)
  - [Headers](#headers)
    - [Atx-style](#atx-style)
    - [Setext-style](#setext-style)
  - [Blockquotes](#blockquotes)
    - [blockquote-in-a-blockquote](#blockquote-in-a-blockquote)
  - [Lists](#lists)
    - [順序なしリスト](#順序なしリスト)
    - [順序付きリスト](#順序付きリスト)
  - [Code Blocks](#code-blocks)
    - [Inline code](#inline-code)
    - [Blocks code](#blocks-code)
  - [Code and Syntax Highlighting](#code-and-syntax-highlighting)
  - [Tables](#tables)
  - [Horizontal Rules](#horizontal-rules)
- [Span Elements](#span-elements)
  - [Links](#links)
    - [インラインスタイル](#インラインスタイル)
    - [タイトル属性付与](#タイトル属性付与)
    - [参照スタイル](#参照スタイル)
    - [title属性を次の行に記述](#title属性を次の行に記述)
  - [Emphasis](#emphasis)
    - [em](#em)
    - [strong](#strong)
  - [Images](#images)
    - [インラインスタイル](#インラインスタイル-1)
    - [title属性付与](#title属性付与)
    - [参照スタイル](#参照スタイル-1)
    - [サイズ指定](#サイズ指定)

## Block Elements
### Headers
#### Atx-style
```md
# This is an H1
## This is an H2
### This is an H3
#### This is an H4
##### This is an H5
###### This is an H6
```

# This is an H1<!-- omit from toc -->
## This is an H2<!-- omit from toc -->
### This is an H3<!-- omit from toc -->
#### This is an H4<!-- omit from toc -->
##### This is an H5<!-- omit from toc -->
###### This is an H6<!-- omit from toc -->

#### Setext-style
```md
This is an H1
=

This is an H2
-
```
<!-- omit from toc -->
This is an H1
=

<!-- omit from toc -->
This is an H2
-

### Blockquotes
```md
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
```
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

#### blockquote-in-a-blockquote
```md
> This is the first level of quoting.
> > This is nested blockquote.
> Back to the first level.
```
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

### Lists
#### 順序なしリスト
```md
* red
* green
* blue
```
* red
* green
* blue
```md
+ red
+ green
+ blue
```
+ red
+ green
+ blue
```md
- red
- green
- blue
```
- red
- green
- blue

#### 順序付きリスト
```md
1. red
2. green
3. blue
```
1. red
2. green
3. blue

### Code Blocks
#### Inline code
```md
Inline `code` has `back-ticks around` it.
```
Inline `code` has `back-ticks around` it.

#### Blocks code
- ４つのスペースか１つのタブインデントを入れる
```md
This is a normal paragraph:

    start code
      code
    end code
```
This is a normal paragraph:

    start code
      code
    end code

### Code and Syntax Highlighting
- ３つのバックティック
- コードブロックを入れ子にするにはインデントを増やす
```md
    ```javascript
    var s = "JavaScript syntax highlighting";
    alert(s);
    ```
```
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
- [ハイライトのデモ](http://softwaremaniacs.org/media/soft/highlight/test.html)

### Tables
```md
| Tables          |  products  | price |
| --------------- | :--------: | ----: |
| col 1 is Left   |  Desktop   | $1600 |
| col 2 is Center |   Laptop   |    $1 |
| col 3 is Right  | smartphone |   $12 |
```

| Tables          |  products  | price |
| --------------- | :--------: | ----: |
| col 1 is Left   |  Desktop   | $1600 |
| col 2 is Center |   Laptop   |    $1 |
| col 3 is Right  | smartphone |   $12 |

- インラインマークダウンを使用することができる
```md
Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```
Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3

### Horizontal Rules
```md
***
* * *
---
- - - 
```
***
* * *
---
- - - 

## Span Elements
### Links
#### インラインスタイル
```md
[This link](https://example.net/) has no title attribute.
```
[This link](https://example.net/) has no title attribute.

#### タイトル属性付与
```md
This is [an example](https://example.com/ "Title") inline link.
```
This is [an example](https://example.com/ "Title") inline link.

#### 参照スタイル
```md
This is [an example][id] reference-style link.

[id]: https://example.com/  "Optional Title Here"
```
This is [an example][id] reference-style link.

[id]: https://example.com/  "Optional Title Here"

#### title属性を次の行に記述
```md
This is [an example][id2] reference-style link.

[id2]: https://example.com/longish/path/to/resource/here
    "Optional Title Here"
```
This is [an example][id2] reference-style link.

[id2]: https://example.com/longish/path/to/resource/here
"Optional Title Here"
    
```md
[Link To Google][1]  
[Link To Github][2]  
[Link To Cloudflare][3]  

[1]: https://google.com/     "Link to Google"
[2]: https://github.co.jp/   "Link to Github"
[3]: https://cloudflare.com/ "Link to Cloudflare"
```
[Link To Google][1]  
[Link To Github][2]  
[Link To Cloudflare][3]  

[1]: https://google.com/     "Link to Google"
[2]: https://github.co.jp/   "Link to Github"
[3]: https://cloudflare.com/ "Link to Cloudflare"

### Emphasis
#### em
```md
*single asterisks*

_single underscores_
```
*single asterisks*

_single underscores_

#### strong
```md
**double asterisks**

__double underscores__
```
**double asterisks**

__double underscores__

### Images
#### インラインスタイル
```md
![Alt text](/path/to/img.jpg)
```
![Alt text](./image/image-1.jpg)

#### title属性付与
```md
![Alt text](/path/to/img.jpg "Optional title")
```
![Alt text](./image/image-1.jpg "Optional title")

#### 参照スタイル
```md
![Alt text][image-id-1]

[image-id-1]: /path/to/img.jpg
```

![Alt text][image-id-2]

[image-id-2]: ./image/image-1.jpg

#### サイズ指定
```md
<img width=200 src="/path/to/img.jpg">
```
<img width=200 src="./image/image-1.jpg">