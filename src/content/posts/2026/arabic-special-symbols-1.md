---
title: 特殊的阿拉伯文Unicode符号一览（1）
published: 2026-08-21
category: Unicode探索
tags: 
- 语言
- Unicode
---

:::note
截止目前（2026年2月24日），很多阿拉伯文字体对于阿拉伯文区块的覆盖率不高，因此文中会出现字符无法显示的情况。
为防止某些结合字符无法正常显示，这些字符会加上◌字符。
:::

文章内容以Unicode 17.0为准，阿拉伯字母包含7个区块：

* 基本阿拉伯文
* 阿拉伯文补充
* 阿拉伯文拓展A、B和C
* 阿拉伯文表现形式A、B

## ؀
名称：`ARABIC NUMBER SIGN`

控制字符，属于“下方标记”子区块。在阿拉伯文早期编码中作为数字起始标记使用。现已弃用。当字符书写方向为右至左时就会以特殊方式渲染。如：؀۱۲۳۴

## ؁
名称：`ARABIC SIGN SAHAH`

下方标记，标记年份开始。与前面的字符同样有特殊渲染方式：؁۱۲۳۴

## ؃
名称：`ARABIC SIGN SAFHA`

下方标记，是数字标记的一个变体，用于标记页码。

## ؄
名称：`ARABIC SIGN SAMVAT`

日期下方标记的一个变体，外观来源于其名称Samvat（سموت），在乌尔都语中使用。

## ؅
名称：`ARABIC NUMBER MARK ABOVE`

上方标记，为数字标记的一个变体，用于标记阿拉伯文中的科普特数字。

## ؈
名称：`ARABIC RAY`

数学符号，表示圆的半径。

## ؋
名称：`AFGHANI SIGN`

阿富汗货币阿富汗尼的符号。

## ،؛؟
名称：

* `ARABIC COMMA`
* `ARABIC SEMICOLON`
* `ARABIC QUESTION MARK`

分别为阿拉伯语中的逗号，分号和问号。实际上，除了阿拉伯文之外，叙利亚文和塔纳文也使用这些标点符号。

## ؍
名称：`ARABIC DATE SEPARATOR`

在巴基斯坦和印度使用的日期分隔符号，写在月与日之间。

## ؎
名称：`ARABIC POETIC VERSE SIGN`

阿拉伯文诗歌符号，表示诗歌的开始。

## ؏
名称：`ARABIC SIGN MISRA`

乌尔都语散文使用的符号，表示下文内容为诗歌。[^2]

## ٭
名称：`ARABIC FIVE POINTED STAR`

阿拉伯文中的星号。

## ﷺ ◌ؐ
名称：

* `ARABIC LIGATURE SALLALLAHOU ALAYHE WASALLAM`
* `ARABIC SIGN SALLALLAHOU ALAYHE WASSALLAM`

两个阿拉伯文尊称符号。第一个字符是阿拉伯语连字，将其进行NFKC分解得到：

> صلى الله عليه وسلم

这是一句清真言，意思为“愿真主赐福他并使他平安”。第二个字符则是这个清真言的缩写，作为附加符号附加在人名上，通常是先知穆罕默德的名字。

## ﵇﵈﵉﵍ ◌ؑ
名称：

* `ARABIC LIGATURE ALAYHI AS-SALAAM`
* `ARABIC LIGATURE ALAYHIM AS-SALAAM`
* `ARABIC LIGATURE ALAYHIMAA AS-SALAAM`
* `ARABIC LIGATURE ALAYHAA AS-SALAAM`
* `ARABIC SIGN ALAYHE ASSALLAM`

前四个连字分别代表的文字是：

* عليه السلام
* عليهم السلام
* عليهما السلام
* عليها السلام

这四句话都是清真言，意思都是“愿主赐其平安”，但人称不同。这四句话的适用对象分别是单个男性，多个人，两个人，单个女性。

最后一个尊称附加符号是这句清真言的缩写，通常附加在其他先知或天使的名字上。

## ﵀﵏﯉ ◌ؒ
名称：

* `ARABIC LIGATURE RAHIMAHU ALLAAH`
* `ARABIC LIGATURE RAHIMAHUM ALLAAH`
* `ARABIC LIGATURE RAHIMAHUMAA ALLAAH`
* `ARABIC SIGN RAHMATULLAH ALAYHE`

前三个连字所代表的文字分别是：

*  رحمه الله
* رحمهم الله
* رحمهما الله

它们的意思都是“愿真主怜悯他”，但对象分别为单数男性，多个男性，两个男性。

最后一个尊称附加符号是这句清真言的缩写，通常附加在殉道者或圣人的名字后面。

## ﵁﵂﵃﵄﵅ ◌ؓ
名称：

* `ARABIC LIGATURE RADI ALLAAHU ANH`
* `ARABIC LIGATURE RADI ALLAAHU ANHAA`
* `ARABIC LIGATURE RADI ALLAAHU ANHUM`
* `ARABIC LIGATURE RADI ALLAAHU ANHUMAA`
* `ARABIC LIGATURE RADI ALLAAHU ANHUNNA`
* `ARABIC SIGN RADI ALLAHOU ANHU`

前五个连字所代表的文字分别是：

* رَضِيَ اللَّهُ عَنْهُ
* رَضِيَ اللَّهُ عَنْهَا
* رَضِيَ اللَّهُ عَنْهُمْ
* رَضِيَ اللَّهُ عَنْهُمَا
* رَضِيَ اللَّهُ عَنْهُنَّ

这些清真言的意思都是“愿真主喜悦他”，但人称分别为单数男性，双数男性，多个男性，两个人，多个女性。

最后一个尊称附加符号是这句清真言的缩写，通常附加在圣门弟子的名字后面。

## ◌ؔ
名称：`ARABIC SIGN TAKHALLUS`

附加在诗人名字上的符号，表示这个名字为笔名。

## ALM (U+061C)
名称：`ARABIC LETTER MARK`

:::note
由于这是一个不可见字符，因此标题改为其简写和码位。
:::

这是一个用于书写方向左右相反的文本混排的字符，功能与U+200F（`RIGHT-TO-LEFT MARK`）类似。

从这个字符的`scx`属性可以看出这个字符同样可以被叙利亚文和塔纳文使用。

## ؝
名称：`ARABIC END OF TEXT MARK`

一个特殊的句号，作为文本或手稿的结束标记使用。加入时间较晚，是在2021年的Unicode 14.0。

## ؞
名称：`ARABIC TRIPLE DOT PUNCTUATION MARK`

非洲曾使用阿拉伯字母的语言的句号，如豪萨语、沃洛夫语等。

## ک
名称：`ARABIC LETTER KEHEH`

了解波斯语的人会对这个字符比较熟悉。这是标准阿拉伯字母ك的变体，在波斯语、乌尔都语等语言中使用，发音与ك一样都是/k/。

## ٵ ٶ ٷ ٸ
名称：

* `ARABIC LETTER HIGH HAMZA ALEF`
* `ARABIC LETTER HIGH HAMZA WAW`
* `ARABIC LETTER U WITH HAMZA ABOVE`
* `ARABIC LETTER HIGH HAMZA YEH`

这些字符都是阿拉伯文版的哈萨克语中的字符，属于子区快*Digraphic letters for Kazakh*，目前仅中国还在使用阿拉伯文书写的哈萨克语。

对照表：

| 阿拉伯文 | 西里尔文 | 拉丁文（2021） |
|-|-|-|
| ٵ | Әә | Ää |
| ٶ | Өө | Öö |
| ٷ | Үү | Üü |
| ٸ | Іі | Iı |


另外，这些字符的兼容分解形式的字符顺序是相反的，如ٵ的兼容分解形式为اٴ（ا排在前面），在这个子区块提到：

> These characters were encoded for Kazakh digraphs, but their compatibility decompsitions do not reflect the preferred order of representation.

字符的介绍中也有“preferred spelling is...”的说明，因此这些字符的兼容分解形式是错的，Unicode官方因此推荐使用两字符的形式（也就是ٴ（`ARABIC LETTER HIGH HAMZA`）加上元音字母的形式）。

## ی
名称：`ARABIC LETTER FARSI YEH`

这个字符的独立式看上去和ى（`ARABIC LETTER ALEF MAKSURA`）没区别，但其后连式与前后连式多了两点。

| 名称 | 独立式 | 后连式 | 前后连式 | 前连式 |
|-|-|-|-|-|
| ALEF MAKSURA | ى | ىـ | ـىـ | ـى |
| FARSI YEH | ی | یـ | ـیـ | ـی |

实际上这个字符是波斯语中的ي，其独立式和前连式中的两点会消失。

## ـ
名称：`ARABIC TATWEEL`

阿拉伯延长符，Unicode名称得名于阿拉伯语تَطْوِيل。主要用于文本对齐排版和承载变音符号。[^1]

本文也使用此符号呈现字符的各种书写形式。

## ه ھ ہ ە
名称：
* `ARABIC LETTER HEH`
* `ARABIC LETTER HEH DOACHASHMEE`
* `ARABIC LETTER HEH GOAL`
* `ARABIC LETTER AE`

这些字母中有三个字母看上去相同，但是他们的连字各种形态不同：

| 名称 | 独立式 | 后连式 | 前后连式 | 前连式 |
|-|-|-|-|-|
| HEH | ه | هـ | ـهـ | ـه |
| HEH DOACHASHMEE | ھ | ھـ | ـھـ | ـھ |
| HEH GOAL | ہ | ہـ | ـہـ | ـہ |
| AE | ە | 无 | 无 | ـە |

ه（`HEH`）是阿拉伯语字母，发音为/h/。[^3]

ہ（`HEH GOAL`）是乌尔都语使用的字母，发音也为/h/，同印地文ह。

ھ ە则是突厥语族的阿拉伯文版所使用的字母，如维吾尔语、柯尔克孜语等。

## ۝
名称：`ARABIC END OF AYAH`

古兰经中的经文结束符号，其内部会包含该经文的阿拉伯文数字编号，如۝١。

目前大多数字体无法正确渲染中间带数字的形式，Segoe UI和新版Noto Sans Arabic是为数不多能正确渲染的字体之一。

## ◌ۖ ◌ۗ ◌ۘ ◌ۙ ◌ۛ
名称：

* `ARABIC SMALL HIGH LIGATURE SAD WITH LAM WITH ALEF MAKSURA`
* `ARABIC SMALL HIGH LIGATURE QAF WITH LAM WITH ALEF MAKSURA`
* `ARABIC SMALL HIGH MEEM INITIAL FORM`
* `ARABIC SMALL HIGH LAM ALEF`
* `ARABIC SMALL HIGH JEEM`
* `ARABIC SMALL HIGH THREE DOTS`

古兰经中与朗读停顿有关的符号，含义见表格：[^4]

| 符号 | 含义 |
| ---- | ---- |
| ◌ۘ | 必须停顿 |
| ◌ۙ | 不许停顿 |
| ◌ۚ | 可停可不停 |
| ◌ۖ | 不停顿更好 |
| ◌ۗ | 停顿更好 |
| ◌ۛ | 两处选择一处停顿 |

## ۞
名称：`ARABIC START OF RUB EL HIZB`

古兰经注释符号，表示一个古兰经章节的四分之一。

## ۩
名称：`ARABIC PLACE OF SAJDAH`

古兰经注释符号，用来指示经文的特定位置，当读者读到此处时需要执行“叩头”（Sajdah）的穆斯林礼仪。


[^1]: https://en.wikipedia.org/wiki/Kashida

[^2]: https://en.wiktionary.org/wiki/%D8%8F

[^3]: 在新版Noto Sans Arabic中，这个字符的独立式外观变得与`HEH DOACHASHMEE`相同。

[^4]: http://yy11.ybsj.com/msl/nianci/df008.html