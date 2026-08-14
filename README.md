# HAQ v2 — working MVP

A clean React + Vite implementation of the HAQ civic-assistance MVP.

## Requirements
- Node.js 20.19+ (or Node 22.12+) for current Vite.
- npm.

## Run
```bash
npm install
npm run dev
```
Open the localhost address printed by Vite.

## Production build
```bash
npm run build
npm run preview
```

## Important architecture note
This version is deliberately runnable without an API key. The case-understanding layer uses deterministic demo-safe logic so the full product journey can be demonstrated offline.

For production AI, replace `demoAnalyze()` with a server-side `/api/understand` endpoint. Never expose a provider API key in browser code.

## Included
- Responsive HAQ shell
- Start-a-case wizard
- Category selection
- Neutral understanding/review
- Facts / claims / missing information
- Evidence selection and local demo metadata
- Timeline
- Next-step options
- Complaint editor/copy
- Case creation
- Case dashboard
- Evidence Locker
- Justice Map (aggregated demo)
- Status/resolution
- Export cases
- Restore demo data
- LocalStorage persistence
- English/Roman Urdu input-ready UX
