# Philip Branch Comparison

This note documents the comparison between the senior design group repository's `main` branch and the `Philip-Branch` contribution branch.

## Source Repository

```text
https://github.com/accessibilitychecker25-arch/AI-ChatBot-Education-2026
```

Compared refs:

```text
main
origin/Philip-Branch
```

Merge base:

```text
713a719314fc3e719ba104af860312523514650f
```

## Branch-Only Commits

These commits were present on `Philip-Branch` and not on `main` at the time of comparison:

```text
91b17cd Point frontend proxy to working backend deployment
22f660b Restore backend Vercel API routing config
42659eb Restore PowerPoint backend upload handler
97becd5 Fix Vercel base href for preview deploy
d6fdd4f Fix Vercel frontend upload routing
7433b34 Improve color contrast handling and reporting
21436a3 Add color contrast analysis and remediation for PPTX text
```

## Diff Summary

Comparing `main..origin/Philip-Branch` showed:

```text
44 files changed, 707 insertions(+), 2696 deletions(-)
```

The file list included backend API routes, the Python PowerPoint analyzer, contrast smoke tests, Angular upload UI files, environment configuration, and Vercel deployment config.

## Main Contribution Areas

### PowerPoint Color Contrast

The branch added and improved PPTX text contrast analysis and remediation logic. This work included contrast calculations, slide-level issue reporting, and smoke-test coverage for contrast detection/remediation.

Representative commits:

```text
21436a3 Add color contrast analysis and remediation for PPTX text
7433b34 Improve color contrast handling and reporting
```

### PowerPoint Upload Handling

The branch restored and adjusted backend PowerPoint upload handling for the deployed app path, including API route support and shared analyzer logic.

Representative commit:

```text
42659eb Restore PowerPoint backend upload handler
```

### Frontend And Deployment Routing

The branch included practical integration work to make the frontend communicate with the working backend deployment and to repair Vercel routing/base-href behavior.

Representative commits:

```text
d6fdd4f Fix Vercel frontend upload routing
97becd5 Fix Vercel base href for preview deploy
22f660b Restore backend Vercel API routing config
91b17cd Point frontend proxy to working backend deployment
```

## Relationship To Current Main

The group repo's `main` branch contains later integration work after `Philip-Branch`, including deployment changes for Hugging Face Spaces and additional CORS/API work. This personal portfolio repo focuses on the backend PowerPoint accessibility engineering pieces from the `Philip-Branch` contribution line while keeping the original group repository attribution visible.
