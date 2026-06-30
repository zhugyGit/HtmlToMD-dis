# HtmlToMD

🌐 [English](README_EN.md) | [中文](README.md) —— 📦 [Download Browser Extension](https://pan.quark.cn/s/adaa6c4bc491)

A Python desktop tool that converts HTML to Markdown. Supports URL fetching and local file conversion, with automatic article content extraction and image downloading.

![Preview](./images/pic_zh_1.png)

## Features

- **Dual Input Modes** — Enter a URL or select a local HTML file
- **Smart Content Extraction** — Automatically removes ads, navigation, sidebars, and other clutter (powered by `trafilatura` + `BeautifulSoup`)
- **Auto Image Download** — Downloads web images to a local `images/` directory and replaces references in the Markdown output
- **Multi-site Support** — Built-in optimizations for Juejin, CSDN, Zhihu, Jianshu, SegmentFault, OSChina, WeChat Official Accounts, WordPress, and more
- **Anti-scraping Handling** — Googlebot UA fallback, `cloudscraper` for Cloudflare bypass, custom Cookie support
- **SPA Compatibility** — Detects SPA shell pages and retries automatically
- **GUI Interface** — Clean Tkinter-based graphical interface for intuitive operation

## Installation

Download the [Release](https://github.com/zhugyGit/HtmlToMD-dis/releases) version matching your system.

> macOS

```
 Apple Silicon  ->  HtmlToMD-mac-arm64.zip
 Intel Chip     ->  HtmlToMD-mac-x86_64.zip
```

> Windows

```
HtmlToMD-win-x86_64.zip
```

## Quick Start

```bash
Double-click the package to run.
```

Once launched, two conversion methods are available:

1. **URL Input** — Enter a link in the URL tab and click "Start Conversion"
2. **Local File** — Switch to the "Local File" tab, select an HTML file, and convert

Use the "Advanced Settings" panel to configure Cookies (required for sites that need login). Check "Download images to local" to save images to the `images/` folder inside the output directory.

## Supported Sites

Juejin · CSDN · Zhihu · Jianshu · SegmentFault · OSChina · WeChat Official Account · WordPress · Generic Articles

## Tech Stack

Python 3 · Tkinter · BeautifulSoup · trafilatura · markdownify · requests

## Possible Conversion Failures

![Possible Conversion Failures](./images/pic_zh_2.png)

### Adding Cookies

![Adding Cookies](./images/pic_zh_3.png)

## Comparison

**Markdown Output**
![Linux一口气删掉近4000行代码！](./images/pic_zh_4.png)

---

**Original Page**
![Linux一口气删掉近4000行代码！](./images/pic_zh_5.png)

## Export Directory Structure

![Export Directory Structure](./images/pic_zh_6.png)

## License

[MIT](LICENSE)
