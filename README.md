# Attachment Styles Lab

Three classroom activities on adult attachment styles, built for PSY157 (Personal Relationships).
Each one is a single self-contained HTML file — no build step, no dependencies, nothing stored and
nothing sent anywhere.

**Live site:** https://rossdavilla.github.io/Attachment_Games/

## The activities

| Page | What it does |
| --- | --- |
| [`quiz.html`](quiz.html) | **What's Your Attachment Style?** — a 12-item questionnaire that places you on the anxiety–avoidance map and explains the quadrant you land in. |
| [`textsim.html`](textsim.html) | **Read the Texts** — text back and forth with three people, each hiding an attachment style, and work out which one from how they reply. |
| [`compatibility.html`](compatibility.html) | **Style Matcher** — pick two attachment styles to see their satisfaction potential, their tension points, and how they handle conflict. |
| [`index.html`](index.html) | The landing page linking all three. |

## The other copies

Each activity also exists in versions for other settings. They are separate files, so an edit to
an activity needs to be made in its copies too.

| Page | What it is |
| --- | --- |
| `QuizStandAlone.html`, `MatcherStandAlone.html`, `TextSimStandAlone.html` | The activity on its own, without the Attachment Styles Lab navigation — for linking directly or dropping into another site. |
| `TextSimStandAlone-embed.html` | The text sim laid out for a fixed **720 × 450** Top Hat iframe, no scrolling. |
| `TextSimStandAlone-embed-1.html`, `-embed-2.html`, `-embed-3.html` | The same embed cut to one, two and three rounds, for when there is less class time. |

```html
<iframe src="https://rossdavilla.github.io/Attachment_Games/TextSimStandAlone-embed.html"
        width="720" height="450" style="border:0;max-width:100%"
        title="Read the Texts"></iframe>
```

## Running it

Open any of the files in a browser — that is all. To serve the folder instead:

```bash
python3 -m http.server 8000
```

Nothing is collected: no accounts, no backend, no analytics, no stored answers. The only outside
request is Google Fonts.
