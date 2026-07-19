<div align="center">

![cli-mage](cli-mage.png)

# cli-mage ✦

**A magical CLI tool that converts images to ASCII art in your terminal.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
[![Node.js](https://img.shields.io/badge/Node.js-%3E%3D18-339933.svg?logo=node.js&logoColor=white)](https://nodejs.org)
[![Offline](https://img.shields.io/badge/works-offline-blue.svg)](#requirements)

```
npm install -g github:yerettegroup/cli-mage
```

</div>

---

## Usage

```
cli-mage <image> [options]
```

```
cli-mage photo.png
cli-mage photo.png --gradient
cli-mage photo.png --braille -w 200
cli-mage photo.png --save mage.gif
cli-mage photo.png --save mage.svg
cli-mage photo.png --save mage.html
cli-mage animation.gif
cli-mage qr "https://yerettegroup.com"
curl https://example.com/image.png | cli-mage
```

---

## Options

| Flag | Description |
|---|---|
| `-w, --width <n>` | Output width in characters (default: 100) |
| `--no-color` | Disable color output |
| `-i, --invert` | Invert brightness |
| `-d, --detailed` | Use a larger, more detailed character set |
| `-g, --gradient` | Rainbow gradient color (ignores source colors) |
| `-e, --edge` | Edge detection mode (Sobel filter) |
| `--braille` | Render using Unicode Braille characters (2× resolution) |
| `--block` | Render using block characters ░▒▓█ |
| `-a, --animate` | Animate in terminal — Ctrl+C to stop |
| `-o, --output <file>` | Save plain-text output to file |
| `--save <file>` | Save as `.html`, `.svg`, or `.gif` |

---

## QR Codes

```
cli-mage qr <text or URL> [options]
```

| Flag | Description |
|---|---|
| `--no-color` | Disable color output |
| `-o, --output <file>` | Save plain-text output to file |
| `--save <file>` | Save as `.html` or `.svg` |

Works fully offline — no internet required.

---

## Requirements

- Node.js 18 or later

---

## License

cli-mage is licensed under the [MIT License](./LICENSE).

Contact: [hello@yerettegroup.com](mailto:hello@yerettegroup.com)

<div align="center">

![yerette](mage.svg)

</div>
