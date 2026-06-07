# Development Journal — School Automation MVP (Concept Mockup)
A chronological log of key developments, decisions and learnings throughout this project.

---

## 2026-06-07 — Built a spec homepage mockup to win a PeoplePerHour proposal

**Type:** Milestone

**What I built or did**
I created a clean, mobile-first concept homepage for a prospective client (Sello M) who posted a £74 job on PeoplePerHour for a school-automation website. Rather than send a generic written pitch like everyone else, I built a single-file HTML mockup of *his* homepage — hero, features, ZAR pricing tiers, lead form, WhatsApp button — and published it live on GitHub Pages so he could tap it on his phone. I then attached two real feature demo clips (AI chatbot + Stripe billing) from my ThaiBridge AI prototype, and submitted the full proposal.

**Why I did it this way**
The advice I was following was "show, don't tell" — a quick spec mockup signals you've already thought about the client's problem, which beats a blurb. I kept it deliberately light (one HTML file, ~20 mins) so I wasn't sinking a weekend of free work into a small job I might not win.

**How it works**
It's a self-contained `index.html` with inline CSS — mobile-first, single-column on phones, expanding to a 3-column desktop layout via one media query. Hosted free on GitHub Pages at the repo's `/` root on `main`.

**What this means for the app**
It's both a live proposal asset *and* a reusable portfolio piece showing I can lay out a clean, responsive site fast.

**What I learned**
- Publishing a static site to GitHub Pages via the CLI (`gh repo create --push` + enabling Pages through the API).
- PeoplePerHour's attachment box stalls on video uploads — solved by compressing the clips with ffmpeg (two-pass, kept 1080p, both under the 20 MB limit).
- The effective `gh` identity is what `gh api user` returns, not always what `gh auth status` shows first.

**References / Conversations**
- Live mockup: https://joshuablakemorekay.github.io/school-automation-mvp/
- Built in a Claude Code session, 2026-06-07.

---
