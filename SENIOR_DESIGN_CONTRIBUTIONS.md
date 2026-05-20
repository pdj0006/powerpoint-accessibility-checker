# Senior Design Contributions

This project grew out of Auburn COMP 4710 Senior Design work on an accessibility checker for PowerPoint presentations.

## Group Repository

Organization:

```text
accessibilitychecker25-arch
```

Active combined project repo:

```text
https://github.com/accessibilitychecker25-arch/AI-ChatBot-Education-2026
```

Related group repos:

```text
https://github.com/accessibilitychecker25-arch/Accessibility-Checker
https://github.com/accessibilitychecker25-arch/Accessibility-Checker-BE
```

My main contribution branch:

```text
Philip-Branch
```

The branch comparison against the group repo's current `main` branch is documented in
[PHILIP_BRANCH_COMPARISON.md](PHILIP_BRANCH_COMPARISON.md).

## Project Goal

The senior design project extended an accessibility checker so it could handle PowerPoint presentations, analyze slide-level accessibility problems, and provide remediation output aligned with WCAG 2.1 Level AA expectations.

## Contribution Timeline

### Cycle 1

Cycle 1 focused on establishing PowerPoint support and the upload/analyze/download workflow:

- accepted PowerPoint files through the frontend/backend flow
- parsed PPTX content using Office Open XML structure
- detected missing slide titles and image alt text issues
- prepared backend support for future remediation and AI-assisted alt text

Local artifacts found:

```text
C:\Users\hyper\Downloads\Cycle 1 Written Report.docx
C:\Users\hyper\Downloads\Cycle 1 Presentation.pptx
```

### Cycle 2

Cycle 2 work expanded backend functionality and remediation depth:

- added color contrast analysis for PPTX text
- added remediation logic for low-contrast text
- improved reporting so contrast issues identify slide-level context
- added smoke tests for contrast analysis and remediation
- improved local AI alt text support

Representative commits from `Philip-Branch`:

```text
21436a3 Add color contrast analysis and remediation for PPTX text
7433b34 Improve color contrast handling and reporting
```

### Later Integration And Deployment Work

Additional work on `Philip-Branch` helped connect the backend and frontend deployment path:

- restored PowerPoint backend upload handling
- centralized CORS handling for deployed endpoints
- fixed Vercel routing and frontend upload routing
- pointed the frontend to the working backend deployment

Representative commits from `Philip-Branch`:

```text
42659eb Restore PowerPoint backend upload handler
d6fdd4f Fix Vercel frontend upload routing
97becd5 Fix Vercel base href for preview deploy
22f660b Restore backend Vercel API routing config
91b17cd Point frontend proxy to working backend deployment
```

## Technical Work Highlighted In This Portfolio Repo

This portfolio repo focuses on the backend PowerPoint accessibility work:

- FastAPI upload/download API
- PPTX zip/XML parsing with `lxml`
- color contrast calculations
- WCAG-style contrast threshold checks
- remediation that changes low-contrast text colors
- optional local AI vision support for generating image alt text
- smoke test coverage for contrast detection/remediation

## Notes

The original senior design repository is a team project. This portfolio repo isolates and documents the backend accessibility engineering pieces most relevant to my contribution area while preserving attribution to the group repository.
