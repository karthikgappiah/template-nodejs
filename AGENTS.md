# AGENTS.md

Node.js web app template. Currently scaffolding only (Biome, Lefthook, pnpm) — no app source yet.

## Commands

- `pnpm lint` — Biome check + auto-fix (formatter + linter; no separate Prettier/ESLint)
- `pnpm install` — installs deps, runs `lefthook install` via `prepare`
- Package manager: pnpm@10.32.1 (pinned in package.json), not npm/yarn

## Conventions

- Formatting: tabs, double quotes (JS) — enforced by Biome, not manual
- Pre-commit (Lefthook): auto-lints and re-stages staged files; don't hand-format to match
- Biome/Lefthook ignore `.agents/`, `.claude/`, `.cursor/`
- `CLAUDE.md` symlinks to this file — edit `AGENTS.md`, not `CLAUDE.md`
