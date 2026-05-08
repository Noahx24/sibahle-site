# Sibahle Digital — Website

**Stack:** React 19 + Vite + GitHub Pages

**Live site:** https://sibahledigital.co.za
**Deployment branch:** `gh-pages`
**Source branch:** `main` (or your working branch)

---

## After every update

```bash
npm run build
npm run deploy
```

Site updates within 1–2 minutes of running deploy.

---

## Local development

```bash
npm install       # first time only
npm run dev       # starts local server at http://localhost:5173
```

---

## File to edit

All website content lives in one file:

```
src/App.jsx
```

Design tokens (colours, spacing) are in the `T` object at the top of App.jsx.

---

## Deployment explained

| Command          | What it does                                      |
|------------------|---------------------------------------------------|
| `npm run build`  | Compiles React → static HTML/CSS/JS into `dist/` |
| `npm run deploy` | Pushes `dist/` to the `gh-pages` branch on GitHub |

GitHub Pages serves the `gh-pages` branch automatically.
The custom domain `sibahledigital.co.za` is set via the `homepage`
field in `package.json` and your DNS settings.

---

## If the site doesn't update after deploy

1. Check GitHub → Settings → Pages — confirm source is `gh-pages` branch
2. Wait 2–3 minutes and hard refresh (Ctrl+Shift+R / Cmd+Shift+R)
3. Check the Actions tab on GitHub for any deploy errors

---

## Never edit the `gh-pages` branch directly.
## Always edit `main`, build, then deploy.
