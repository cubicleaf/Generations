# Generations — STATUS

**What this file is.** A running record of where this project stands — interviews completed, decisions made, what's in the pipeline. Reference [INTENT.md](INTENT.md) for what this project is trying to be.

Last updated: 2026-07-31

---

## Interview log

| # | Subject | Relationship | Date | Status |
|---|---------|-------------|------|--------|
| 1 | First uncle | Tim's uncle | Earlier | **At risk** — audio didn't record properly; must review video quality before deciding to reshoot |
| 2 | Uncle Craig (± his wife) | Dad's older brother | 2026-05-16 | Recorded — question set: `_docs/interviews/craig-interview-2026-05-16.md` |
| 3 | Dad | Father | TBD | Planned (3 videos potentially in pipeline — on hold, artistic decisions) |
| 4 | Mom | Mother | TBD | Planned |
| 5 | Sister | Sibling | TBD | Possible |

---

## Decisions

### 2026-07-31 (v2) — Favicon redesigned: video-library card stack, light/rice-paper shell
**What:** Replaced the single dark-shell play-triangle design with a three-card "video library" composition (from an uploaded reference SVG: a stack of three rounded-rect cards, decreasing depth, front card containing the play triangle cutout). Shell flipped from dark (`#1a1610`) to rice paper (`#f5f0e8`, matching the tone used across the rest of the portfolio). Front card is a warm coffee brown `#4a3527`; the two cards behind step up in lightness by a fixed geometric ratio (×1.42 per layer, in HSL space, hue/saturation held constant) — `#694b37`, then `#956b4f` — rather than eyeballed shades. Icon sized to 64% of canvas, verified by pixel measurement to sit fully inside the shell's 95%-fill bounds (the same margin ratio that worked well on Zifang's final approved size).
**Why:** Direct request to keep Generations' original earthy color family but move to a richer, more literal "library of recordings" icon instead of an abstract play-triangle, and to lighten the background.
**How to apply:** Files live in project root, relative `href`s (Netlify serves root directly, no rewrite rule). `index.html`'s `<link>` tags are unchanged — same filenames, only pixel content replaced.

### 2026-07-31 — Favicon set built and wired
**What:** Full favicon set (`favicon.ico`, 16/32/180/192/512 PNGs, `site.webmanifest`) generated and added to project root; `<link>` tags wired into `index.html`, replacing the old single `apple-touch-icon` pointed at `og-image.png`. Design: dark shell (`#1a1610`, the site's own `--bg` token) with a gold play-triangle (`#c9a87c`, `--accent`) — nested inside the same rounded-square outer shell used for Master Reader/Charles Hub. Sized at 95% canvas fill.
**Why:** Part of the portfolio-wide favicon rollout; grounded in Generations' real CSS tokens.
**How to apply:** Files live in project root, relative `href`s (Netlify serves root directly, no rewrite rule). Not pushed yet — command handed to Tim directly.

### 2026-07-17 — Completed interview question set archived under `_docs/`
**What:** Moved Craig's completed 2026-05-16 interview question set to `_docs/interviews/`.
**Why:** It is valuable as interview evidence and a future recon reference, but it is a completed dated capture rather than the project's current operating surface.
**How to apply:** Use the Question library and current interview log to plan future sessions; consult the archived set when building on Craig's testimony.

### 2026-06-24 — Stage corrected: active, not archived
Generations is a live ongoing content project — videos get added as they're recorded. "Done, don't touch" is retired. The site is the presentation layer; the interviews are the project.

### 2026-05-16 — Recording redundancy required going forward
First uncle's audio failed. Every interview from here on: backup phone-mic per person + playback check before rolling.

### 2026-05-16 — Interviewee-specific question design
Each interview has phases that only work for that person. The generic 25-question base set (TEMP questions.txt, iteration 3) is now a base layer, not the whole interview. Craig's set added 4 new phases: older-brother, outside-in (in-law POV), memory-joggers for Dad, and triangulation.

### 2026-05-16 — Triangulation is a structural feature
Some questions are asked to multiple interviewees deliberately. The contradictions and differences between versions are the story — potentially its own episode format in editing.

### 2026-05-16 — Older-brother angle is the wedge
Craig saw the grandparents before Tim's dad was old enough to notice anything. Highest-leverage use of Craig's slot.

### 2026-05-16 — Recon mode built in
Some interviews are also intelligence-gathering for later ones. Craig's session was partly about unlocking material for Dad's eventual interview.

---

## Open items

- Review first uncle's video: salvage or reshoot?
- 3 videos potentially ready to record — being held for artistic decisions
- No Dad interview template yet — draft after reviewing what Craig surfaced
- No sister interview template
- Episode release format / cadence: undecided

---

## Question library

- `_docs/interviews/craig-interview-2026-05-16.md` — Craig's question set, 43 questions across 8 phases
- `TEMP questions.txt` — prior 3-iteration question library; iteration 3 is the canonical 25-question, 6-phase base set
