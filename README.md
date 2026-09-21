# Fara Fatima — Portfolio

Personal portfolio site. One self-contained `index.html` file: no build step, no dependencies, no framework. Works offline except for the Google Fonts request.

## Files

```
index.html    the whole site
resume.pdf    optional — the Résumé button links here
README.md     this file
```

## Hosting on GitHub Pages

**1. Create the repository**

On github.com click **New repository**. Name it `farafatima26.github.io` (replace with your own GitHub username — the `.github.io` part must match exactly). Make it **Public** and leave "Add a README" unchecked.

**2. Push the files**

```bash
cd portfolio
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin https://github.com/farafatima26/farafatima26.github.io.git
git push -u origin main
```

**3. Turn on Pages**

In the repo go to **Settings → Pages**. Under "Build and deployment", set Source to **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**.

**4. Wait about a minute**

The site goes live at `https://farafatima26.github.io`. Every future `git push` redeploys it automatically.

### If you'd rather not use the username repo

Name the repo anything (e.g. `portfolio`) and follow the same steps. The URL becomes `https://farafatima26.github.io/portfolio/` instead. Everything still works — all links in the page are relative.

## Adding your résumé PDF

The **Résumé** button in the sidebar points at `resume.pdf`. Drop your PDF in this folder with that exact filename and push. If you'd rather remove the button, delete this line from `index.html`:

```html
<a class="chip" href="resume.pdf" download>Résumé</a>
```

## Using a custom domain

Buy a domain, then in **Settings → Pages → Custom domain** enter it and save. At your registrar add these DNS records:

| Type  | Name | Value |
|-------|------|-------|
| A     | @    | 185.199.108.153 |
| A     | @    | 185.199.109.153 |
| A     | @    | 185.199.110.153 |
| A     | @    | 185.199.111.153 |
| CNAME | www  | farafatima26.github.io |

Then tick **Enforce HTTPS** once the certificate provisions.

## Editing

Everything lives in `index.html`. Content is plain HTML in the `<body>`; colors and type are CSS custom properties at the top of the `<style>` block:

```css
--accent:#1F6F5C;   /* the green used for links and highlights */
--ink:#0D1B2A;      /* the dark navy in the contact panel */
```

Change `--accent` in both the light block (`:root`) and the two dark blocks to reskin the whole site.

## What's interactive

- Animated aurora backdrop and a cursor spotlight that follows the pointer
- Typed rotator under the headline cycling through specialities
- Scroll progress bar, blur-on-scroll nav, and active-section highlighting
- Stat counters that animate up when they scroll into view
- Project cards with 3D tilt and a glow that tracks the cursor
- Experience shown as keyboard-navigable tabs, one employer at a time
- Filterable skill chips by layer (Languages, Frontend, Backend, Data, Cloud, Testing, AI)
- Dark/light toggle, remembered in `localStorage`
- Full-screen mobile menu
- Copy-email button with a toast confirmation

## Notes

- Dark is the default; light mode is one click away and the choice persists.
- Responsive to small phones; keyboard focus is visible throughout; `prefers-reduced-motion` disables every animation.
- The site is static, so there is no contact form. The email and copy buttons cover it without a backend.
