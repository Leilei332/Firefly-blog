---
title: 特殊的标点符号一览（1）
published: 2026-10-01
category: Unicode探索
tags: 
- Unicode
---

:::note
本文不包含控制字符和空格的信息。除ASCII和Latin-1区块，其他不专门用于编码标点符号区块中的标点符号不会在此系列中提到。
:::

:::note
由于部分标点符号在正常情况下隐藏，因此标题改为其缩写和码位。
:::

广义的标点符号包含以下区块：

* 通用标点符号
* ASCII标点符号
* Latin-1标点符号
* 标点符号补充
* 中日韩符号和标点符号
* 表意符号和标点符号

## ¡¿
名称：

* `INVERTED EXCLAMATION MARK`
* `INVERTED QUESTION MARK`

西班牙语使用的标点符号，分别加在感叹号和问号的开头。

这个符号在HTML中的简易输入方法分别为`&iexcl;`和`&iquest;`。

## ¦
名称：`BROKEN BAR`

`&brvbar;`

## SHY (U+00AD)
名称：`SOFT HYPHEN`

软连字符，这个字符用于标记一个可段行处，在断行上显示，词语没有断行则不显示。

这个字符的在HTML中有简易写法：`&shy;`。

## ¯‾
名称：

* `MACRON`
* `OVERLINE`

旧名称：

* `SPACING MACRON`
* `SPACING OVERSCORE`

对这两个字符进行

Macron在HTML的简易写法为：`&macr;`,`&strns;`；Overline在HTML中的简易写法为`&oline;`,`&OverBar;`

## ‐−
名称：

* `HYPHEN`
* `MINUS SIGN`

**注意：虽然长得很像，但这两个字符不是平时使用的ASCII编码中的-（`HYPHEN-MINUS`）**

这些字符虽然外观相似，但其属性有差异，可以看其`gc`（类别）、`bidi`（双向类别）、`lb`（断行）属性。

| 字符 | 类别 | 双向类别 | 断行 |
| ---- | ---- | -------- | ---- |
| HYPHEN-MINUS | Pd | ES（欧洲数字分隔符） | HY（连字符） |
| HYPHEN | Pd | ON（其他中性） | BA（可在之后断行） |
| MINUS SIGN | Sm | ES（欧洲数字分隔符） | PR（数字前缀） |

双向类别。-（`HYPHEN-MINUS`）的双向类别为`ES`（欧洲数字分隔符），‐的双向类别为`ON`（其他中性）。

`&dash;` `&minus;`

## ‑
名称：`NON-BREAKING HYPHEN`

`GL`

## †‡
名称：

* `DAGGER`

这两个字符在HTML中的简易写法分别为`&dagger;`和`&Dagger;`。

## ․
名称：`ONE DOT LEADER`

## …
名称：`HORIZONTAL ELLIPSIS`

`&hellip;`

## ‧
名称：`HYPHENATION POINT`

## ‸
名称：`CARET`

## ※
名称：`REFERENCE MARK`

## ‽
名称：`INTERROBANG`

## ‿
名称：`UNDERTIE`

## ⁁
名称：`CARET INSERTION POINT`

`&caret;`

## ⁂
名称：`ASTERISM`

## ⁄
名称：`FRACTION SLASH`

`&frasl;`

## ⁅⁆
名称：`LEFT SQUARE BRACKET WITH QUILL`

## ⁊
名称：`TIRONIAN SIGN ET`

[^1]: https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references
