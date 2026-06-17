# CLAUDE.md — statistical-design (public Quarto site)

_Notes for Claude Code or any AI assistant working in this repo._

## What this repo is

The **public-facing Quarto course-materials site** for **Design,
Experiments & Causal Evidence** (an undergraduate study-design and
causal-reasoning course) assembled by Matt Hester. It is a sibling of the
main site [matthewhester.com](https://matthewhester.com) and is intended
to live at `/statistical-design/` under that domain, alongside the other
course sites. (Repo/deploy slug is `statistical-design`; the public
display title is "Design, Experiments & Causal Evidence".)

It holds **assembled undergraduate course material** — the course's own
synthesized notes, hands-on labs, and curated resources.

## What this repo is not

- It is **not** the private course build. That lives in a separate,
  Drive-synced teaching workspace and is not part of this repository.
- It is **not** a claim that the course is currently being taught. This
  is durable, public course material; honest wording is "assembled
  undergraduate course materials," not "a course I am teaching now."
- It is **not** the LMS. **Blackboard remains authoritative** for grades,
  due dates, submissions, rosters, and anything operational whenever the
  course runs.
- It is **not** a raw archive. Lesson pages are the course's own
  synthesized prose; the site does not host bulk-copied textbook
  material, private assessments, or instructor-only build artifacts.

## Do not add to this repo

- Answer keys or solutions (any form: PDF, TeX, Markdown, `_key.*`).
- Assessment items, specs, manifests, scenarios, rubrics, point values.
- Anything from the private course build:
  `_state/`, `assessment_shadow/`, `source_text/`, `run_reports/`,
  `accessibility/`, `export/`.
- Source mirrors of Introduction to Modern Statistics, ModernDive, or
  Causal Inference: What If, or per-chapter extracts/indexes. Cite at the
  section level; do not reproduce source text wholesale.
- Student data, FERPA-adjacent material, gradebook exports, rosters.

When unsure, default to **don't publish** and ask.

## Provenance

Assembled (2026-06) from a course-material build. Only the public surface
was promoted: `index.qmd`, `syllabus.qmd`, `schedule.qmd`, `notes/`,
`labs/`, `resources/`, `styles.css`, and `_quarto.yml`. Every private
directory listed above was deliberately left behind.

## Rendering

- R chunks are written as **static, non-executed** ` ```r ` fences, so
  `quarto render` builds the whole site **without R** (deterministic).
  Output goes to `_site/` (gitignored).
- The combined public site is assembled and deployed by the hub repo
  (`matthewhester-site`); this repo has no CI of its own.

## Images

- `assets/hero.png` — full course-identity banner (carries the title);
  referenced on `index.qmd` with `.course-hero-img` and alt text.
- `assets/icon.png` — square crystal mark with transparent background;
  wired as the navbar `logo`.
- Every committed image needs alt text.

## Hard rules for Claude in this repo

- **Commit only when explicitly instructed.** Never push without explicit
  instruction.
- **Do not reach back into the private course build** unless explicitly
  instructed.
- **Do not wire up deployment** (CI, remotes, hub workflow edits) without
  an explicit decision.
