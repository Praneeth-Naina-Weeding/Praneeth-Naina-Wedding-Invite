# Praneeth & Naina — Wedding Invitation Website

A single-page, bilingual (Telugu / English) wedding invitation site with an Indian temple-inspired aesthetic — kalash, diyas, toran garland, mandala backdrop, floating petals, and a scroll-animated event timeline. Background music ("Kalyanam Vybhogam") starts automatically when the page loads.

## Files

```
index.html          ← the entire site (HTML + CSS + JS in one file)
assets/
  kalyanam-vybhogam.mp3   ← background music
```

## How to publish on GitHub Pages

1. Create a new GitHub repository (e.g. `praneeth-naina-wedding`).
2. Upload `index.html` and the `assets/` folder (with the mp3 inside it) to the repo, keeping the same folder structure.
3. In the repo, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. Save.
5. Wait a minute, then your site will be live at:
   `https://<your-github-username>.github.io/<repo-name>/`

That's it — no build step needed, it's plain HTML/CSS/JS.

## Notes

- **Opening screen**: the site opens on a maroon-and-gold "Open Invitation" cover. Tapping it reveals the invitation *and* starts the music at the same moment. This is intentional — every modern browser (Chrome, Safari, Edge) now blocks a page from playing sound before the visitor interacts with it, no matter how the code is written, so a tap-to-open cover is the standard, reliable way real wedding-invite sites handle this.
- **Language toggle**: the button in the top-right (🪔) switches all text between Telugu (default) and English. The choice is remembered on the visitor's device.
- **Music controls**: the 🎵 button lets anyone pause/resume any time after opening.
- **Editing text**: open `index.html` in any text editor and search for the event/name you want to change — each piece of text has a Telugu (`<span class="te">`) and English (`<span class="en">`) version sitting next to each other.
- **Editing colours**: all colours are defined once at the top of the `<style>` block under `:root { ... }` (e.g. `--maroon`, `--gold`, `--green`).
- **On the artwork**: the decorative elements (banana leaves, hanging diya, floral pots, kalash, peacock, mandala, Ganesha, the garland-exchange scene, diamond borders) are original SVG line-art, drawn to closely echo the composition and palette of your printed invitation. The exact clipart images inside the PDF are licensed template stock art (from the invitation-design service that made it), which is normally licensed only for that specific printed/PDF invite — not for re-hosting on a separate public website/repo — so those exact files aren't reused here.
