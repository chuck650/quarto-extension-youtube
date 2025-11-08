# 📦 My Awesome Quarto Extension

A Quarto extension for [briefly describe the main function, e.g., "creating custom LaTeX environments" or "adding interactive maps"]. This extension helps you [mention a key benefit, e.g., "maintain brand consistency" or "embed interactive components"].

[![Quarto Extension](https://img.shields.io/badge/Quarto-Extension-blue.svg)]([https://quarto.org/docs/extensions/](https://quarto.org/docs/extensions/))
[![GitHub license](https://img.shields.io/github/license/YOUR-ORG/YOUR-REPO?color=blue)](LICENSE)

---

## 💻 Installation

Install the extension by running the following command in your project's terminal:

```bash
quarto install extension YOUR-ORG/YOUR-REPO
```

For example, if your GitHub username is `johndoe` and the repository is `fancy-shortcodes`, the command would be:

```bash
quarto install extension johndoe/fancy-shortcodes
```

---

## 🛠️ Usage

Once installed, you can use the extension in any Quarto document (`.qmd`) by adding the extension's name (which corresponds to the folder name inside `_extensions/`) to the appropriate YAML key.

### Configuration

Add the extension to your YAML front matter. If it's a filter or shortcode extension, use the `filters` key:

```yaml
---
title: "My Document"
format: html
filters:
  - my-awesome-extension # Replace with your actual extension folder name
---
```

### Demonstration

Here is how to invoke the core functionality of the extension in your document:

**Input (`.qmd`):**

```markdown
::alert-box[
This is an important note displayed using the extension's custom div.
]
```

**Output (Expected Result):**

> The content will render as a prominent, styled callout box, demonstrating the successful application of the extension's CSS and/or Lua filter logic.

---

## ⚙️ Options

If your extension supports configuration, document them here. If not, you can remove this section.

This extension supports the following document options, which can be set in the YAML front matter:

| Option         | Type    | Default     | Description                                      |
|:-------------- |:------- |:----------- |:------------------------------------------------ |
| `alert-color`  | string  | `"#E74C3C"` | The background color used for the alert box.     |
| `alert-shadow` | boolean | `true`      | Set to `false` to remove the drop shadow effect. |

---

## ⚖️ License and Contribution

This extension is released under the **MIT License**.

We welcome contributions from the community! If you have suggestions, find a bug, or want to add a feature, please feel free to:

1. **Open an Issue** to discuss the change.
2. **Submit a Pull Request** with your proposed changes.
