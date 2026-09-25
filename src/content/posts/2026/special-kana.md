---
title: 特殊的假名一览
published: 2026-09-22
category: Unicode探索
tags: 
- Unicode
- 语言
---

:::note
以下
:::

广义上的假名包括以下区块：

* [平假名](http://unicode.org/Public/18.0.0/charts/PDF/U3040.pdf)
* [片假名](http://unicode.org/Public/18.0.0/charts/PDF/U30A0.pdf)
* [假名增补](http://unicode.org/Public/18.0.0/charts/PDF/U1B000.pdf)
* 假名拓展[A](http://unicode.org/Public/18.0.0/charts/PDF/U1B100.pdf)、[B](http://unicode.org/Public/18.0.0/charts/PDF/U1AFF0.pdf)

## ゠
名称：`KATAKANA-HIRAGANA DOUBLE HYPHEN`

片假名中的连字符，用于书写英语借词中的连字符。之所以使用类似等号的形式是为了防止与日语发音加长符ー混淆。

## ゔヴヷヸヹヺ
名称：

* `HIRAGANA LETTER VU`
* `KATAKANA LETTER VU`
* `KATAKANA LETTER VA`
* `KATAKANA LETTER VI`
* `KATAKANA LETTER VE`
* `KATAKANA LETTER VO`

ヴヷヸヹヺ这些片假名都不在五十音图中，它们都是由福泽谕吉发明用于转写外语借词的片假名，对应罗马字都以v开头。在实际书写中，ヷヸヹヺ不常用，通常被ヴァ、ヴィ、ヴェ、ヴォ给代替，而现在的一般借词则通常使用バ行的片假名代替ヴ。

ゔ则是富士通OASYS的日语输入法中为了对应片假名ヴ而被引入的，之后加入了JIS X 0213标准，在现实中极少使用。

## ･至ﾟ
名称：

* `HALFWIDTH KATAKANA MIDDLE DOT`
* ……
* `HALFWIDTH KATAKANA SEMI-VOICED SOUND MARK`

半角假名与符号，用于兼容使用半角假名的标准JIS X 0201。

## ゐヰゑヱ
名称：

* `HIRAGANA LETTER WI`
* `KATAKANA LETTER WI`
* `HIRAGANA LETTER WE`
* `KATAKANA LETTER WE`

废弃假名，分别对应罗马音wi，we，在1946年在日语中被废弃。在冲绳语和阿伊努语中仍在使用。

## ゝヽゞヾ
名称：

* `HIRAGANA ITERATION MARK`
* `KATAKANA ITERATION MARK`
* `HIRAGANA VOICED ITERATION MARK`
* `KATAKANA VOICED ITERATION MARK`

假名中的叠音符号，ゝヽ表示重复上一个假名，如“こゝろ”同“こころ”。ゞヾ则是在前一个假名的基础上加上浊音符号，如たゞ代表ただ。

## ゟ𛄦
名称：

* `HIRAGANA DIGRAPH YORI`
* `KATAKANA DIGRAPH YORI`

对两个字符进行兼容分解会分别得到より、ヨリ，在日语中有“比较、从”的意思。

这个合字的片假名版本是刚刚在18.0版本中新增的。

## 𛄣ヿ
名称：

* `HIRAGANA DIGRAPH KOTO`
* `KATAKANA DIGRAPH KOTO`

这个合字的平假名是在不久前发布的18.0版本中新增的。

## ㇰ至ㇿ
名称：

* `KATAKANA LETTER SMALL KU`
* ……
* `KATAKANA LETTER SMALL RO`

阿伊努语使用的假名。

## 𚿰至𚿾
名称：

* `KATAKANA LETTER MINNAN TONE-2`
* ……
* `KATAKANA LETTER MINNAN NASALIZED TONE-8`

这些符号都是台湾日本殖民时期的一套用假名表示的闽南语发音所使用的符号，表示闽南语的声调，对应如下：

| 名称 | 常音 | 鼻音 |
| ---- | ---- | ---- |
| 阴平 |   | 𚿷 |
| 阴上 | 𚿰 | 𚿸 |
| 阴去 | 𚿱 | 𚿹 |
| 阴入 | 𚿲 | 𚿺 |
| 阳平 | 𚿳 | 𚿻 |
| 阳去 | 𚿵 | 𚿽 |
| 阳入 | 𚿶 | 𚿾 |

## 𛀀
名称：`KATAKANA LETTER ARCHAIC E`

## 𛀆𛄠
名称：

* `HENTAIGANA LETTER I-1`
* `KATAKANA LETTER ARCHAIC YI`

## 𛀁𛄡
名称：

* `HIRAGANA LETTER ARCHAIC YE`
* `KATAKANA LETTER ARCHAIC YE`

## 𛄟𛄢
名称：

* `HIRAGANA LETTER ARCHAIC WU`
* `KATAKANA LETTER ARCHAIC WU`

## 𛄧
不久前发布的Unicode 18.0中增加的历史片假名，对应变体假名𛂘。

## 𛄨
不久前发布的Unicode 18.0中增加的历史片假名，对应变体假名𛄍、𛄎。

[^1]: https://www.unicode.org/L2/L2020/20209r-taiwan-kana.pdf
