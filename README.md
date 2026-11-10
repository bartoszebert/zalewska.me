# zalewska.me

One-page site built with Astro (static output, zero client JS). Copy lives in `src/content/site.ts`.

```sh
npm install
npm run dev      # http://localhost:4321
npm run build    # -> dist/
```

## Deploy

Vercel Git integration: every push to `main` deploys production, every other branch/PR gets a preview URL.
No GitHub Actions and no `vercel.json` needed — Vercel detects Astro and runs `npm run build` → `dist/`.

One-time setup:
1. Vercel → Add New → Project → import this GitHub repo (framework preset: Astro, defaults are fine).
2. Project → Settings → Domains → add `zalewska.me` (and `www.zalewska.me` redirecting to it),
   then set the DNS records Vercel shows at the domain registrar.
