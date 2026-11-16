English | [简体中文](README.zh-Hans.md)

# Sticker Tags

**Universal attribute tags: an open standard by [Nav.cc](https://nav.cc). Version 1.1.**

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
<img src="svg/ai.svg" width="32" height="32" alt="AI" title="AI">
<img src="svg/social.svg" width="32" height="32" alt="Social" title="Social">
<img src="svg/media.svg" width="32" height="32" alt="Media" title="Media">
<img src="svg/game.svg" width="32" height="32" alt="Games" title="Games">
<img src="svg/finance.svg" width="32" height="32" alt="Finance" title="Finance">
<img src="svg/email.svg" width="32" height="32" alt="Email" title="Email">
<img src="svg/open-source.svg" width="32" height="32" alt="Open source" title="Open source">
<img src="svg/free.svg" width="32" height="32" alt="Free" title="Free">
<img src="svg/paid.svg" width="32" height="32" alt="Paid" title="Paid">
<img src="svg/trial.svg" width="32" height="32" alt="Free trial" title="Free trial">
<img src="svg/ads.svg" width="32" height="32" alt="Ads" title="Ads">
<img src="svg/account.svg" width="32" height="32" alt="Account required" title="Account required">
<img src="svg/web.svg" width="32" height="32" alt="Web" title="Web">
<img src="svg/ios.svg" width="32" height="32" alt="iOS" title="iOS">
<img src="svg/android.svg" width="32" height="32" alt="Android" title="Android">
<img src="svg/desktop.svg" width="32" height="32" alt="Desktop" title="Desktop">
<img src="svg/extension.svg" width="32" height="32" alt="Extension" title="Extension">
<img src="svg/nonprofit.svg" width="32" height="32" alt="Nonprofit" title="Nonprofit">
<img src="svg/personal.svg" width="32" height="32" alt="Personal" title="Personal">
<img src="svg/custom.svg" width="32" height="32" alt="Customizable" title="Customizable">
</p>

Directories, start pages, catalogs and app stores put a row of small badges on each card: is it free, is there a phone app, does it need an account, is there something to be careful about. Sticker Tags gives those badges one shared vocabulary. Each tag has an identifier, a permanent number (TID), names in twelve languages and an exact meaning, and is drawn as a rounded square that can still be told apart at 14 pixels.

- **A Nav.cc project:** Sticker Tags is a project of [Nav.cc](https://nav.cc), which edits and maintains it.
- **The standard:** the canonical text is at https://nav.cc/standards/sticker-tags/. This repository holds a copy: [STANDARD.md](STANDARD.md) (English, canonical) and [STANDARD.zh-Hans.md](STANDARD.zh-Hans.md) (简体中文).
- **First batch:** 30 tags in six groups. More will follow.

## What is here

| Path | Contents |
| --- | --- |
| `STANDARD.md`, `STANDARD.zh-Hans.md` | The text of the standard. |
| `svg/` | One SVG file per tag, as Nav.cc draws it. |
| `tags.json` | Every tag: TID, identifier, group, names in twelve languages, meaning and SVG file. |

## Using the tags

The quickest way: nav.cc serves every tag as an image, always in its current drawing. The standard's page has [each tag's code to copy](https://nav.cc/standards/sticker-tags/#use).

```html
<img src="https://nav.cc/sticker-tags/free.svg" width="20" height="20" alt="Free" title="Free">
```

Replace `free` with any identifier in `tags.json` (`image` gives each address). Show tags at 14 pixels or more. You can also copy the files in `svg/` into your own project.

Use them for any purpose, including commercial use, on one condition: credit Nav.cc as the source, once on the page:

```html
Tags: <a href="https://nav.cc/standards/sticker-tags/">Sticker Tags by Nav.cc</a>
```

The text, the vocabulary, the glyphs and the data are licensed under [CC BY 4.0](LICENSE). How you use the tags, such as which object gets which tag and how you show them, is up to you.

## Proposing a tag or a change

New tags, clearer meanings, better glyphs and translations are welcome: open an [issue](https://github.com/nav-cc/sticker-tags/issues/new/choose) or a pull request. Nav.cc edits the standard and decides whether a proposal is adopted. See [CONTRIBUTING.md](CONTRIBUTING.md).
