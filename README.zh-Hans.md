[English](README.md) | 简体中文

# Sticker Tags

**通用属性标签：由 [Nav.cc](https://nav.cc) 发起的开放标准。版本 1.0。**

<p>
<img src="svg/caution.svg" width="32" height="32" alt="Caution" title="Caution">
<img src="svg/danger.svg" width="32" height="32" alt="Danger" title="Danger">
<img src="svg/licensed.svg" width="32" height="32" alt="Licensed" title="Licensed">
<img src="svg/sensitive.svg" width="32" height="32" alt="Sensitive" title="Sensitive">
<img src="svg/government.svg" width="32" height="32" alt="Government" title="Government">
<img src="svg/education.svg" width="32" height="32" alt="Education" title="Education">
<img src="svg/news.svg" width="32" height="32" alt="News" title="News">
<img src="svg/portal.svg" width="32" height="32" alt="Portal" title="Portal">
<img src="svg/store.svg" width="32" height="32" alt="Store" title="Store">
<img src="svg/software.svg" width="32" height="32" alt="Software" title="Software">
<img src="svg/open-source.svg" width="32" height="32" alt="Open source" title="Open source">
<img src="svg/free.svg" width="32" height="32" alt="Free" title="Free">
<img src="svg/paid.svg" width="32" height="32" alt="Paid" title="Paid">
<img src="svg/account.svg" width="32" height="32" alt="Account required" title="Account required">
<img src="svg/ios.svg" width="32" height="32" alt="iOS" title="iOS">
<img src="svg/android.svg" width="32" height="32" alt="Android" title="Android">
<img src="svg/desktop.svg" width="32" height="32" alt="Desktop" title="Desktop">
<img src="svg/extension.svg" width="32" height="32" alt="Extension" title="Extension">
<img src="svg/personal.svg" width="32" height="32" alt="Personal" title="Personal">
<img src="svg/custom.svg" width="32" height="32" alt="Customizable" title="Customizable">
</p>

网址导航、目录、软件目录和应用商店都会在每张卡片上放一排小标签：免费吗，有没有手机应用，要不要注册，有没有需要留意的地方。Sticker Tags 给这些标签一套共用的词表。每个标签有一个编号、一个永久数字编号（TID）、12 种语言的名称和准确的含义，画成圆角正方形，小到 14 像素也能分辨。

- **标准正文：** 以 https://nav.cc/standards/sticker-tags/ 上的为准。本仓库存有一份副本：[STANDARD.md](STANDARD.md)（英文，为准）和 [STANDARD.zh-Hans.md](STANDARD.zh-Hans.md)（简体中文译文）。
- **首批标签：** 20 个，分六组，以后会陆续增加。

## 仓库里有什么

| 路径 | 内容 |
| --- | --- |
| `STANDARD.md`、`STANDARD.zh-Hans.md` | 标准正文。 |
| `svg/` | 每个标签一个 SVG 文件，是 Nav.cc 的画法。 |
| `tags.json` | 所有标签：TID、编号、分组、12 种语言的名称、含义和 SVG 文件。 |

## 使用

最简单的办法：nav.cc 把每个标签都做成了图片，始终是当前的画法。标准页上有[每个标签可以直接复制的代码](https://nav.cc/standards/sticker-tags/#use)。

```html
<img src="https://nav.cc/sticker-tags/free.svg" width="20" height="20" alt="免费" title="免费">
```

把 `free` 换成 `tags.json` 里的任何编号即可（`image` 字段给出每个标签的地址）。标签显示不要小于 14 像素。也可以把 `svg/` 里的文件复制到自己的项目里。

任何人都可以出于任何目的（包括商业用途）使用，唯一的条件是在页面上注明一次来源是 Nav.cc：

```html
标签：<a href="https://nav.cc/standards/sticker-tags/">Sticker Tags（Nav.cc）</a>
```

正文、词表、图形和数据都按 [CC BY 4.0](LICENSE) 许可。标签怎么用，例如给哪个对象加哪个标签、怎么显示，由使用者自己决定。

## 提议新标签或修改

欢迎提议新标签、更清楚的含义、更好的图形和翻译：开一个 [Issue](https://github.com/nav-cc/sticker-tags/issues/new/choose) 或提交合并请求（Pull Request）。标准由 Nav.cc 编辑，提议是否采纳由 Nav.cc 决定。详见 [CONTRIBUTING.md](CONTRIBUTING.md)。
