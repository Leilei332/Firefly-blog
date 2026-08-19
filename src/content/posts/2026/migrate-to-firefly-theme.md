---
title: 博客迁移至Firefly主题
published: 2026-08-20
category: 站点
---

最近从之前使用的[重新编排](https://retypeset.radishzz.cc)主题迁移至了[Firefly](https://firefly.cuteleaf.cn)主题。

之所以进行迁移，是因为之前使用的博客主题存在一些问题。

![之前使用的“重新编排”主题](../_images/zen_1mTblR58nd.png)

![现在使用的Firefly主题](../_images/zen_QAiqAFtIKO.png)

## 暗色模式切换问题
使用重新编排主题后，我发现这个主题的自动切换暗色模式功能非常容易坏：这个暗色模式切换按钮没有自动切换暗色模式的选项，并且第一次切换暗色之后再访问就不会自动切换了，只有再重新手动开关一下系统暗色模式才会触发自动切换。

然而在我寻找其他主题的过程中，我发现这是一个大多数主题都存在的问题：在这些候选主题中，[Mizuki](http://mizuki.mysqil.com)不支持暗色模式自动切换；[Antfustyle](https://github.com/lin-stephanie/astro-antfustyle-theme)主题、[astro-paper](https://astro-paper.pages.dev)主题和重新编排有同样的问题；只有[Twilight](https://twilight.spr-aachen.com)和[Firefly](https://firefly.cuteleaf.cn)提供了自动切换选项，并且能正常运作。

## 时间戳问题
这个问题与“博客俱乐部”有关。Astro的文章的时间戳格式是靠主题定义的，而“重新编排”主题只支持仅日期的时间戳格式（类似`2020-01-01`），在生成RSS中这个文章的时间就会变成`8:00`。如果其他支持使用时间的博客发布了，这个博客文章就会往往排在“博客俱乐部”文章列表的后面，容易被忽视。

在我找到的博客主题中，只有Antfustyle和astro-paper主题支持使用时间。

## 选择主题
我本来是想要解决时间戳问题的，因此本来想迁移到Antfustyle和astro-paper其中之一。但迁移到这两个主题的成本较高：

这两个主题使用的Admontion语法和我现在使用的不兼容。它们使用的是Github式语法：

```markdown
> [!TIP]
> This is a tip.
```

而我的博客文章里使用的是另一种语法：

```markdown
:::tip
This is a tip.
:::
```

在我第一次选Astro主题时这就是一个头疼的问题。当时我的流程是在Tiddlywiki中写博客再导出至博客网站，而大多数主题仅支持Github式语法，选择“重新编排”这个主题也是因为它同时支持两种语法。

另外别的方面也有不兼容的地方：`published`和`updated`字段在Antfustyle中变成了`pubDate`和`lastModDate`，在astro-paper中变成了`pubDatetime`和`modDatetime`；`slug`字段在astro-paper中变成了`permalink`。我本来想花一段时间把原博客文章都迁移过去，但这两个主题的暗黑模式问题成为了压倒骆驼的最后一根稻草。

之后，我本来想用Twilight主题，这个主题支持我使用的Admonition语法，但是它不够现代化，pnpm用的还是9版本，并且也不太喜欢yml格式。最终选择了类似的代替品Firefly。

## 迁移
Firefly主题使用的字段大多数都是和现有文章相同的，因此迁移还是比较快的，基本上就是将标签适配了`category`属性，迁移`abbrlink`[^1]和`pin`属性。

## 重新配置
Firefly的配置都存放在`src/config`文件夹中。大部分配置没啥好说的。

其中字体配置折腾了一下。这个配置可以让网页使用自定义的字体，并且还可以去除字体中不常用的字符、区块，以减少自定义字体大小，增加加载速度。

```json
// 通过设置subsets属性使获取的字体只包含常用拉丁文字符
{
	name: "Zen Maru Gothic",
	cssVariable: "--font-zen-maru-gothic",
	provider: "fontsource",
	weights: ["300", "400", "500", "600", "700"],
	styles: ["normal"],
	subsets: ["latin"],
	fallbacks: ["sans-serif"],
}
```

我本来想让页面使用`Noto Sans Arabic ➡️ Noto Sans ➡️ 系统字体`的回退方式，但是浏览器的字体回退机制实在是过于抽象，因此最后只套了一个`Noto Sans Arabic`字体。

## 新功能
目前已用上了Firefly主题的不少新功能，包括动态、书签导航。书签导航加了不少有趣的网页。

[^1]: 这个是“重新编排”主题中定义文章slug的字段，后来我发现使用`slug`也可以被识别。现在感觉直接将Markdown文件名作为slug反而更方便些。