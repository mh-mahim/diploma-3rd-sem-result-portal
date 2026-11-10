# Architecture Decision Records (ADRs)

## ADR-001: Pre-Baking Clean JSON Data into Single-Page Architecture
- **Date**: 2026-11-10
- **Context**: The BTEB results endpoint provides server-rendered RSC chunks which cannot be fetched client-side directly due to CORS restrictions and bandwidth overhead.
- **Decision**: Parse and sanitize the raw 79-student dataset down to the verified 33 students with active 3rd Semester results, pre-baking it directly into `data/results.json` and inlined as default fallback in `index.html`.
- **Consequence**: Ultra-fast performance, zero network delay, 100% offline support, and hassle-free deployment to any static host (GitHub Pages, Netlify, Vercel).

## ADR-002: Definition of Drop Out Status
- **Date**: 2026-11-10
- **Context**: The user specified: "jodi karo 4 subject referd pao tader pase ullekh koiro je se dorp out".
- **Decision**: In BTEB regulation, students who fail in 4 or more subjects in an exam face semester drop / drop out. All students with >= 4 failed subjects are tagged with the prominent `Drop Out` badge, while explicitly breaking out students with exactly 4 subjects as well as 4+ subjects in the top KPI summary.
