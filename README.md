# Quarto YouTube Video Extension

A Quarto extension for embedding YouTube videos in your documents.

[![Quarto Extension](https://img.shields.io/badge/Quarto-Extension-blue.svg)](https://quarto.org/docs/extensions/)
[![Render and Test](https://github.com/chuck650/quarto-extension-youtube/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/chuck650/quarto-extension-youtube/actions/workflows/test.yml)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/chuck650/quarto-extension-youtube/blob/main/LICENSE)

---

## 💻 Installation

Install the extension by running the following command in your project's terminal:

```bash
quarto install extension chuck650/quarto-extensions-youtube
```

---

## 🛠️ Usage

To embed a YouTube video, first add video metadata to your document's YAML front matter. Then, use the `youtube_video` shortcode to embed the video.

### Example

**Input (`.qmd`):**

```yaml
---
title: "My Document"
format: html
videos:
  - title: Quarto Crash Course
    url: https://www.youtube.com/watch?v=_VKxTPWDhA4
    author: Posit PBC
    channel: https://www.youtube.com/@PositPBC
    video_id: _VKxTPWDhA4
    description: Create Professional Reports, Dashboards & Websites w/ Markdown & Python Code!
---

Embed a video like this:

`{{< youtube_video _VKxTPWDhA4 >}}`

On rendering, the result looks like this:

{{< youtube_video _VKxTPWDhA4 >}}
```

---

## ⚖️ License and Contribution

This extension is released under the **MIT License**.

We welcome contributions from the community! If you have suggestions, find a bug, or want to add a feature, please feel free to:

1. **Open an Issue** to discuss the change.
2. **Submit a Pull Request** with your proposed changes.
