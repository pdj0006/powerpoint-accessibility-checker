# PowerPoint Accessibility Checker

FastAPI backend for auditing and remediating PowerPoint accessibility issues.

The project checks presentation files for:

- missing slide titles
- weak list formatting
- missing image alt text
- low color contrast against WCAG-style thresholds

It can also generate remediated `.pptx` output by adding fallback alt text and improving low-contrast text colors.

## Why This Is Portfolio-Worthy

This is a practical accessibility engineering project. It combines backend API work, Office Open XML parsing, file upload/download flows, automated remediation, and optional local AI-assisted alt-text generation.

## Tech Stack

- Python
- FastAPI
- lxml
- Office Open XML / `.pptx` internals
- Optional local BLIP image captioning
- Optional PowerPoint or LibreOffice conversion for legacy `.ppt`

## Run Locally

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn app:app --reload
```

Open:

```text
http://localhost:8000
```

## Tests

Run the contrast smoke test:

```bash
python test_color_contrast.py
```

Generated uploads, outputs, local model files, and sample decks are intentionally ignored so the repository stays clean and safe for public GitHub.
