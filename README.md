# 🫐 נוי השדה — FreshEye

Field inventory management for produce retail: a clerk photographs a stand, an AI
vision model estimates unit count and weight per product, and the app rolls that up
into per-branch, per-department inventory with reorder alerts — for clerks, branch
managers, and executives.

## Repo layout

- **`fresheye-store-pwa/`** — the app (Vite + React 18 + TypeScript + Tailwind, PWA).
  Role-based (clerk / branch manager / executive), full RTL Hebrew, matching the
  Noy HaSade brand design system. See `fresheye-store-pwa/README.md` for the screen
  list, what's implemented vs. deferred, and the vision-AI seam to replace with a
  real backend.
- **`docs/`** — the client pilot package (Hebrew) for נוי השדה.

## Run the app

```bash
cd fresheye-store-pwa
npm install
npm run dev      # http://localhost:5173 — demo mode, full app works with no backend
npm run build    # strict tsc + vite build + PWA service worker
```

Requires Node.js 18+ (20 LTS recommended).

Demo login: pick any of the three seed users (clerk / branch manager / executive) —
each gets a different navigation and home screen matching their role.
