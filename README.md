# Homework 1: AI-Generated Portfolio Site

**CSC 436 — Web Applications | DePaul University**
**Points:** 100

---

## Overview

In this assignment, you will use AI tools (GitHub Copilot, ChatGPT, Claude, or similar) to generate a **responsive personal portfolio website**. The goal is not just to produce a working site — it's to develop a critical eye for AI-generated code. You will document every prompt you use, identify and fix issues in the output, and reflect on the experience.

**You are required to use AI for this assignment.** However, you must understand every line of code you submit and be prepared to explain it.

---

## Requirements

### Portfolio Website

Starting from the provided `starter-template.html`, use AI to build a portfolio site that includes:

1. **Hero Section** — A visually engaging introduction with your name (or a fictitious name) and a tagline
2. **About Section** — A short bio paragraph with a professional tone
3. **Projects Grid** — At least **4 project cards** displayed in a responsive grid layout. Each card should have:
   - Project title
   - Brief description
   - A placeholder image or icon
   - A link (can be `#`)
4. **Contact Form** — A form with the following fields and validation:
   - Name (required)
   - Email (required, must be valid format)
   - Message (required, minimum 10 characters)
   - Submit button
   - Client-side validation with user-friendly error messages

### Responsiveness

- The site **must work on both mobile and desktop** screen sizes
- Use a mobile-first or responsive approach (media queries, flexbox, grid, etc.)
- Test at common breakpoints: 375px (mobile), 768px (tablet), 1024px+ (desktop)

### Accessibility

Your site must pass basic accessibility checks:

- All images have meaningful `alt` text
- Form inputs have associated `<label>` elements
- Color contrast is sufficient for readability
- Heading hierarchy is logical (h1 → h2 → h3, no skipped levels)
- The page is navigable via keyboard (tab through interactive elements)

### Prompt Log

Document **every prompt** you use in the provided template below. This is a critical part of the assignment — we want to see your process, not just the result.

### Issue Identification & Fixes

Identify and fix **at least 3 issues** in the AI-generated code. These could be:

- Accessibility problems (missing alt text, no labels, poor contrast)
- Responsiveness bugs (layout breaks at certain widths)
- Semantic HTML issues (using `<div>` where `<section>` or `<nav>` is appropriate)
- Validation errors (form submits without proper checks)
- Code quality issues (inline styles that should be classes, repeated code)
- Browser compatibility issues

Document each issue: what was wrong, why it matters, and how you fixed it.

### Reflection

Write a **reflection** covering:

- What did AI get right on the first try?
- What did it get wrong or miss?
- What surprised you about working with AI?
- What did you learn about web development from this process?
- How did you decide which prompts to use, and how did you refine them?

---

## Grading Rubric

| Category | Points | Criteria |
|---|---|---|
| **Portfolio Content & Functionality** | 25 | All 4 sections present and functional. Projects grid has 4+ cards. Contact form validates correctly. |
| **Responsiveness** | 15 | Site works well at mobile, tablet, and desktop sizes. No horizontal scroll, no overlapping elements. |
| **Accessibility** | 10 | Passes basic checks: alt text, labels, contrast, heading hierarchy, keyboard navigation. |
| **Prompt Log** | 20 | All prompts documented with context and outcomes. Shows iterative refinement. Thorough and honest. |
| **Issue Identification & Fixes** | 20 | At least 3 genuine issues identified. Clear explanation of what was wrong and how it was fixed. |
| **Reflection** | 10 | Thoughtful. Addresses all reflection prompts. Shows genuine learning. |
| **Total** | **100** | |

---

## Submission Instructions

Submit the following files to the course D2L dropbox:

1. **`portfolio.html`** — Your final portfolio site (single HTML file with embedded CSS/JS, or separate files)
2. **`prompt-log.md`** — Your completed prompt log (use the template below)
3. **`issues.md`** — Your documented issues and fixes
4. **`reflection.md`** — Your written reflection

If you use separate CSS/JS files, include those as well. Zip all files together if submitting multiple files.

---

## How To Run The Portfolio Locally

From the project folder, start a simple local server:

```bash
python3 -m http.server 8000
```

Then open this URL in your browser:

```text
http://localhost:8000/portfolio.html
```

---

## Prompt Log Template

Create a file called `prompt-log.md` and use this format:

```markdown
# Prompt Log — Homework 1

## Prompt 1
- **Tool Used:** (e.g., ChatGPT, GitHub Copilot, Claude)
- **Prompt:** (Paste your exact prompt here)
- **Goal:** (What were you trying to accomplish?)
- **Result:** (Brief summary — did it work? What did the AI produce?)
- **Changes Made:** (Did you modify the output? How?)

## Prompt 2
- **Tool Used:**
- **Prompt:**
- **Goal:**
- **Result:**
- **Changes Made:**

<!-- Add as many prompts as needed. Most students use 5–15 prompts. -->
```

---

## Issues & Fixes Template

Create a file called `issues.md` and use this format:

```markdown
# Issues Found & Fixed — Homework 1

## Issue 1
- **What I Found:** (Describe the problem)
- **Why It Matters:** (Why is this a problem? Accessibility? UX? Code quality?)
- **How I Fixed It:** (What did you change?)
- **Before:** (Paste the problematic code snippet)
- **After:** (Paste the corrected code snippet)

## Issue 2
...

## Issue 3
...
```

---

## Reflection Guide

Create a file called `reflection.md`. Address the following questions:

1. **What worked well?** — Which parts of the portfolio did AI generate effectively on the first try?
2. **What didn't work?** — Where did the AI fall short? What required manual intervention?
3. **Surprises** — What surprised you about the AI's output (good or bad)?
4. **Learning** — What did you learn about HTML, CSS, JavaScript, or web development in general?
5. **Process** — How did your prompting strategy evolve? Did you get better at prompting as you went?

---

## Tips for Success

- **Start early.** You'll need time to experiment with prompts and iterate.
- **Be specific in your prompts.** "Make a website" produces worse results than "Create a responsive hero section with a dark background, white text, my name in an h1, and a subtitle paragraph."
- **Don't accept the first output.** Refine your prompts. Ask follow-up questions. Iterate.
- **Test on different screen sizes.** Use your browser's developer tools (F12 → toggle device toolbar) to test responsiveness.
- **Read the code.** Don't just paste and pray. Understand what each section does. You may be asked to explain your code.
- **Use the starter template.** It gives you a clean structure to build from.
- **Check accessibility.** Try tabbing through your page. Use a contrast checker. Run a quick audit in Chrome DevTools (Lighthouse).

---

## Academic Integrity Policy for AI-Assisted Work

This course **requires** the use of AI tools — that is the whole point. However:

1. **You must document all AI usage.** Every prompt, every tool, every interaction goes in your prompt log. Undocumented AI usage is a violation.
2. **You must understand your code.** If you cannot explain what a piece of code does and why, you will not receive credit for it. Be prepared for in-class code reviews.
3. **You must fix and improve AI output.** Submitting raw, unreviewed AI output is not acceptable. The issue identification requirement exists for this reason.
4. **Do not copy from classmates.** Your prompts, fixes, and reflections must be your own. AI-generated code will naturally vary between students, but prompt logs and reflections should be unique.
5. **Be honest.** If a prompt didn't work, document that. If you wrote code manually, note that too. We value your learning process over a polished result.

**In short: Use AI, document everything, understand everything, improve everything.**

---

*Questions? Post in the course discussion board or visit office hours.*
