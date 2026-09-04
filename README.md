# Who's Calling — Teachers' Day invite

An interactive invitation for **Teachers' Day at Atomic Energy Central School, Mysore** — Saturday, 5 September 2026.

A rotary phone rings on the landing screen. Pick up, and the call connects to the invitation and the day's programme.

## What's in it

- **Screen one** — a ringing phone (SVG, drawn in-page), a Web Audio ringtone that switches on at the first tap, and a DECLINE button that refuses to take no for an answer.
- **Screen two** — the invite: ransom-note headline, a torn-paper note, and the programme in three acts, with a live call timer running in the top bar.

No build step, no dependencies. One `index.html`, fonts from Google Fonts.

## Run it locally

Open `index.html` in a browser, or:

```sh
python -m http.server 8000
# then visit http://localhost:8000
```

## Publish on GitHub Pages

1. Push this folder to a GitHub repository.
2. **Settings → Pages → Source: Deploy from a branch**, branch `main`, folder `/ (root)`.
3. The site goes live at `https://<user>.github.io/<repo>/` in a minute or two.

## Editing the programme

Every item lives in one of the three `<article class="card">` blocks in `index.html`. A row is:

```html
<li><span class="d">What happens</span><span class="dots"></span><span class="tm">8:40</span></li>
```

Add `class="mark"` to the `<li>` to highlight a row (bold text, yellow-boxed time).
