# MedAbroad — MBBS Abroad Landing Page

Astro landing page for a Hyderabad-based educational consultancy: MBBS admissions in Vietnam & Georgia.

## 🚀 Project Structure

```text
/
├── public/
├── src/
│   ├── components/   # Topbar, Header, Hero, Stats, Why, Universities, Process, Contact, Footer
│   ├── layouts/      # BaseLayout.astro
│   ├── pages/        # index.astro
│   └── styles/       # global.css
└── package.json
```

## 🧞 Commands

| Command           | Action                                      |
| ----------------- | ------------------------------------------- |
| `npm install`     | Install dependencies                        |
| `npm run dev`     | Dev server at `localhost:4321`              |
| `npm run build`   | Build static site to `./dist/`              |
| `npm run preview` | Preview the build locally                   |
| `npm run deploy`  | Build + deploy to Cloudflare Pages (wrangler) |

## ☁️ Deploy to Cloudflare Pages

**Option A — Git integration (recommended):**
1. Push this repo to GitHub/GitLab.
2. Cloudflare Dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
3. Build settings:
   - Framework preset: **Astro**
   - Build command: `npm run build`
   - Build output directory: `dist`

**Option B — Direct upload via Wrangler:**
```sh
npx wrangler login        # one-time auth
npm run deploy            # builds and deploys ./dist
```

Static output is used by default — no adapter needed. If you later add SSR/API routes,
install the adapter: `npx astro add cloudflare`.

## 📞 Contact

- 95026 44931 / 81868 47470
- Hyderabad, Telangana, India
