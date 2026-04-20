# PDFbox

A free, open-source PDF toolkit that runs entirely in your browser. No file uploads, no accounts, no watermarks.

## Features

- **Merge** — combine multiple PDFs into a single file, in any order
- **Extract Pages** — pull out specific pages or ranges from a PDF (e.g. `2, 5-8, 12`)
- **Compress** — reduce file size by stripping metadata and optimizing object streams

## Privacy

Nothing ever leaves your device. All processing is done client-side using [pdf-lib](https://pdf-lib.js.org/), a WebAssembly-powered library that runs directly in the browser. No server, no cloud, no tracking.

## Usage

Just open the site and drop your PDF in. No installation required.

Live site: `https://YOURUSERNAME.github.io/pdfbox`

### Page extraction syntax

The page extractor supports comma-separated page numbers and ranges:

```
2          → extract page 2 only
1-5        → extract pages 1 through 5
2, 10-20   → extract page 2 and pages 10 through 20
1, 3, 5-8  → extract pages 1, 3, and 5 through 8
```

## Self-hosting

This is a single HTML file with no build step and no dependencies to install.

```bash
git clone https://github.com/YOURUSERNAME/pdfbox.git
cd pdfbox
# open index.html in your browser, or serve it locally:
npx serve .
```

That's it. No Node, no bundler, no config.

## Tech stack

- Vanilla HTML, CSS, and JavaScript
- [pdf-lib](https://pdf-lib.js.org/) for all PDF manipulation (loaded from cdnjs)
- No frameworks, no build tools

## Deploying your own fork

1. Fork this repository
2. Go to Settings → Pages
3. Set source to `main` branch, `/ (root)`
4. Your instance will be live at `https://YOURUSERNAME.github.io/pdfbox`

## License

MIT — do whatever you want with it.
