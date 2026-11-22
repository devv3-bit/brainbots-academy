# AGENTS.md: BrainBots Academy site

One-page site for BrainBots Academy (student-led non-profit, Indore) built on the Kinfold template by 8B. One file, `index.html`, inline CSS and scripts, no libraries, no build step. Blue theme: the eight paper and ink tokens in `:root` (`data-8b-part="tokens"`) plus `--color-9`, a bright accent used only for the bar under the Impact titles.

## Keep
- Every `id`, `data-8b-section`, `data-8b-motion`, `data-8b-part`, `data-8b-items`, `data-8b-fixed` and `data-8b-enter` attribute: the CSS scroll scenes and the inline motion kit read them.
- Fixed counts: fifteen entries in the learning tree (`#case`, client first then two children per entry), four steps in `#method`, two cards in `#people` (their start offsets are inline variables that make the two stamps begin as one joined block).
- Selectors the scripts use: `.tabs__tab`, `.case__chart`, `.case__person`, `.case__dot`, `.letters__track`, `.contact__form`, `.contact__status`, `.contact__copy`, `.archives__frame`, `.archives__ledger`, `.archives__name`, `.method__slips`, `.fees__body`, `.fees__item`, `.fees__name`, `.fees__amount`.
- The header comment, `<meta name="generator">` and the LICENSE file: that is what the template's MIT licence asks for. The visible "Design: 8B" footer link was removed at the owner's request.

## Facts on the page (from BrainBots' own documents, not invented)
- Student-led non-profit, Indore, Madhya Pradesh; co-founded by Dev Hemnani and Arham Sethi (the whole team: two people); teaches students aged 12 to 19; free of charge.
- 50+ sessions, 550+ students, 3+ NGO partners (founders, November 2026). Named partners: AAS Foundation and FTS Yuva (confirmed by the founders).
- Program 1, spring 2025, about 30 students: Cybersecurity 4/10 to 8/10, Introduction to AI 1/10 to 9/10, Prompt engineering 4/10 to 8/10, AI tools for daily life 2/10 to 10/10, Introduction to programming 1/10 to 9/10 (knowledge level before and after). Test papers are set in Hindi and English.
- Learning curve: skill proficiency index 35, 42, 50, 58, 67, 84 over weeks 1 to 6.
- Instagram @brainbotsacademyy, LinkedIn /company/brainbots-academy, sign-up Google Form (see the Join button).

## Still placeholder
- `data-8b-placeholder="email"` in `#contact`; the form sends nothing. All photo slots now hold real photos (originals in ../photos).
