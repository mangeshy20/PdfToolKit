<h1 align="center">📄 PDF ToolKit</h1>

<p align="center">
  A free, fast, browser-based PDF platform with <b>48+ tools</b>.<br>
  No sign-up. No uploads. <b>100% client-side</b> — your files never leave your device.
</p>

<p align="center">
  <a href="https://freepdftoolkitt.netlify.app/">
    <img src="https://img.shields.io/badge/Live%20Demo-Open-6366f1?style=for-the-badge&logo=netlify&logoColor=white" alt="Live Demo">
  </a>
  <img src="https://img.shields.io/badge/Tools-48%2B-6366f1?style=for-the-badge" alt="48+ Tools">
  <img src="https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge" alt="MIT License">
  <img src="https://img.shields.io/badge/Build-No%20build%20step-brightgreen?style=for-the-badge" alt="No build step">
</p>

<p align="center">
  <a href="https://github.com/mangeshy20/PdfToolKit/stargazers">
    <img src="https://img.shields.io/github/stars/mangeshy20/PdfToolKit?style=social" alt="GitHub stars">
  </a>
  <a href="https://github.com/mangeshy20/PdfToolKit/issues">
    <img src="https://img.shields.io/github/issues/mangeshy20/PdfToolKit" alt="GitHub issues">
  </a>
</p>

---

## 🔗 Live Demo

**👉 [freepdftoolkitt.netlify.app](https://freepdftoolkitt.netlify.app/)**

> Live and ready to use — no install required. Open the link and start editing PDFs right in your browser.

## 📑 Table of Contents

- [Features](#-features)
- [Tools Available](#-tools-available)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Deployment](#-deployment)
- [How It Works](#-how-it-works)
- [Project Structure](#-project-structure)
- [Themes](#-themes)
- [Browser Support](#-browser-support)
- [Contributing](#-contributing)
- [License](#-license)

## ✨ Features

- **48+ PDF Tools** — Merge, split, compress, convert, rotate, watermark, sign, and more
- **100% Client-Side** — All processing runs in your browser via pdf-lib and PDF.js
- **Zero Server Uploads** — Your files never leave your device
- **No Sign-up Required** — Just open and use, no account needed
- **No Watermarks** — Clean output on every tool
- **10 Color Themes** — Light, Dark, Ocean Blue, Forest Green, Sunset, Rose, Midnight, Lavender, Charcoal, Emerald
- **Fully Responsive** — Works on desktop, tablet, and mobile
- **Search & Filter** — Find any tool instantly with search and category tabs

## 🧰 Tools Available

<details open>
<summary><b>Merge &amp; Organize (6)</b></summary>

Merge PDF · Split PDF · Organize PDF · Rotate PDF · Remove Pages · Extract Pages
</details>

<details>
<summary><b>Convert to PDF (8)</b></summary>

Image to PDF · HTML to PDF · Word to PDF · Excel to PDF · PowerPoint to PDF · Text to PDF · Markdown to PDF · Base64 to PDF
</details>

<details>
<summary><b>PDF to Image (4)</b></summary>

PDF to PNG · PDF to JPG · PDF to TIFF · PDF to BMP
</details>

<details>
<summary><b>PDF to Document (9)</b></summary>

PDF to Word · PDF to Excel · PDF to PowerPoint · PDF to Text · PDF to HTML · PDF to Markdown · PDF to XML · PDF to CSV · PDF to Base64
</details>

<details>
<summary><b>Edit &amp; Enhance (10)</b></summary>

Compress PDF · Watermark · Page Numbers · Edit PDF* · Crop PDF · Resize PDF · Grayscale · Flatten PDF · Metadata · PDF/A
</details>

<details>
<summary><b>Security (4)</b></summary>

Protect PDF · Unlock PDF · Redact PDF* · Sign PDF
</details>

<details>
<summary><b>Extract &amp; Utility (6)</b></summary>

Extract Images · Extract Links · PDF Info · Repair PDF · Compare PDF · OCR PDF*
</details>

> `*` = Coming Soon

## 🛠 Tech Stack

| Technology | Purpose |
|---|---|
| **HTML5 / CSS3 / JS** | Frontend (no framework) |
| **Bootstrap 5** | Layout & responsive grid |
| **Bootstrap Icons** | Icon system |
| **pdf-lib** | Client-side PDF manipulation |
| **PDF.js** | PDF rendering & text extraction |
| **Google Fonts (Inter)** | Typography |

## 🚀 Getting Started

It's a static site — no build step, no dependencies to install.

```bash
# 1. Clone the repository
git clone https://github.com/mangeshy20/PdfToolKit.git

# 2. Enter the project
cd PdfToolKit

# 3. Serve it with any static server
npx serve .
#   or:  python -m http.server 3000

# 4. Open http://localhost:3000 in your browser
```

> 💡 You can also just open `index.html` directly, but a local server is recommended so PDF.js workers load correctly.

## 🌐 Deployment

This project is live on **Netlify**: **[freepdftoolkitt.netlify.app](https://freepdftoolkitt.netlify.app/)**

### Netlify (recommended)

1. Push this repository to GitHub.
2. Go to [Netlify](https://app.netlify.com) → **Add new site** → **Import an existing project**.
3. Connect your GitHub repo (`mangeshy20/PdfToolKit`).
4. Leave the **Build command** empty and set the **Publish directory** to `.`.
5. Click **Deploy** — that's it. No build step needed.

### GitHub Pages

1. Go to **Settings → Pages**.
2. Set **Source** to **Deploy from a branch**.
3. Choose branch **`main`** and folder **`/ (root)`**, then **Save**.
4. Your site goes live at `https://mangeshy20.github.io/PdfToolKit/`.

### Other hosts

Any static host works — **Vercel** or **Cloudflare Pages** too. Leave the build command empty and set the publish directory to `.`.

## ⚙️ How It Works

1. **Upload** — Select or drag & drop your file (up to 50 MB).
2. **Configure** — Set tool-specific options (rotation angle, watermark text, page ranges, etc.).
3. **Process** — Everything runs locally in your browser via pdf-lib / PDF.js.
4. **Download** — Get the result instantly. Nothing is uploaded or stored anywhere.

## 📁 Project Structure

```
PdfToolKit/
├── index.html                  # Homepage with all tools grid
├── favicon.svg                 # Site favicon
├── css/
│   ├── bootstrap.min.css       # Bootstrap 5
│   ├── bootstrap-icons.css     # Bootstrap Icons
│   ├── style.css               # Custom styles + 10 themes
│   ├── tool-page.css           # Tool page styles
│   └── fonts/                  # Bootstrap Icons font files
├── js/
│   ├── bootstrap.bundle.min.js # Bootstrap JS
│   ├── app.js                  # Homepage logic (tabs, search, mega-menu, themes)
│   └── pdf-tools-engine.js     # PDF processing engine for all 48+ tools
└── tools/
    ├── tool-template.html      # Base template for tool pages
    ├── merge-pdf.html          # Individual tool pages (48 total)
    ├── split-pdf.html
    └── ...
```

## 🎨 Themes

10 fully-designed color themes, all driven by CSS custom properties for instant switching:

| Theme | Primary | Theme | Primary |
|---|---|---|---|
| Light | `#6366f1` | Rose | `#e11d48` |
| Dark | `#818cf8` | Midnight | `#38bdf8` |
| Ocean Blue | `#2563eb` | Lavender | `#9333ea` |
| Forest Green | `#16a34a` | Charcoal | `#a78bfa` |
| Sunset | `#ea580c` | Emerald | `#10b981` |

## 🧭 Browser Support

| Chrome | Firefox | Safari | Edge |
|:---:|:---:|:---:|:---:|
| 90+ | 90+ | 15+ | 90+ |

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo
2. Create a branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m "Add my feature"`
4. Push the branch: `git push origin feature/my-feature`
5. Open a Pull Request

Found a bug or have an idea? [Open an issue](https://github.com/mangeshy20/PdfToolKit/issues).

## 📄 License

Released under the **MIT License**. See [LICENSE](LICENSE) for details.

---

<p align="center">
  Built with ❤️ by <b>Mangesh Yadav</b>
</p>

<p align="center">
  ⭐ If you find this project useful, consider giving it a star on
  <a href="https://github.com/mangeshy20/PdfToolKit">GitHub</a>!
</p>
