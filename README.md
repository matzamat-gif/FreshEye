# 🫐 FreshEye

Photo-based produce inventory management: the branch manager photographs the stand,
the system estimates quantity and weight per item, and computes the gap vs. the
branch's daily quota.

## Repo layout

- **`fresheye-store-pwa/`** — the store-layer PWA (Vite + React 18 + TypeScript).
  Full 4-step loop: camera → review/confirm → gap vs quota → submit.
  All CV is stubbed behind `src/lib/cv-contract.ts`, so it runs in demo mode
  with no backend and no validated model.
- **`docs/`** — the client pilot package (Hebrew) for נוי השדה.

## Run the app

```bash
cd fresheye-store-pwa
npm install
npm run dev      # http://localhost:5173 — demo mode, full loop works offline-first
npm run build    # strict tsc + vite build + PWA service worker
```

Requires Node.js 18+ (20 LTS recommended).

See `fresheye-store-pwa/README.md` for what's built, what's stubbed, and the CV seam to respect.
