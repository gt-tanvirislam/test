# Tamvir Islam Platform

Monorepo for the Tamvir Islam personal brand, portfolio, and CMS platform.

## Structure

- `apps/web` — Next.js frontend (public site + admin dashboard)
- `apps/api` — FastAPI backend
- `packages/ui` — shared design system components
- `packages/types` — shared TypeScript types
- `packages/utils` — shared framework-agnostic utilities
- `packages/config` — shared ESLint/TypeScript/Tailwind config
- `docs/` — architecture and engineering documentation

## Getting Started

```bash
pnpm install
cp .env.example apps/web/.env.local   # fill in real values
cp apps/api/.env.example apps/api/.env # fill in real values

pnpm dev:web     # http://localhost:3000
pnpm dev:api     # http://localhost:8000 (requires: cd apps/api && pip install -e ".[dev]")
```

## Documentation

The full architecture and engineering standards are documented across
Phases 2.1–2.11 (see `docs/architecture/`). Every engineering decision in
this codebase traces back to one of those documents — when in doubt,
check there before introducing a new pattern.

## Status

Sprint 0 (infrastructure foundation) complete. See the Sprint 0 report for
details on what's built and what's next.
