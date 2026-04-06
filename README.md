# Bryant Nankee — Portfolio Site

Live at **portfolio.bryantnankee.com** | Resume at **resume.bryantnankee.com**

Hosted on Cloudflare Pages. GitHub repo: `teslaterdude/portfolio-site`. Pushes to `main` auto-deploy.

## Files

- `index.html` — main portfolio (hero, results, work samples, AI & systems, about, contact)
- `resume.html` — web resume (print-ready, linked from nav)
- `_redirects` — redirects resume.bryantnankee.com → portfolio.bryantnankee.com/resume
- `vercel.json` — kept for reference, not used by Cloudflare

## Adding images and video

Drop files into this folder, then replace placeholder blocks in `index.html`.

**For images** — find the `<div class="work-img-placeholder">` in each work card and replace with:
```html
<img src="your-file.jpg" alt="Description" style="width:100%; height:100%; object-fit:cover;" />
```

**For the Remotion video** (work card 6) — replace placeholder with:
```html
<video autoplay muted loop playsinline style="width:100%; height:100%; object-fit:cover;">
  <source src="your-video.mp4" type="video/mp4" />
</video>
```

**For the headshot** (about section) — replace the entire `<div class="about-photo">` with:
```html
<img src="headshot.jpg" alt="Bryant Nankee" style="aspect-ratio:4/5; max-width:360px; width:100%; border-radius:20px; object-fit:cover;" />
```

### Placeholder checklist

- [ ] 1. HubSpot attribution/reporting dashboard (screenshot)
- [ ] 2. Ad creative — Meta or Google collage (screenshot)
- [ ] 3. HubSpot lead routing workflow (screenshot)
- [ ] 4. UTM attribution system — diagram, Notion doc, or HubSpot view (screenshot)
- [ ] 5. AI agent system — Claude Code terminal or GitHub repo structure (screenshot)
- [ ] 6. Remotion video (mp4)
- [ ] 7. ecp123.com website rebuild — before/after or WIP (screenshot)
- [ ] 8. Headshot (jpg/png)

## Deploying changes

```bash
git add .
git commit -m "your message"
git push
```

Cloudflare picks it up automatically. No build step needed.

## Resume (.docx)

The updated Word resume lives at:
`/Users/bryantnankee/Downloads/Claude Workspace/Professional/Projects/8_Bryant Resume/Bryant Nankee - Resume - 2026.docx`

The source markdown is in the same folder as `Bryant Nankee - Resume - 2025.docx.md`.
