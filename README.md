# Resume Studio

A developer-focused CV generator with live preview, accent color theming, EN/FR language toggle, PDF export, and JSON save/load — all in a single self-contained page. No build step, no framework, no database.

![Preview](https://img.shields.io/badge/stack-HTML%20%2B%20CSS%20%2B%20JS-0e7c66?style=flat-square)

## Features

- **Live preview** — edits reflect instantly on the A4 resume layout
- **PDF export** — generates a clean, print-ready PDF via html2canvas + jsPDF
- **Save / Load** — export your data as JSON and reload it later
- **Accent themes** — 7 color presets, applied globally to both the UI and the resume
- **EN / FR** — toggle section labels between English and French
- **Photo upload** — add a profile photo (stored as base64 in your JSON)
- **Responsive form** — collapsible preview pane for focused editing

## Getting started

### Prerequisites

- [Node.js](https://nodejs.org/) v14 or newer (no npm packages to install)

### Run locally

```bash
git clone https://github.com/thomasdqr/resume-studio.git
cd resume-studio
npm start
```

Then open **http://localhost:3000** in your browser.

The port can be overridden with the `PORT` environment variable:

```bash
PORT=8080 npm start
```

## Usage

1. Fill in your details in the left-hand form panel.
2. Adjust the accent color and language in the top bar.
3. Click **Download PDF** to export your resume.
4. Click **Save data** to export your form state as a `.json` file — reload it anytime with **Load data**.

## Project structure

```
resume-studio/
├── index.html   # The entire app — form, preview, and logic
├── server.js    # Zero-dependency Node.js static file server
└── package.json
```

## License

MIT
