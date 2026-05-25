# web-astro-landing

opencode skill for building, reviewing, and modifying public marketing and SEO landing projects with Astro.

## Use When

- Creating or updating Astro landing pages.
- Working with MDX Content Collections for blogs.
- Adding SEO metadata, sitemap, RSS, or robots.txt support.
- Styling landing pages with Tailwind CSS.
- Adding targeted React islands for real interactivity.
- Preparing static Cloudflare Pages deployments.
- Reviewing landing-page CI, testing, or launch readiness.

## Baseline Stack

- Astro for static-first public landing sites.
- Bun for installs, scripts, builds, and tests.
- TypeScript strict mode.
- Tailwind CSS for styling.
- MDX Content Collections for repository-owned blog content.
- Cloudflare Pages publishing static `dist/` output by default.

## Core Rules

- Do not build landing pages as React SPAs.
- Do not add dashboard, admin, authenticated app, backend, or database logic.
- Add React only as narrow Astro islands for genuine interactivity.
- Keep SEO metadata, canonical URLs, sitemap, RSS, and robots.txt production-ready.
- Keep tests under top-level `tests/`, not colocated with `src/` implementation files.
- Never expose secrets through public environment variables or committed source.

## Expected Checks

Landing projects should support this verification baseline:

```bash
bun install --frozen-lockfile
bun run typecheck
bun run lint
bun run test
bun run build
```

## Skill File

The skill instructions live in [`SKILL.md`](./SKILL.md). opencode discovers this repository as an external skill from `~/.agents/skills/web-astro-landing/SKILL.md`.
