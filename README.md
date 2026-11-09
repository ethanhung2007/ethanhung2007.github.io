# ethanhung2007.github.io

Personal ePortfolio, plain HTML + CSS, hosted on GitHub Pages.

## Layout

```
index.html                 Home
about.html                 About
resume.html                Resume (embeds assets/resume.pdf)
goals.html                 Career Goals
projects/index.html        Project grid
projects/*.html            One page per project
assets/style.css           The whole theme (colors, fonts, layout)
assets/resume.pdf          Your resume (add this)
assets/img/                Photos, diagrams, waveforms (add these)
```

## Editing

- **Text:** anything in `[brackets]` with `class="todo"` is a placeholder. Write your text and delete `todo` from the class.
- **Images:** each `<div class="slot ...">Label</div>` is an image spot. Replace the label with
  `<img src="assets/img/name.jpg" alt="What the photo shows">` (use `../assets/...` inside `projects/`).
- **Colors / fonts:** change the variables at the top of `assets/style.css`.
- **New project:** copy `projects/simt-gpu-core.html`, rename it, edit it, and add a card to `projects/index.html`.
- **Nav link:** the header is copied into every page, so update all of them.

## Preview locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Publish

Push to `main`. In the repo: Settings → Pages → Deploy from a branch → `main` / root.
