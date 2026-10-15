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

180翻转的感叹号和问号，为西班牙语使用的标点符号，分别加在感叹号和问号的开头。

这个符号在HTML中的简易输入方法分别为`&iexcl;`和`&iquest;`。

## ¦
名称：`BROKEN BAR`

`&brvbar;`

## SHY (U+00AD)
名称：`SOFT HYPHEN`

软连字符，这个字符用于标记一个可段行处，平时不显示，在断行时才显示。

这个字符的在HTML中有简易写法：`&shy;`。

## ¯‾
名称：

* `MACRON`
* `OVERLINE`

旧名称：

* `SPACING MACRON`
* `SPACING OVERSCORE`

虽然两个字符看上去很像，但两字符的类别不同：Macron的类别是`Sk`（修饰符号），而Overline的类别是`Po`（其他标点符号）。

对这两个字符分别进行兼容分解会得到 ̄和 ̅，也就是空格分别加上`COMBINING MACRON`和`COMBINING OVERLINE`

Macron在HTML的简易写法为：`&macr;`,`&strns;`；Overline在HTML中的简易写法为`&oline;`,`&OverBar;`

## ‐−
名称：

* `HYPHEN`
* `MINUS SIGN`

**注意：虽然长得很像，但这两个字符不是平时使用的ASCII编码中的-（`HYPHEN-MINUS`）**

这些字符虽然外观相似，但其属性有差异，可以看其`gc`（类别）、`bidi`（双向类别）、`lb`（断行）属性。

| 字符 | 类别 | 双向类别 | 断行 |
| ---- | ---- | -------- | ---- |
| HYPHEN-MINUS | Pd（连接号标点） | ES（欧洲数字分隔符） | HY（连字符） |
| HYPHEN | Pd（连接号标点） | ON（其他中性） | BA（可在之后断行） |
| MINUS SIGN | Sm（数学符号） | ES（欧洲数字分隔符） | PR（数字前缀） |

`HYPHEN`在HTML中的简易写法为`&dash;`、和`&hyphen;`；`MINUS SIGN`在HTML中的简易写法为`&minus;`。

## ‑
名称：`NON-BREAKING HYPHEN`

不断的连字符。其`lb`属性为`GL`（粘连字符）

## †‡
名称：

* `DAGGER`
* `DOUBLE DAGGER`

这两个符号通常都用于脚注标记，在*被用做脚注标记符号后†‡分别用于第二个和第三个脚注标记符号。名称dagger来源于其外观像短剑。

这两个字符在HTML中的简易写法分别为`&dagger;`和`&Dagger;`。

## •
名称：`BULLET`

这个字符与·（`MIDDLE DOT`）为兼容等价关系。和中点符号·（`MIDDLE DOT`）相比，这个字符的`lb`属性为`AL`（普通字母或符号），而中点符号为`AI`（歧义字符）

## ․
名称：`ONE DOT LEADER`

专门用于排版的前导符，在目录中用于连接章节标题和对应页码。

这个字符的兼容分解形式是.（`FULL STOP`）。与西文句号.（`FULL STOP`）相比，这个字符的`lb`（断行）属性是`IN`（不可分离），而西文句号则是`IS`（数字内缀）。

## …
名称：`HORIZONTAL ELLIPSIS`

这个字符的兼容分解形式为...，也就是三个西文句号。这个字符在HTML中的简写形式为`&hellip;`。

## ‧
名称：`HYPHENATION POINT`

和中点符号·（`MIDDLE DOT`）相比，这个字符的`lb`属性为`BA`（之后断行），而中点符号为`AI`（歧义字符）

## ‸
名称：`CARET`

## ※
名称：`REFERENCE MARK`

## ‼⁇⁈⁉
名称：

* `DOUBLE EXCLAMATION MARK`
* `DOUBLE QUESTION MARK`
* `QUESTION EXCLAMATION MARK`
* `EXCLAMATION QUESTION MARK`

‼和⁉这两个字符有emoji变体，在其后面加上变体选择器15会强制将其变形为文本外观，加上变体选择器16则会将其强制变形为emoji外观：

* ‼︎ ‼️
* ⁉︎ ⁉️

## ‽⸘
名称：

* `INTERROBANG`
* `INVERTED INTERROBANG`

问叹结合符。这个字符由美国广告高管Martin K. Speckter发明，表示即惊叹又疑问的语气，其名称“Interrobang”来源于单词“interrogation”和“bang”的结合。

⸘则是这个符号的翻转版本，用于西班牙语。

## ‿
名称：`UNDERTIE`

## ⁁
名称：`CARET INSERTION POINT`

这个字符在HTML中的简易写法为`&caret;`。

## ⁂
名称：`ASTERISM`

## ⁄
名称：`FRACTION SLASH`

**注意这不是平时使用的ASCII编码里的/（`SOLIDUS`）**

这个字符虽然外观与/（`SOLIDUS`）比较像，但属性不同：`FRACTION SLASH`的`gc`为`Sm`（数学符号），`lb`为`IS`（数字内缀）；`SOLIDUS`的`gc`为`Po`（其他标点），`lb`为`SY`（断行符号）。

类似¼这样的符号的兼容分解形式中使用此符号代表符号中的斜线，而不是/（`SOLIDUS`）。这个字符在HTML中的简易写法为`&frasl;`。

## ⁅⁆
名称：

* `LEFT SQUARE BRACKET WITH QUILL`
* `RIGHT SQUARE BRACKET WITH QUILL`

## ⹒⁊
名称：

* `TIRONIAN SIGN CAPITAL ET`
* `TIRONIAN SIGN ET`

[^1]: https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references
