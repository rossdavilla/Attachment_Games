# Attachment Apps (`Attachment_Games`)

Three classroom activities on adult attachment styles, for **PSY157 (Personal Relationships)**.
Live at <https://rossdavilla.github.io/Attachment_Games/>.

## Layout

Every page is one self-contained `.html` file — HTML, CSS and JS inline, no build step, no
dependencies, nothing stored or sent anywhere. The only outside request is Google Fonts.

| File | What it is |
|---|---|
| `index.html` | Landing page ("Attachment Styles Lab") linking the three activities |
| `quiz.html` | **What's Your Attachment Style?** — 12 items placing the student on the anxiety–avoidance map |
| `textsim.html` | **Read the Texts** — text back and forth with three people, each hiding a style, and work out which is which |
| `compatibility.html` | **Style Matcher** — pick two styles to see satisfaction potential, tension points and conflict behaviour |

## The `*StandAlone*.html` copies

Two different things share that prefix — check which one you are editing:

| File | What it is |
|---|---|
| `QuizStandAlone.html`, `MatcherStandAlone.html`, `TextSimStandAlone.html` | **Standalone copies** — the activity on its own, without the Attachment Styles Lab chrome. Not sized to any frame. |
| `TextSimStandAlone-embed.html` | **Top Hat embed** — laid out to fit a fixed **720 × 450** iframe with no scrolling |
| `TextSimStandAlone-embed-1/-2/-3.html` | the same embed cut to one, two and three rounds, for when there is less class time |

- These are separate files, not generated from the main pages. **A change to an activity has to be
  made in its main page *and* in each copy of it**, or they drift apart. Say so when you only
  change one.
- Only the `-embed` files need to hold 720 × 450 without scrolling.
- In the site directory they are `links` on the main app's card, not cards of their own.

## Conventions

- Keep each page a single file with no runtime dependency beyond Google Fonts.
- Nothing is collected: no localStorage, no analytics, no backend. Keep it that way — these run in
  front of a class.
- Embeds must fit 720 × 450 exactly and must not scroll at that size.

## Publishing

GitHub Pages serves `main` from the repository root, so a push to `main` is the deploy.

`index.html` is deliberately kept out of the directory (it is in this repo's `ignore` list in
`data/sites.json`) — the three activities get their own cards instead.

After adding a new page here, add it to `data/sites.json` in the
[`rossdavilla.github.io`](https://github.com/rossdavilla/rossdavilla.github.io) repo (tag
`PSY157`) — a new activity gets its own `apps` entry; a Top Hat or standalone copy of an existing
activity goes in that app's `links`.
