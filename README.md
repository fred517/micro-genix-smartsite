# Micro‑Genix Smart Site (Next.js)

A production‑grade, **AI‑and‑SEO‑ready** starter for Micro‑Genix, using Next.js 15 App Router.

## Why this stack
- Built‑in `/robots.txt` and `/sitemap.xml` via Next metadata routes
- Opinionated SEO metadata + JSON‑LD utilities (`lib/seo.tsx`)
- Operator calculators (SVI, mass‑balance, RAS/WAS, clarifier loading)
- Stubbed AI endpoint at `/api/assist` for LLM features (RAG, Q&A, form helper)
- Tokenised CSS variables for brand alignment
- Accessible structure, core‑web‑vitals friendly

## Quickstart
```bash
npm install
cp .env.example .env.local   # set NEXT_PUBLIC_SITE_URL, GA_MEASUREMENT_ID, OPENAI_API_KEY
npm run dev
```

## Deploy
- Vercel, Netlify, or any Node 18+ host.
- Ensure `NEXT_PUBLIC_SITE_URL` is the public URL for correct sitemap canonicalisation.

## Extend
- Replace tokens in `app/globals.css` with official brand colours and fonts.
- Fill out pages under `/solutions`, `/products`, `/case-studies`.
- Use `OrgJsonLd` and `ProductJsonLd` components to add rich schema.
- Wire `/api/assist` to your LLM provider for AI features (on‑page explainers, content drafting, calculator coaching).

## Security & Perf
- Keep Next.js ≥ 15.2.3 to include critical security fixes.
- Target **INP < 200ms**, LCP < 2.5s, CLS < 0.1.
- Add GA4 and Search Console; generate a core web vitals dashboard.
