# PDFbox

I got tired of sites that make you sign up just to merge two PDFs, so I built this. It's a small browser-based toolkit that handles the PDF tasks I actually run into day to day.

## What it does

- **Merge** — drag in a bunch of PDFs, reorder them, get one file back
- **Extract Pages** — pick specific pages or ranges out of a PDF (e.g. `2, 5-8, 12`)
- **Compress** — strips metadata and optimizes the file to bring the size down

## Your files stay on your device

No uploads. Everything runs in the browser using [pdf-lib](https://pdf-lib.js.org/). I'm not storing anything, and there's no server involved at all.

## How to use it

Open the site, drop your PDF in, done.

Live site: `https://ManuCovr.github.io/pdfbox`

### Page extraction

You can mix and match page numbers and ranges:

```
2          → just page 2
1-5        → pages 1 through 5
2, 10-20   → page 2 and pages 10 through 20
1, 3, 5-8  → pages 1, 3, and 5 through 8
```

## Running it locally

It's a single HTML file, so there's nothing to install or build.

```bash
git clone https://github.com/YOURUSERNAME/pdfbox.git
cd pdfbox
npx serve .
```

Or just open `index.html` directly in your browser.

## Built with

- Vanilla HTML, CSS, JS — no frameworks
- [pdf-lib](https://pdf-lib.js.org/) for all the PDF stuff

## Fork it

1. Fork the repo
2. Go to Settings → Pages → deploy from `main`
3. It'll be live at `https://ManuCovr.github.io/pdfbox`

## License
MIT

```
MIT License

Copyright (c) 2025 Manuel Bernardes

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
