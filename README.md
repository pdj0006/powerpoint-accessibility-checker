# PowerPoint Accessibility Checker

FastAPI backend for auditing and remediating PowerPoint accessibility issues.

This repo is a portfolio-focused extraction of my Auburn COMP 4710 Senior Design accessibility checker work. The group project lives under the `accessibilitychecker25-arch` GitHub organization, and my main contribution branch was `Philip-Branch`.

The project checks presentation files for:

- missing slide titles
- weak list formatting
- missing image alt text
- low color contrast against WCAG-style thresholds

It can also generate remediated `.pptx` output by adding fallback alt text and improving low-contrast text colors.

## Why This Is Portfolio-Worthy

This is a practical accessibility engineering project. It combines backend API work, Office Open XML parsing, file upload/download flows, automated remediation, and optional local AI-assisted alt-text generation.

## Senior Design Context

This work came from a team senior design project focused on helping Auburn University users identify and improve accessibility issues in PowerPoint presentations. My contribution area centered on backend PowerPoint analysis and remediation, especially:

- PPTX text color contrast analysis
- automated color contrast remediation
- PowerPoint upload and processing flow
- backend/frontend routing and deployment fixes
- production API connection fixes for the deployed frontend

More detail is in [SENIOR_DESIGN_CONTRIBUTIONS.md](SENIOR_DESIGN_CONTRIBUTIONS.md), including the
[`Philip-Branch` comparison](PHILIP_BRANCH_COMPARISON.md) against the group repo's main branch.

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
