# BrainBots Academy website

One-page site for BrainBots Academy, the student-led non-profit in Indore that teaches coding, AI, cybersecurity and digital design to underprivileged students aged 12 to 19.

**Live:** https://devv3-bit.github.io/brainbots-academy/

## How it is built

- One file, `index.html`, with the CSS and scripts inline. No build step, no JavaScript libraries.
- Built on the free Kinfold template by 8B (MIT), restyled in blue for BrainBots. See `CREDITS.md`.
- Hosted on GitHub Pages from the `main` branch. Every push to `main` redeploys the site within a minute or two.

## Editing

Open `index.html` and change the text in place. Each section is marked with a comment and a `data-8b-section` name:

| Section | id | What it holds |
|---|---|---|
| Home | `opening` | Headline, intro, four numbers, logo and a photo |
| Impact | `archives` | Learning-curve chart and five modules with before/after knowledge levels |
| How a program runs | `method` | Four steps |
| What we teach | `folder` | Four tabs: Coding, AI, Safety, Design |
| How a student grows | `case` | The learning tree (keep fifteen entries, in order) |
| Team | `people` | Four portrait cards (keep four) |
| Before and after | `letters` | Five score slips |
| Where we teach | `room` | Visit card and a wide photo |
| Questions | `questions` | Six questions and answers |
| Programs | `fees` | Three programs |
| Write to us | `contact` | Email, Instagram, LinkedIn, sign-up form |

### Adding photos

1. Put the image in `assets/` (JPG or PNG, about 1600px on the long side is plenty).
2. Find the `<img src="assets/placeholder.svg" ...>` you want to replace and point `src` at your file. Update `alt` and the `width`/`height` attributes to the image's ratio.

Photo slots, in page order: one classroom photo on the Home sheet, one per tab in What we teach (four), four portraits in Team, one wide room photo in Where we teach.

### Things still to fill in

- The email address in Write to us (`hello@brainbotsacademy.example`), marked `data-8b-placeholder="email"`.
- Three team cards still say "Name to add".
- The form shows a thank-you line but sends nothing. To receive messages, connect Formspree (set the form's `action` to your Formspree URL) or link the Join button to the existing Google Form.
- The numbers on the Home sheet (sessions, students, partners) are from December 2025; bump them as the work grows.

## Running locally

Any static server works:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000/.
