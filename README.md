# Loopstack

A dark, single-screen landing page for a closed beta. Words of the headline rise out of a mask, the logo letters slide in one by one, a glass pill follows your cursor, and a looping video plays behind everything.

Built by AI from a prompt found online. Copy it, open it, or paste it into your own AI and make it yours, with no need to build it from scratch.

## Features

- Word-by-word headline reveal with a blur-in effect
- Giant "Loopstack" wordmark that slides in letter by letter
- Glass cursor card ("Say Hello!") and ring that follow the mouse with smooth easing, and hide over the button
- Pulsing green dot on the "Book a demo" button
- Looping, muted background video with a black gradient overlay
- Footer with social icons, links and a "Think. Build. Repeat." tagline

## Tech

Plain HTML, CSS and JavaScript. No build step and no dependencies to install.

## Setup

**Option 1: just open it.** Double-click `index.html`. You need an internet connection.

**Option 2: run a local server** (needs [Node.js](https://nodejs.org)):

```bash
npm start
```

Then open the address it prints, usually http://localhost:3000.

**Put it online for free:** push this folder to GitHub, then go to Settings → Pages and deploy from the `main` branch.

## Make it yours

Open `index.html` and change:

| What | Where |
|---|---|
| Headline | the `<h1 class="hero-title">` line |
| Brand name | the `<h2 class="footer-logo-text">` line and the `<title>` |
| Button text | `<span class="btn-text">` |
| Cursor card text | `<span class="cursor-card-text">` |
| Tagline, links, copyright | the `<footer class="footer-container">` block |
| Background video | the `src` on the `<source>` inside `<video id="bg-video">` |
| Fonts | the `@import` lines at the top of the `<style>` block |

Quick way: paste `index.html` into your AI and say what you want, for example *"Rebrand this as a fitness app called PulseFit, with orange accents and new copy."*

## Good to know

- **Hosted files.** The background video and gradient load from `api.getlayers.ai`:
  - `black_gradient.svg`
  - `flower.mp4`

  If that host removes them, the page loses its background. To make it fully offline, download both files into an `assets/` folder and update the two URLs in `index.html`, if the license allows.
- **Fonts** (Outfit, Playfair Display, General Sans) load from Google Fonts and Fontshare.
- **One screen only.** The page doesn't scroll. Everything is fixed to the viewport.
- **Demo content.** The brand, links and copy are placeholders. The social links and footer links point to `#`.
- **Language.** The page is marked `lang="ru"`, the code comments are in Russian, and the video fallback text is in Russian. Change `lang` to `en` and translate the fallback if you want.

## Credits

Original prompt: _add the source link here_
