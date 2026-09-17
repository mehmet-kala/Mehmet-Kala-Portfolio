# Portfolio — Mehmet Kala

## Folder structure

```
site/
  index.html                 main page (project flow, about, contact)
  project-holo.html          Hôlo
  project-opus.html          Opus
  project-glucobuddy.html    GlucoBuddy
  project-metu-app.html      METU App
  project-lattice.html       Full Control Lattice Generator
  css/
    style.css                shared by all project pages
    home.css                 main page only
    lattice.css              extra components, lattice page only
  images/                    all images, plain files
```

## Running it locally

1. Open this folder in VS Code (`File → Open Folder`).
2. Install the **Live Server** extension.
3. Right-click `index.html` → *Open with Live Server*.
   The browser refreshes every time you save.

## Adding an image

Every empty slot looks like this in the HTML:

```html
<!-- add your image: replace the div below with an img tag pointing at images/gb_exploded.png -->
<div class="placeholder"><span>EXPLODED VIEW</span></div>
```

Two steps:

1. Put your file in `images/` — **name it exactly as the comment says**
   (e.g. `gb_exploded.png`).
2. Replace the `<div class="placeholder">…</div>` line with:

```html
<img src="images/gb_exploded.png" alt="Exploded view">
```

Keep the `<div class="corner …">` lines underneath — those are the hover brackets.

## Adding a video (lattice page)

```html
<video src="images/lattice_fill_demo.mp4" autoplay muted loop playsinline></video>
```

`muted` and `playsinline` are required or it won't autoplay on phones.

## Image sizes to export

| Slot | Ratio | Export at |
|---|---|---|
| Page hero render | 4:3 | 1600–2000 px wide |
| Main page project shot | 4:3 | 1600 px wide |
| Portrait (main page) | 4:5 | 1200 × 1500 px |
| Slider render | free | 1500–1900 px wide |
| Bento cell | free | 1200–1500 px wide |
| Storyboard frame | 3:2 | 800–1000 px wide |

Export photos as JPG (quality ~85), line art and drawings as PNG.
Keep any single file under ~400 KB.

## Still to fill in

- [ ] Hôlo — Overview text is still generic; your own contribution isn't stated
- [ ] Team projects (Hôlo, GlucoBuddy, METU App) — add which parts were yours
- [ ] GlucoBuddy — all images are placeholders
- [ ] METU App — all images are placeholders
- [ ] Lattice — hero, fig. 01, the four cell shots, and two "Building the Generator" bento
      cells are filled in; the rest are still placeholders. CTA links are `#`
- [ ] Projects 06 and 07 on the main page are still placeholders
- [ ] Contact links in every footer (`youremail@example.com`, LinkedIn, Behance, Instagram)

## Publishing

Drag this whole folder onto <https://app.netlify.com/drop>. It goes live immediately.
Make a free account to keep the URL and attach a domain later.
