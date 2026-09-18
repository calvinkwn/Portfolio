# Portfolio Website

A single-page HTML/CSS portfolio site. No build step, no dependencies — just one file.

## How to publish it on GitHub Pages (free custom-ish URL)

1. Create a new repository on GitHub (e.g. `your-username.github.io` for a root URL, or any name like `portfolio` for a project URL).
2. Upload `index.html` (and this `README.md` if you want) to the repo — either drag-and-drop on github.com, or via git:
   ```
   git init
   git add .
   git commit -m "Initial portfolio"
   git branch -M main
   git remote add origin https://github.com/your-username/your-repo.git
   git push -u origin main
   ```
3. On GitHub, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute or two — GitHub will give you a live URL:
   - `https://your-username.github.io/` (if the repo is named `your-username.github.io`)
   - `https://your-username.github.io/your-repo/` (for any other repo name)

That's it — no build tools needed, since it's plain HTML/CSS.

## Editing later

Everything (HTML, CSS, fonts via Google Fonts CDN) lives in `index.html`. Colors are defined once near the top of the `<style>` block as CSS variables (`--paper`, `--ink`, `--blue-mid`, etc.) — change those to restyle the whole site.
