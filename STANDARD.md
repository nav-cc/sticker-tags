# Sticker Tags: Universal Attribute Tags

> **Version 1.1**, published 2026-11-16 by Nav.cc.
> **Address:** https://nav.cc/standards/sticker-tags/
> **Repository:** https://github.com/nav-cc/sticker-tags (glyphs, data and proposals)
> **Canonical language:** English. Translations are informative; where they differ, this text prevails.
> **License:** open to everyone. You may use, copy, translate, adapt and redistribute this standard for any purpose, on one condition: credit Nav.cc as the source (section 9).
> The key words **MUST**, **MUST NOT**, **SHOULD**, **SHOULD NOT** and **MAY** are to be read as described in RFC 2119 and RFC 8174 when, and only when, they appear in bold capitals.

## 1. Why this standard

Web directories, start pages, software catalogs and app stores put a row of small badges on each card: is it free, is there a phone app, does it need an account, is there something to be careful about. Today every directory draws its own set. The same badge means different things on different sites, and the same meaning is drawn a dozen ways. Visitors relearn the badges on every site, and directories cannot exchange the information.

Sticker Tags defines the tags themselves:

1. **Vocabulary**: which tags exist, and each tag's identifier, TID, names and exact meaning.
2. **Appearance**: the shape of the sample drawings and the smallest size a tag may be shown at (section 6).

How tags are used, such as which object is given which tag, on what evidence, and how tags are shown or exchanged, is left to their users. Users may draw their own glyphs and colors; the showcase in section 5 shows Nav.cc's.

## 2. Scope

The standard defines tags for **objects**: websites, online services, apps and anything else that can be listed. A tag describes an objective attribute of an object. It is not a rating, a recommendation or an endorsement.

## 3. Terms

| Term | Meaning |
| --- | --- |
| Object | Whatever a tag is attached to: a website, an online service, an app or anything else that can be listed. |
| Tag | One attribute from this standard's vocabulary, such as `free` or `ios`. |
| Tag identifier | A tag's machine-readable name: lowercase ASCII letters, digits and hyphens, such as `open-source`. |
| TID | A tag's permanent number: four digits, from 1001. The twenty tags of version 1.0 were numbered in the order of the showcase in section 5, `caution` being 1001; each later tag takes the next free number (section 7). |
| User | Anyone who gives tags to objects, shows them or publishes them: a directory, a start page, an app store, a dataset. |

## 4. Principles

1. **Facts, not judgments.** A tag states a fact ("has an official iOS app"), never a judgment ("good", "recommended").
2. **No negative tags.** A tag says that an attribute is present. **The absence of a tag does not mean the attribute is absent.** There are no negative tags: no "not free", no "no iOS app".
3. **Stable identifiers.** A published identifier or TID never changes meaning and is never reused. A retired identifier stays in the vocabulary, with its TID, marked deprecated.
4. **Names in many languages.** Every tag has an English name. Appendix A gives its names in other languages, so that one language uses one name.
5. **Extensible.** A user **MAY** add tags of their own, but **MUST** use extension identifiers (section 7) and **MUST NOT** take over or change the meaning of a standard identifier.

## 5. Vocabulary

Thirty tags in six groups: notices (TID 1001 to 1004), type (1005 to 1010 and 1021 to 1026), open source (1011), cost and account (1012 to 1014, 1027 and 1028), platforms (1015 to 1018 and 1029), and origin and customization (1019, 1020 and 1030). Each tag has an identifier and a TID (section 3); within a group, tags are listed in the showcase's order, not by TID. The showcase gathers every tag in one place, at the three sizes of section 6.2 (large, medium and the smallest allowed), with its TID, name, identifier and meaning.

| 48 px | 24 px | 14 px | TID | Identifier | Name | Meaning |
| --- | --- | --- | --- | --- | --- | --- |
| <img src="svg/caution.svg" width="48" height="48" alt="Caution" title="Caution"> | <img src="svg/caution.svg" width="24" height="24" alt="Caution" title="Caution"> | <img src="svg/caution.svg" width="14" height="14" alt="Caution" title="Caution"> | 1001 | `caution` | Caution | The object carries a risk the visitor should be aware of. |
| <img src="svg/danger.svg" width="48" height="48" alt="Danger" title="Danger"> | <img src="svg/danger.svg" width="24" height="24" alt="Danger" title="Danger"> | <img src="svg/danger.svg" width="14" height="14" alt="Danger" title="Danger"> | 1002 | `danger` | Danger | The object is extremely dangerous, or calls for special care. |
| <img src="svg/licensed.svg" width="48" height="48" alt="Licensed" title="Licensed"> | <img src="svg/licensed.svg" width="24" height="24" alt="Licensed" title="Licensed"> | <img src="svg/licensed.svg" width="14" height="14" alt="Licensed" title="Licensed"> | 1003 | `licensed` | Licensed | The object operates in a business that requires a license, and holds a valid license from a regulator. |
| <img src="svg/sensitive.svg" width="48" height="48" alt="Sensitive" title="Sensitive"> | <img src="svg/sensitive.svg" width="24" height="24" alt="Sensitive" title="Sensitive"> | <img src="svg/sensitive.svg" width="14" height="14" alt="Sensitive" title="Sensitive"> | 1004 | `sensitive` | Sensitive | The object contains content some visitors may not want to see, or that is unsuitable for minors: adult content, graphic violence, drugs, piracy. |
| <img src="svg/government.svg" width="48" height="48" alt="Government" title="Government"> | <img src="svg/government.svg" width="24" height="24" alt="Government" title="Government"> | <img src="svg/government.svg" width="14" height="14" alt="Government" title="Government"> | 1005 | `government` | Government | Officially run by a government body or public institution. |
| <img src="svg/education.svg" width="48" height="48" alt="Education" title="Education"> | <img src="svg/education.svg" width="24" height="24" alt="Education" title="Education"> | <img src="svg/education.svg" width="14" height="14" alt="Education" title="Education"> | 1006 | `education` | Education | Mainly provides teaching, courses, learning or academic resources. |
| <img src="svg/news.svg" width="48" height="48" alt="News" title="News"> | <img src="svg/news.svg" width="24" height="24" alt="News" title="News"> | <img src="svg/news.svg" width="14" height="14" alt="News" title="News"> | 1007 | `news` | News | A media outlet that mainly publishes news reporting. |
| <img src="svg/portal.svg" width="48" height="48" alt="Portal" title="Portal"> | <img src="svg/portal.svg" width="24" height="24" alt="Portal" title="Portal"> | <img src="svg/portal.svg" width="14" height="14" alt="Portal" title="Portal"> | 1008 | `portal` | Portal | A search engine or general portal, a place visitors start from to go elsewhere. |
| <img src="svg/store.svg" width="48" height="48" alt="Store" title="Store"> | <img src="svg/store.svg" width="24" height="24" alt="Store" title="Store"> | <img src="svg/store.svg" width="14" height="14" alt="Store" title="Store"> | 1009 | `store` | Store | Mainly sells goods or services online, including marketplaces, second-hand, price comparison and delivery platforms. |
| <img src="svg/software.svg" width="48" height="48" alt="Software" title="Software"> | <img src="svg/software.svg" width="24" height="24" alt="Software" title="Software"> | <img src="svg/software.svg" width="14" height="14" alt="Software" title="Software"> | 1010 | `software` | Software | Mainly about software and IT: developer tools, code hosting, developer documentation, cloud services and software products. |
| <img src="svg/ai.svg" width="48" height="48" alt="AI" title="AI"> | <img src="svg/ai.svg" width="24" height="24" alt="AI" title="AI"> | <img src="svg/ai.svg" width="14" height="14" alt="AI" title="AI"> | 1021 | `ai` | AI | The core features are provided by artificial intelligence, such as chat, writing, or generating images or video. |
| <img src="svg/social.svg" width="48" height="48" alt="Social" title="Social"> | <img src="svg/social.svg" width="24" height="24" alt="Social" title="Social"> | <img src="svg/social.svg" width="14" height="14" alt="Social" title="Social"> | 1022 | `social` | Social | Mainly for talking and sharing with other people: social networks, forums, communities and instant messaging. |
| <img src="svg/media.svg" width="48" height="48" alt="Media" title="Media"> | <img src="svg/media.svg" width="24" height="24" alt="Media" title="Media"> | <img src="svg/media.svg" width="14" height="14" alt="Media" title="Media"> | 1023 | `media` | Media | Mainly offers video, music, podcasts or live streams. |
| <img src="svg/game.svg" width="48" height="48" alt="Games" title="Games"> | <img src="svg/game.svg" width="24" height="24" alt="Games" title="Games"> | <img src="svg/game.svg" width="14" height="14" alt="Games" title="Games"> | 1024 | `game` | Games | Mainly offers games: browser games, online games, or a platform for games. |
| <img src="svg/finance.svg" width="48" height="48" alt="Finance" title="Finance"> | <img src="svg/finance.svg" width="24" height="24" alt="Finance" title="Finance"> | <img src="svg/finance.svg" width="14" height="14" alt="Finance" title="Finance"> | 1025 | `finance` | Finance | Mainly provides financial services: banking, payments, investing, insurance, lending or trading crypto-assets. |
| <img src="svg/email.svg" width="48" height="48" alt="Email" title="Email"> | <img src="svg/email.svg" width="24" height="24" alt="Email" title="Email"> | <img src="svg/email.svg" width="14" height="14" alt="Email" title="Email"> | 1026 | `email` | Email | Mainly provides email: personal, business or disposable mailboxes. |
| <img src="svg/open-source.svg" width="48" height="48" alt="Open source" title="Open source"> | <img src="svg/open-source.svg" width="24" height="24" alt="Open source" title="Open source"> | <img src="svg/open-source.svg" width="14" height="14" alt="Open source" title="Open source"> | 1011 | `open-source` | Open source | The object's core software, or its main client, is published as source code under an OSI-approved license. |
| <img src="svg/free.svg" width="48" height="48" alt="Free" title="Free"> | <img src="svg/free.svg" width="24" height="24" alt="Free" title="Free"> | <img src="svg/free.svg" width="14" height="14" alt="Free" title="Free"> | 1012 | `free` | Free | The core features can be used free of charge. |
| <img src="svg/paid.svg" width="48" height="48" alt="Paid" title="Paid"> | <img src="svg/paid.svg" width="24" height="24" alt="Paid" title="Paid"> | <img src="svg/paid.svg" width="14" height="14" alt="Paid" title="Paid"> | 1013 | `paid` | Paid | The core features have to be paid for: by subscription, by usage or per transaction; or a free tier exists but its core features are unlocked by payment. |
| <img src="svg/trial.svg" width="48" height="48" alt="Free trial" title="Free trial"> | <img src="svg/trial.svg" width="24" height="24" alt="Free trial" title="Free trial"> | <img src="svg/trial.svg" width="14" height="14" alt="Free trial" title="Free trial"> | 1027 | `trial` | Free trial | The paid core features can be tried free for a limited time. |
| <img src="svg/ads.svg" width="48" height="48" alt="Ads" title="Ads"> | <img src="svg/ads.svg" width="24" height="24" alt="Ads" title="Ads"> | <img src="svg/ads.svg" width="14" height="14" alt="Ads" title="Ads"> | 1028 | `ads` | Ads | The object shows ads. |
| <img src="svg/account.svg" width="48" height="48" alt="Account required" title="Account required"> | <img src="svg/account.svg" width="24" height="24" alt="Account required" title="Account required"> | <img src="svg/account.svg" width="14" height="14" alt="Account required" title="Account required"> | 1014 | `account` | Account required | An account (sign-up or sign-in) is required to use the core features. |
| <img src="svg/web.svg" width="48" height="48" alt="Web" title="Web"> | <img src="svg/web.svg" width="24" height="24" alt="Web" title="Web"> | <img src="svg/web.svg" width="14" height="14" alt="Web" title="Web"> | 1029 | `web` | Web | There is an official web version: the core features work in a browser, with nothing to install. |
| <img src="svg/ios.svg" width="48" height="48" alt="iOS" title="iOS"> | <img src="svg/ios.svg" width="24" height="24" alt="iOS" title="iOS"> | <img src="svg/ios.svg" width="14" height="14" alt="iOS" title="iOS"> | 1015 | `ios` | iOS | There is an official iPhone or iPad app. |
| <img src="svg/android.svg" width="48" height="48" alt="Android" title="Android"> | <img src="svg/android.svg" width="24" height="24" alt="Android" title="Android"> | <img src="svg/android.svg" width="14" height="14" alt="Android" title="Android"> | 1016 | `android` | Android | There is an official Android app. |
| <img src="svg/desktop.svg" width="48" height="48" alt="Desktop" title="Desktop"> | <img src="svg/desktop.svg" width="24" height="24" alt="Desktop" title="Desktop"> | <img src="svg/desktop.svg" width="14" height="14" alt="Desktop" title="Desktop"> | 1017 | `desktop` | Desktop | There is an official desktop client for Windows, macOS or Linux. |
| <img src="svg/extension.svg" width="48" height="48" alt="Extension" title="Extension"> | <img src="svg/extension.svg" width="24" height="24" alt="Extension" title="Extension"> | <img src="svg/extension.svg" width="14" height="14" alt="Extension" title="Extension"> | 1018 | `extension` | Extension | There is an official browser extension. |
| <img src="svg/nonprofit.svg" width="48" height="48" alt="Nonprofit" title="Nonprofit"> | <img src="svg/nonprofit.svg" width="24" height="24" alt="Nonprofit" title="Nonprofit"> | <img src="svg/nonprofit.svg" width="14" height="14" alt="Nonprofit" title="Nonprofit"> | 1030 | `nonprofit` | Nonprofit | The object is run by a nonprofit organization. |
| <img src="svg/personal.svg" width="48" height="48" alt="Personal" title="Personal"> | <img src="svg/personal.svg" width="24" height="24" alt="Personal" title="Personal"> | <img src="svg/personal.svg" width="14" height="14" alt="Personal" title="Personal"> | 1019 | `personal` | Personal | The object was created by an individual or a very small internal team. |
| <img src="svg/custom.svg" width="48" height="48" alt="Customizable" title="Customizable"> | <img src="svg/custom.svg" width="24" height="24" alt="Customizable" title="Customizable"> | <img src="svg/custom.svg" width="14" height="14" alt="Customizable" title="Customizable"> | 1020 | `custom` | Customizable | The object supports customization: the visitor can change what it shows. |

## 6. Appearance

### 6.1 Shape and glyph

1. **Meaning and recognition come first.** A tag's glyph and colors **MUST** carry the tag's meaning correctly, and the tag **MUST** be recognizable at a glance, down to the smallest size of section 6.2. Every other rule of this section serves this one.
2. The sample drawings, that is the showcase in section 5 and the images Nav.cc serves, draw each tag as a square with rounded corners, the corner radius 22% of the side. This shape is the standard for the samples only: a user **MAY** show tags in any shape, such as a circle, as long as item 1 holds.
3. The glyph **MUST** be vector graphics, such as SVG. It **MUST NOT** be a raster image (PNG, JPEG, WebP and the like), which blurs when scaled, nor a character set in a font, whose look depends on the fonts of the device.
4. The glyph may use as many colors as its meaning needs. It is centered on the tag and **SHOULD** take 65% to 75% of the tag's width; Nav.cc draws its glyphs on a 16×16 grid and gives them 70%. A glyph **MAY** take more where its design calls for it, as long as a rim of the tag's background still shows: the disc of `free` takes 87.5%.
5. To help recognition, each color of the glyph **SHOULD** have a contrast ratio of at least 3:1 against the color it sits on (WCAG 2.2, non-text contrast).
6. Tags **MUST NOT** be drawn to look like a certification, a medal or a rating.

### 6.2 Size

1. A tag **MUST NOT** be shown smaller than 14 CSS pixels across, whatever its shape. This is the smallest size at which every glyph of this standard can still be told apart; it was checked by eye at a device pixel ratio of 1.
2. A user who draws glyphs of their own **SHOULD** check them at that size, and **MUST** use a larger minimum if they cannot be told apart.
3. Section 5 shows every tag at three sizes: large (48 px), medium (24 px) and the smallest allowed (14 px).

## 7. Extensions and versions

- **Extension tags:** an extension identifier **MUST** start with `x-<user>-`, where `<user>` is a short name of the user who defines it, for example `x-example-beta`. An extension tag **MUST NOT** share a name with a standard tag, and **MUST NOT** change a standard tag's meaning. It follows the same appearance rules as a standard tag (section 6), and its glyph and color **SHOULD** differ from those of every standard tag.
- **TIDs:** a new tag takes the next free TID, whatever its place in the showcase; a TID is never given to another tag.
- **Version numbers:** `major.minor`. A minor version only adds tags and never changes an existing meaning. A change of meaning requires a new identifier and a new major version; the old identifier is marked deprecated and kept for at least one major version.
- **This page** always shows the current version.

## 8. Governance

- Nav.cc initiated the standard and acts as its editor: it maintains the vocabulary, publishes new versions and records every change.
- Anyone may propose a new tag or a change, by opening an issue or a pull request at https://github.com/nav-cc/sticker-tags.
- Nav.cc decides whether a proposal is adopted, and has the final say.
- Other directories that adopt the standard may apply to join its maintenance.

## 9. License

This standard is open. Its text, its vocabulary and tag identifiers, and the glyphs shown in section 5 may be used, copied, translated, adapted and redistributed by anyone, for any purpose, including commercial use, on one condition: credit Nav.cc as the source, with a link to https://nav.cc/standards/sticker-tags/ where the medium allows. Suggested credit: "Sticker Tags, by Nav.cc (https://nav.cc/standards/sticker-tags/)". This corresponds to the Creative Commons Attribution 4.0 International license (CC BY 4.0): https://creativecommons.org/licenses/by/4.0/

## Appendix A: Names in other languages

This appendix is informative. These are the names Nav.cc uses.

| TID | Tag | English | Français | Español | العربية | Português | Русский | Deutsch | 日本語 | 한국어 | Ελληνικά | 简体中文 | 繁體中文 |
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
| 1021 | `ai` | AI | IA | IA | ذكاء اصطناعي | IA | ИИ | KI | AI | AI | ΤΝ | AI | AI |
| 1022 | `social` | Social | Social | Social | تواصل اجتماعي | Social | Соцсети | Sozial | ソーシャル | 소셜 | Κοινωνικά | 社交 | 社交 |
| 1023 | `media` | Media | Médias | Multimedia | وسائط | Mídia | Медиа | Medien | 動画・音楽 | 미디어 | Πολυμέσα | 影音 | 影音 |
| 1024 | `game` | Games | Jeux | Juegos | ألعاب | Jogos | Игры | Spiele | ゲーム | 게임 | Παιχνίδια | 游戏 | 遊戲 |
| 1025 | `finance` | Finance | Finance | Finanzas | مالية | Finanças | Финансы | Finanzen | 金融 | 금융 | Οικονομικά | 金融 | 金融 |
| 1026 | `email` | Email | E-mail | Correo | بريد إلكتروني | E-mail | Почта | E-Mail | メール | 이메일 | Email | 邮件 | 郵件 |
| 1011 | `open-source` | Open source | Open source | Código abierto | مفتوح المصدر | Código aberto | Открытый код | Open Source | オープンソース | 오픈 소스 | Ανοιχτός κώδικας | 开源 | 開源 |
| 1012 | `free` | Free | Gratuit | Gratis | مجاني | Grátis | Бесплатно | Kostenlos | 無料 | 무료 | Δωρεάν | 免费 | 免費 |
| 1013 | `paid` | Paid | Payant | De pago | مدفوع | Pago | Платно | Kostenpflichtig | 有料 | 유료 | Επί πληρωμή | 付费 | 付費 |
| 1027 | `trial` | Free trial | Essai gratuit | Prueba gratis | تجربة مجانية | Teste grátis | Пробный период | Testphase | 試用 | 체험판 | Δοκιμή | 试用 | 試用 |
| 1028 | `ads` | Ads | Publicité | Anuncios | إعلانات | Anúncios | Реклама | Werbung | 広告あり | 광고 | Διαφημίσεις | 广告 | 廣告 |
| 1014 | `account` | Account required | Compte requis | Cuenta obligatoria | حساب مطلوب | Conta necessária | Нужен аккаунт | Konto nötig | アカウント必須 | 계정 필요 | Απαιτείται λογαριασμός | 需账号 | 需帳號 |
| 1029 | `web` | Web | Web | Web | ويب | Web | Веб | Web | ウェブ版 | 웹 | Web | 网页版 | 網頁版 |
| 1015 | `ios` | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS | iOS |
| 1016 | `android` | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android | Android |
| 1017 | `desktop` | Desktop | Ordinateur | Escritorio | سطح المكتب | Computador | Компьютер | Desktop | デスクトップ | 데스크톱 | Υπολογιστής | 桌面 | 桌面 |
| 1018 | `extension` | Extension | Extension | Extensión | إضافة | Extensão | Расширение | Erweiterung | 拡張機能 | 확장 프로그램 | Επέκταση | 扩展 | 擴充功能 |
| 1030 | `nonprofit` | Nonprofit | Non lucratif | Sin ánimo de lucro | غير ربحي | Sem fins lucrativos | Некоммерческий | Gemeinnützig | 非営利 | 비영리 | Μη κερδοσκοπικό | 非营利 | 非營利 |
| 1019 | `personal` | Personal | Personnel | Personal | شخصي | Pessoal | Личный | Persönlich | 個人 | 개인 | Προσωπικό | 个人 | 個人 |
| 1020 | `custom` | Customizable | Personnalisable | Personalizable | قابل للتخصيص | Personalizável | Настраиваемый | Anpassbar | カスタマイズ可 | 사용자 지정 가능 | Προσαρμόσιμο | 自定义 | 自訂 |
