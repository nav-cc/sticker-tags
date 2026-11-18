# Sticker Tags：通用属性标签标准

> **版本 1.2**，Nav.cc 于 2026-11-19 发布。
> **地址**：https://nav.cc/standards/sticker-tags/
> **仓库**：https://github.com/nav-cc/sticker-tags（图形、数据和提议）
> **以英文版为准**：本文是中文译文，仅供参考；与英文版不一致时，以英文版为准。[阅读英文版](STANDARD.md)
> **许可**：向所有人开放。任何人都可以出于任何目的使用、复制、翻译、改编和再发布本标准，唯一的条件是注明来源是 Nav.cc（第 9 节）。
> 文中加粗的「**必须**」「**不得**」「**应当**」「**不应**」「**可以**」是规范用语，对应英文版的 MUST、MUST NOT、SHOULD、SHOULD NOT、MAY（见 RFC 2119、RFC 8174）。

## 1. 为什么要有这个标准

网址导航、网站目录、软件目录和应用商店都会在每张卡片上放一排小标签，告诉访客：这个站免费吗，有没有手机应用，要不要注册，有没有需要留意的风险。现在每家各做一套：同一个标签在不同的站含义不同，同一个意思又有十几种画法。访客每到一个站都要重新学一遍，目录之间也没法交换这些信息。

Sticker Tags 只定义标签本身：

1. **词表**：一共有哪些标签，每个标签的编号、TID、名称和准确含义。
2. **外观**：样图的形状，以及标签允许显示的最小尺寸（第 6 节）。

标签怎么用，例如给哪个对象加哪个标签、依据什么、怎么显示或交换，由使用者自己决定。图形和配色使用者可以自己画；第 5 节的总览画的是 Nav.cc 的。

## 2. 适用范围

本标准为**对象**定义标签：网站、在线服务、应用，以及其他任何可以被列出的东西。标签描述对象的客观属性，不是评分、推荐或背书。

## 3. 术语

| 术语 | 含义 |
| --- | --- |
| 对象 | 标签所标的东西：网站、在线服务、应用，或其他任何可以被列出的东西。 |
| 标签 | 本标准词表中的一项属性，例如 `free`、`ios`。 |
| 标签编号 | 标签的机器可读名称：小写英文字母、数字和连字符，例如 `open-source`。 |
| TID | 标签的永久数字编号：四位数，从 1001 起。`caution` 是 1001，每个新标签取下一个空着的号（第 7 节）。第 5 节的总览按 TID 排列。 |
| 使用者 | 给对象加标签、显示标签或发布标签数据的任何一方：目录、导航站、应用商店、数据集等。 |

## 4. 基本原则

1. **只说事实，不做评价。** 标签陈述事实（「有官方 iOS 应用」），不陈述好坏（「好用」「推荐」）。
2. **不设否定标签。** 标签表示某个属性存在。**没有某个标签，不代表没有这个属性。** 标准不设否定标签：没有「不免费」，也没有「没有 iOS 应用」。
3. **编号稳定。** 已发布的编号和 TID 永不改变含义，也不重复使用；停用的编号连同它的 TID 保留在词表里，标为「已废弃」。
4. **多语言名称。** 每个标签都有英文名；附录 A 给出它在其他语言里的名称，保证同一种语言里叫法一致。
5. **可以扩展。** 使用者**可以**加自己的标签，但**必须**使用扩展编号（第 7 节），**不得**占用或改变标准编号的含义。

## 5. 词表

所有标签放在一起，按 TID 的顺序排列。每个标签有一个编号和一个 TID（第 3 节）。总览把所有标签集中在一处，每个标签按第 6.2 节的三种尺寸（大、中、允许的最小尺寸）各示一次，并列出 TID、名称、编号和含义。

| 48 px | 24 px | 14 px | TID | 编号 | 名称 | 含义 |
| --- | --- | --- | --- | --- | --- | --- |
| <img src="svg/caution.svg" width="48" height="48" alt="Caution" title="Caution"> | <img src="svg/caution.svg" width="24" height="24" alt="Caution" title="Caution"> | <img src="svg/caution.svg" width="14" height="14" alt="Caution" title="Caution"> | 1001 | `caution` | 注意 | 这个对象有访客应当留意的风险。 |
| <img src="svg/danger.svg" width="48" height="48" alt="Danger" title="Danger"> | <img src="svg/danger.svg" width="24" height="24" alt="Danger" title="Danger"> | <img src="svg/danger.svg" width="14" height="14" alt="Danger" title="Danger"> | 1002 | `danger` | 危险 | 这个对象极度危险，或需要特别当心。 |
| <img src="svg/licensed.svg" width="48" height="48" alt="Licensed" title="Licensed"> | <img src="svg/licensed.svg" width="24" height="24" alt="Licensed" title="Licensed"> | <img src="svg/licensed.svg" width="14" height="14" alt="Licensed" title="Licensed"> | 1003 | `licensed` | 持牌 | 这个对象从事需要牌照的业务，并持有监管机构颁发的有效牌照。 |
| <img src="svg/sensitive.svg" width="48" height="48" alt="Sensitive" title="Sensitive"> | <img src="svg/sensitive.svg" width="24" height="24" alt="Sensitive" title="Sensitive"> | <img src="svg/sensitive.svg" width="14" height="14" alt="Sensitive" title="Sensitive"> | 1004 | `sensitive` | 敏感 | 这个对象含有部分访客可能不想看到、或不适合未成年人的内容：成人、暴力血腥、毒品、盗版。 |
| <img src="svg/government.svg" width="48" height="48" alt="Government" title="Government"> | <img src="svg/government.svg" width="24" height="24" alt="Government" title="Government"> | <img src="svg/government.svg" width="14" height="14" alt="Government" title="Government"> | 1005 | `government` | 政府 | 由政府机关或公共机构官方运营。 |
| <img src="svg/education.svg" width="48" height="48" alt="Education" title="Education"> | <img src="svg/education.svg" width="24" height="24" alt="Education" title="Education"> | <img src="svg/education.svg" width="14" height="14" alt="Education" title="Education"> | 1006 | `education` | 教育 | 主要提供教学、课程、学习或学术资源。 |
| <img src="svg/news.svg" width="48" height="48" alt="News" title="News"> | <img src="svg/news.svg" width="24" height="24" alt="News" title="News"> | <img src="svg/news.svg" width="14" height="14" alt="News" title="News"> | 1007 | `news` | 新闻 | 主要发布新闻报道的媒体。 |
| <img src="svg/portal.svg" width="48" height="48" alt="Portal" title="Portal"> | <img src="svg/portal.svg" width="24" height="24" alt="Portal" title="Portal"> | <img src="svg/portal.svg" width="14" height="14" alt="Portal" title="Portal"> | 1008 | `portal` | 门户 | 搜索引擎或综合门户，访客从这里出发去往别处。 |
| <img src="svg/store.svg" width="48" height="48" alt="Store" title="Store"> | <img src="svg/store.svg" width="24" height="24" alt="Store" title="Store"> | <img src="svg/store.svg" width="14" height="14" alt="Store" title="Store"> | 1009 | `store` | 商店 | 主要在线销售商品或服务，包括电商平台、二手、比价和外卖平台。 |
| <img src="svg/software.svg" width="48" height="48" alt="Software" title="Software"> | <img src="svg/software.svg" width="24" height="24" alt="Software" title="Software"> | <img src="svg/software.svg" width="14" height="14" alt="Software" title="Software"> | 1010 | `software` | 软件 | 主要是软件和 IT 相关：开发工具、代码托管、开发文档、云服务和软件产品。 |
| <img src="svg/open-source.svg" width="48" height="48" alt="Open source" title="Open source"> | <img src="svg/open-source.svg" width="24" height="24" alt="Open source" title="Open source"> | <img src="svg/open-source.svg" width="14" height="14" alt="Open source" title="Open source"> | 1011 | `open-source` | 开源 | 这个对象的核心软件，或主要客户端，以 OSI 认可的许可证公开了源代码。 |
| <img src="svg/free.svg" width="48" height="48" alt="Free" title="Free"> | <img src="svg/free.svg" width="24" height="24" alt="Free" title="Free"> | <img src="svg/free.svg" width="14" height="14" alt="Free" title="Free"> | 1012 | `free` | 免费 | 核心功能可以免费使用。 |
| <img src="svg/paid.svg" width="48" height="48" alt="Paid" title="Paid"> | <img src="svg/paid.svg" width="24" height="24" alt="Paid" title="Paid"> | <img src="svg/paid.svg" width="14" height="14" alt="Paid" title="Paid"> | 1013 | `paid` | 付费 | 核心功能要付费：按订阅、按量或按交易收费；或者有免费档，但核心功能要付费解锁。 |
| <img src="svg/account.svg" width="48" height="48" alt="Account required" title="Account required"> | <img src="svg/account.svg" width="24" height="24" alt="Account required" title="Account required"> | <img src="svg/account.svg" width="14" height="14" alt="Account required" title="Account required"> | 1014 | `account` | 需账号 | 使用核心功能必须先注册或登录。 |
| <img src="svg/ios.svg" width="48" height="48" alt="iOS" title="iOS"> | <img src="svg/ios.svg" width="24" height="24" alt="iOS" title="iOS"> | <img src="svg/ios.svg" width="14" height="14" alt="iOS" title="iOS"> | 1015 | `ios` | iOS | 有官方的 iPhone 或 iPad 应用。 |
| <img src="svg/android.svg" width="48" height="48" alt="Android" title="Android"> | <img src="svg/android.svg" width="24" height="24" alt="Android" title="Android"> | <img src="svg/android.svg" width="14" height="14" alt="Android" title="Android"> | 1016 | `android` | Android | 有官方的 Android 应用。 |
| <img src="svg/desktop.svg" width="48" height="48" alt="Desktop" title="Desktop"> | <img src="svg/desktop.svg" width="24" height="24" alt="Desktop" title="Desktop"> | <img src="svg/desktop.svg" width="14" height="14" alt="Desktop" title="Desktop"> | 1017 | `desktop` | 桌面 | 有官方的 Windows、macOS 或 Linux 桌面客户端。 |
| <img src="svg/extension.svg" width="48" height="48" alt="Extension" title="Extension"> | <img src="svg/extension.svg" width="24" height="24" alt="Extension" title="Extension"> | <img src="svg/extension.svg" width="14" height="14" alt="Extension" title="Extension"> | 1018 | `extension` | 扩展 | 有官方的浏览器扩展。 |
| <img src="svg/personal.svg" width="48" height="48" alt="Personal" title="Personal"> | <img src="svg/personal.svg" width="24" height="24" alt="Personal" title="Personal"> | <img src="svg/personal.svg" width="14" height="14" alt="Personal" title="Personal"> | 1019 | `personal` | 个人 | 这个对象由个人或极小的内部团队创建。 |
| <img src="svg/custom.svg" width="48" height="48" alt="Customizable" title="Customizable"> | <img src="svg/custom.svg" width="24" height="24" alt="Customizable" title="Customizable"> | <img src="svg/custom.svg" width="14" height="14" alt="Customizable" title="Customizable"> | 1020 | `custom` | 自定义 | 这个对象支持自定义修改：访客可以修改它显示的内容。 |
| <img src="svg/ai.svg" width="48" height="48" alt="AI" title="AI"> | <img src="svg/ai.svg" width="24" height="24" alt="AI" title="AI"> | <img src="svg/ai.svg" width="14" height="14" alt="AI" title="AI"> | 1021 | `ai` | AI | 核心功能由人工智能提供，例如对话、写作、生成图片或视频。 |
| <img src="svg/social.svg" width="48" height="48" alt="Social" title="Social"> | <img src="svg/social.svg" width="24" height="24" alt="Social" title="Social"> | <img src="svg/social.svg" width="14" height="14" alt="Social" title="Social"> | 1022 | `social` | 社交 | 主要用于和他人交流、分享：社交网络、论坛、社区和即时通讯。 |
| <img src="svg/media.svg" width="48" height="48" alt="Media" title="Media"> | <img src="svg/media.svg" width="24" height="24" alt="Media" title="Media"> | <img src="svg/media.svg" width="14" height="14" alt="Media" title="Media"> | 1023 | `media` | 影音 | 主要提供视频、音乐、播客或直播。 |
| <img src="svg/game.svg" width="48" height="48" alt="Games" title="Games"> | <img src="svg/game.svg" width="24" height="24" alt="Games" title="Games"> | <img src="svg/game.svg" width="14" height="14" alt="Games" title="Games"> | 1024 | `game` | 游戏 | 主要提供游戏：网页游戏、在线游戏，或游戏平台。 |
| <img src="svg/finance.svg" width="48" height="48" alt="Finance" title="Finance"> | <img src="svg/finance.svg" width="24" height="24" alt="Finance" title="Finance"> | <img src="svg/finance.svg" width="14" height="14" alt="Finance" title="Finance"> | 1025 | `finance` | 金融 | 主要提供金融服务：银行、支付、投资、保险、借贷或加密资产交易。 |
| <img src="svg/email.svg" width="48" height="48" alt="Email" title="Email"> | <img src="svg/email.svg" width="24" height="24" alt="Email" title="Email"> | <img src="svg/email.svg" width="14" height="14" alt="Email" title="Email"> | 1026 | `email` | 邮件 | 主要提供电子邮件服务：个人邮箱、企业邮箱或临时邮箱。 |
| <img src="svg/trial.svg" width="48" height="48" alt="Free trial" title="Free trial"> | <img src="svg/trial.svg" width="24" height="24" alt="Free trial" title="Free trial"> | <img src="svg/trial.svg" width="14" height="14" alt="Free trial" title="Free trial"> | 1027 | `trial` | 试用 | 付费的核心功能可以免费试用一段时间。 |
| <img src="svg/ads.svg" width="48" height="48" alt="Ads" title="Ads"> | <img src="svg/ads.svg" width="24" height="24" alt="Ads" title="Ads"> | <img src="svg/ads.svg" width="14" height="14" alt="Ads" title="Ads"> | 1028 | `ads` | 广告 | 这个对象显示广告。 |
| <img src="svg/web.svg" width="48" height="48" alt="Web" title="Web"> | <img src="svg/web.svg" width="24" height="24" alt="Web" title="Web"> | <img src="svg/web.svg" width="14" height="14" alt="Web" title="Web"> | 1029 | `web` | 网页版 | 有官方的网页版：在浏览器里就能使用核心功能，不用安装。 |
| <img src="svg/nonprofit.svg" width="48" height="48" alt="Nonprofit" title="Nonprofit"> | <img src="svg/nonprofit.svg" width="24" height="24" alt="Nonprofit" title="Nonprofit"> | <img src="svg/nonprofit.svg" width="14" height="14" alt="Nonprofit" title="Nonprofit"> | 1030 | `nonprofit` | 非营利 | 这个对象由非营利组织运营。 |
| <img src="svg/pending-review.svg" width="48" height="48" alt="Pending review" title="Pending review"> | <img src="svg/pending-review.svg" width="24" height="24" alt="Pending review" title="Pending review"> | <img src="svg/pending-review.svg" width="14" height="14" alt="Pending review" title="Pending review"> | 1031 | `pending-review` | 待审核 | 这个对象尚未经使用者仔细审核。 |

## 6. 外观

### 6.1 形状与图形

1. **寓意和识别度第一。** 标签的图形和颜色**必须**正确表达标签的含义，标签**必须**一眼就能认出来，小到第 6.2 节的最小尺寸也一样。本节其余各条都为这一条服务。
2. 样图，即第 5 节的总览和 Nav.cc 提供的图片，把每个标签画成圆角正方形，圆角半径为边长的 22%。这个形状只是样图的出样标准：使用者**可以**用任何形状显示标签，例如圆形，只要满足第 1 条。
3. 图形**必须**是矢量图（例如 SVG）。**不得**用位图（PNG、JPEG、WebP 等），位图缩放会发糊；也**不得**用字体里的文字字符，它的样子取决于设备上的字体。
4. 图形的颜色不限，表达含义需要几种就用几种。图形在标签中居中，**应当**占标签宽度的 65% 到 75%；Nav.cc 在 16×16 的网格上画图形，占边长的 70%。图形设计需要时**可以**更大，只要还露出一圈标签的底色：`free` 的圆占 87.5%。
5. 为了便于识别，图形的每种颜色与它下面的颜色的对比度**应当**至少 3:1（WCAG 2.2 对非文字内容的要求）。
6. **不得**把标签画成看起来像认证、奖章或评分的样子。

### 6.2 尺寸

1. 不论什么形状，标签的宽度**不得**小于 14 个 CSS 像素。这是本标准每个图形都还能分辨的最小尺寸，是在 1 倍像素密度下逐个目测确定的。
2. 自己画图形的使用者，**应当**在这个尺寸下检查；分辨不出来时，**必须**用更大的最小尺寸。
3. 第 5 节把每个标签按三种尺寸各示一次：大（48 px）、中（24 px）和允许的最小尺寸（14 px）。

## 7. 扩展与版本

- **扩展标签：** 扩展编号**必须**以 `x-<使用者简称>-` 开头，例如 `x-example-beta`。扩展标签**不得**与标准标签同名，**不得**改变标准标签的含义。它和标准标签遵守同样的外观规则（第 6 节），图形和配色**应当**与每个标准标签都不同。
- **TID：** 新标签取下一个空着的 TID，加在总览的最后；TID 不会给别的标签再用。
- **版本号：** 写作「主版本.次版本」。次版本只增加标签，不改变已有含义。要改变含义，就要新增编号并升主版本；旧编号标为「已废弃」，至少保留一个主版本。
- **本页**始终显示当前版本。

## 8. 治理

- Nav.cc 发起本标准并担任编辑：维护词表，发布新版本，记录每次变更。
- 任何人都可以提出新标签或修改意见：在 https://github.com/nav-cc/sticker-tags 开一个 Issue 或提交合并请求（Pull Request）。
- 提议是否采纳由 Nav.cc 决定，Nav.cc 有最终决定权。
- 采用本标准的其他目录，可以申请加入共同维护。

## 9. 许可

本标准向所有人开放。它的正文、词表和标签编号以及第 5 节展示的图形，任何人都可以出于任何目的（包括商业用途）使用、复制、翻译、改编和再发布，唯一的条件是：注明来源是 Nav.cc，在条件允许时附上 https://nav.cc/standards/sticker-tags/ 的链接。建议的署名写法：「Sticker Tags，来源：Nav.cc（https://nav.cc/standards/sticker-tags/）」。这与知识共享署名 4.0 国际许可（CC BY 4.0）一致：https://creativecommons.org/licenses/by/4.0/

## 附录 A：各语言的名称

本附录仅供参考。下表是 Nav.cc 使用的译名。

| TID | 标签 | English | Français | Español | العربية | Português | Русский | Deutsch | 日本語 | 한국어 | Ελληνικά | 简体中文 | 繁體中文 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1001 | `caution` | Caution | Attention | Precaución | تنبيه | Atenção | Внимание | Vorsicht | 注意 | 주의 | Προσοχή | 注意 | 注意 |
| 1002 | `danger` | Danger | Danger | Peligro | خطر | Perigo | Опасно | Gefahr | 危険 | 위험 | Κίνδυνος | 危险 | 危險 |
| 1003 | `licensed` | Licensed | Autorisé | Con licencia | مرخّص | Licenciado | Лицензия | Lizenziert | 許可済み | 허가 | Με άδεια | 持牌 | 持牌 |
| 1004 | `sensitive` | Sensitive | Sensible | Sensible | حسّاس | Sensível | Чувствительный | Sensibel | センシティブ | 민감 | Ευαίσθητο | 敏感 | 敏感 |
| 1005 | `government` | Government | État | Gobierno | حكومة | Governo | Государство | Staat | 政府 | 정부 | Δημόσιο | 政府 | 政府 |
| 1006 | `education` | Education | Éducation | Educación | تعليم | Educação | Образование | Bildung | 教育 | 교육 | Εκπαίδευση | 教育 | 教育 |
| 1007 | `news` | News | Actualités | Noticias | أخبار | Notícias | Новости | Nachrichten | ニュース | 뉴스 | Ειδήσεις | 新闻 | 新聞 |
| 1008 | `portal` | Portal | Portail | Portal | بوابة | Portal | Портал | Portal | ポータル | 포털 | Πύλη | 门户 | 入口 |
| 1009 | `store` | Store | Boutique | Tienda | متجر | Loja | Магазин | Shop | ショップ | 상점 | Κατάστημα | 商店 | 商店 |
| 1010 | `software` | Software | Logiciel | Software | برمجيات | Software | ПО | Software | ソフトウェア | 소프트웨어 | Λογισμικό | 软件 | 軟體 |
| 1011 | `open-source` | Open source | Open source | Código abierto | مفتوح المصدر | Código aberto | Открытый код | Open Source | オープンソース | 오픈 소스 | Ανοιχτός κώδικας | 开源 | 開源 |
| 1012 | `free` | Free | Gratuit | Gratis | مجاني | Grátis | Бесплатно | Kostenlos | 無料 | 무료 | Δωρεάν | 免费 | 免費 |
| 1013 | `paid` | Paid | Payant | De pago | مدفوع | Pago | Платно | Kostenpflichtig | 有料 | 유료 | Επί πληρωμή | 付费 | 付費 |
| 1014 | `account` | Account required | Compte requis | Cuenta obligatoria | حساب مطلوب | Conta necessária | Нужен аккаунт | Konto nötig | アカウント必須 | 계정 필요 | Απαιτείται λογαριασμός | 需账号 | 需帳號 |
| 1015 | `ios` | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS |
| 1016 | `android` | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android |
| 1017 | `desktop` | Desktop | Ordinateur | Escritorio | سطح المكتب | Computador | Компьютер | Desktop | デスクトップ | 데스크톱 | Υπολογιστής | 桌面 | 桌面 |
| 1018 | `extension` | Extension | Extension | Extensión | إضافة | Extensão | Расширение | Erweiterung | 拡張機能 | 확장 프로그램 | Επέκταση | 扩展 | 擴充功能 |
| 1019 | `personal` | Personal | Personnel | Personal | شخصي | Pessoal | Личный | Persönlich | 個人 | 개인 | Προσωπικό | 个人 | 個人 |
| 1020 | `custom` | Customizable | Personnalisable | Personalizable | قابل للتخصيص | Personalizável | Настраиваемый | Anpassbar | カスタマイズ可 | 사용자 지정 가능 | Προσαρμόσιμο | 自定义 | 自訂 |
| 1021 | `ai` | AI | IA | IA | ذكاء اصطناعي | IA | ИИ | KI | AI | AI | ΤΝ | AI | AI |
| 1022 | `social` | Social | Social | Social | تواصل اجتماعي | Social | Соцсети | Sozial | ソーシャル | 소셜 | Κοινωνικά | 社交 | 社交 |
| 1023 | `media` | Media | Médias | Multimedia | وسائط | Mídia | Медиа | Medien | 動画・音楽 | 미디어 | Πολυμέσα | 影音 | 影音 |
| 1024 | `game` | Games | Jeux | Juegos | ألعاب | Jogos | Игры | Spiele | ゲーム | 게임 | Παιχνίδια | 游戏 | 遊戲 |
| 1025 | `finance` | Finance | Finance | Finanzas | مالية | Finanças | Финансы | Finanzen | 金融 | 금융 | Οικονομικά | 金融 | 金融 |
| 1026 | `email` | Email | E-mail | Correo | بريد إلكتروني | E-mail | Почта | E-Mail | メール | 이메일 | Email | 邮件 | 郵件 |
| 1027 | `trial` | Free trial | Essai gratuit | Prueba gratis | تجربة مجانية | Teste grátis | Пробный период | Testphase | 試用 | 체험판 | Δοκιμή | 试用 | 試用 |
| 1028 | `ads` | Ads | Publicité | Anuncios | إعلانات | Anúncios | Реклама | Werbung | 広告あり | 광고 | Διαφημίσεις | 广告 | 廣告 |
| 1029 | `web` | Web | Web | Web | ويب | Web | Веб | Web | ウェブ版 | 웹 | Web | 网页版 | 網頁版 |
| 1030 | `nonprofit` | Nonprofit | Non lucratif | Sin ánimo de lucro | غير ربحي | Sem fins lucrativos | Некоммерческий | Gemeinnützig | 非営利 | 비영리 | Μη κερδοσκοπικό | 非营利 | 非營利 |
| 1031 | `pending-review` | Pending review | En attente de vérification | Pendiente de revisión | قيد المراجعة | Revisão pendente | Ожидает проверки | Prüfung ausstehend | 審査待ち | 검토 대기 | Εκκρεμεί έλεγχος | 待审核 | 待審核 |
