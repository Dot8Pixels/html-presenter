# html_presenter — Frontend Slides Skill

This workspace is a local installation of **[frontend-slides](https://github.com/zarazhangrui/frontend-slides)** v2.1.0 by @zarazhangrui — a coding-agent skill for creating stunning, zero-dependency HTML presentations.

## What's Here

| File | Purpose |
|---|---|
| [`SKILL.md`](SKILL.md) | **Core workflow** — the entry point for any AI agent. Read this first. |
| [`STYLE_PRESETS.md`](STYLE_PRESETS.md) | 12 curated visual presets (dark, light, specialty themes) |
| [`viewport-base.css`](viewport-base.css) | Mandatory fixed 16:9 stage CSS — include in every presentation |
| [`html-template.md`](html-template.md) | HTML architecture, JS features, inline editing implementation |
| [`animation-patterns.md`](animation-patterns.md) | CSS/JS animation reference by feeling |
| [`bold-template-pack/`](bold-template-pack/) | 34 bold design systems (Vellum, Studio, Signal, etc.) |
| [`scripts/`](scripts/) | PPT extraction, Vercel deploy, PDF export utilities |

## How to Use (for AI Agents)

1. **Read [`SKILL.md`](SKILL.md)** — it's the full workflow map
2. Follow the phases:
   - **Phase 0** — Detect mode: new presentation, PPT conversion, or enhancement
   - **Phase 1** — Content discovery (ask user about purpose, length, content, density)
   - **Phase 2** — Style discovery (generate 3 visual previews, let user pick)
   - **Phase 3** — Generate full HTML presentation
   - **Phase 4-6** — PPT conversion, delivery, share/export
3. **Key rules:**
   - Every deck uses a fixed 1920×1080 stage scaled uniformly — never reflow content
   - Include the **full** `viewport-base.css` in every presentation
   - Use distinctive fonts (Fontshare / Google Fonts) — never system fonts
   - No generic "AI slop" aesthetics (no Inter/Roboto, no purple gradients on white)

## Scripts

```bash
# Extract content from a PowerPoint file
pip install python-pptx
python scripts/extract-pptx.py input.pptx output_dir/

# Deploy to a live URL (Vercel)
bash scripts/deploy.sh ./my-deck/

# Export to PDF
bash scripts/export-pdf.sh ./presentation.html
```

## Philosophy

- **Zero dependencies** — Single HTML files with inline CSS/JS, no build tools
- **Show, don't tell** — Visual previews instead of abstract design choices
- **Distinctive design** — Every presentation should feel custom-crafted
- **Progressive disclosure** — Read lightweight indexes first, full details only when needed

---

*Installed from [zarazhangrui/frontend-slides](https://github.com/zarazhangrui/frontend-slides) — MIT License*
