rafay.spec — QA Portfolio

Personal portfolio for Rafay (QA engineer, 1.5+ years in QA). Every approved change ends with a working live URL.

Links
Repo: https://github.com/qa-rafay-sdet/rafay-qa-portfolio (branch: main)
Live (production): https://rafay-spec.netlify.app (Netlify project name: rafay-spec)
Always share the production URL, never a per-deploy preview link.
Deployment protection stays OFF so the link opens without a login.
Current status (as of 2026-11-15)

Done: 1/7 (Hero)

Built so far:

Foundation: one self-contained index.html, inline CSS/JS, no build tools.
Sticky test-runner panel (desktop) and bottom progress pill (mobile/tablet).
Reusable test-card component: data-state goes QUEUED → RUNNING → PASS when scrolled into view.
Cursor blob and card tilt, mouse-only, off under prefers-reduced-motion.
Hero section: humanized copy (no generic claims), "1.5+ years in QA", photo as WebP with JPG fallback. Photo sits above the text on mobile and beside the terminal on desktop.
No-JS fallback: all cards render as PASS so content stays visible.

Not done / open issues:

The GitHub repo is EMPTY. Nothing has been pushed yet. First job: put index.html and /assets/ in this folder, commit, push to main.
The Netlify site has a deploy from a manual drag-and-drop. Connect it to the repo (or deploy with the Netlify CLI) so pushes go live.
README.md not written yet.

Remaining sections (assumed order, confirm with me before building): 2. Identity 3. Skills 4. Projects (placeholder cards only) 5. LinkedIn posts (I supply the links) 6. Automation (fails on purpose, retries, passes: "still compiling") 7. Contact + final report

Concept (keep exactly this)

"Live test run": the site runs a test suite on me.

Sticky runner panel on desktop; bottom progress pill on mobile.
Each section is an it('should …') test card: QUEUED → RUNNING → PASS. It starts when scrolled into view.
The automation test fails on purpose, retries, then passes ("still compiling").
Final report: all tests passed, real elapsed time, confetti, re-run suite button.
Style: bold, playful neo-brutalist. Thick ink borders, hard shadows, teal/indigo palette (ink #0f1b2d, paper #f1f5f9, teal #5eead4, periwinkle #a5b4fc, indigo #6366f1, aqua #2dd4bf). Space Grotesk + JetBrains Mono. Animations smooth and fast.
Content rules
Do not name any employer or company. Show total experience only: 1.5+ years in QA.
Core skills: manual and exploratory testing, test cases from PRDs, bug reporting, API (Postman), mobile QA, AI/RAG feature testing, Jira, Git.
Automation (Playwright, API automation, CI) is shown as in progress.
Projects: placeholder cards only until I supply real samples.
One test case features my best LinkedIn posts (links to come).
Copy must sound human: specific facts about my real work, no AI-sounding filler, no hype, no forced jokes.
Real contact links:
GitHub: https://github.com/qa-rafay-sdet
LinkedIn: https://linkedin.com/in/syedmuhammadrafayhassni
Email: rafayarwork01@gmail.com
Every other CTA links to #.
Output format
One self-contained index.html, inline CSS/JS, no build tools, no frameworks.
Placeholder images (https://placehold.co/...) unless I provide images.
Forms are visual only.
Repo structure
/index.html   ← the portfolio
/assets/      ← images (only ones I provide; hero photo as .webp + .jpg)
README.md     ← concept, sections, live link
CLAUDE.md     ← this file
Responsive (mandatory)
Works from 320px to 1920px+, portrait and landscape. No horizontal scroll at any width.
Fluid type with clamp(). Touch targets at least 44px. Grids collapse to one column on small screens.
Runner panel on desktop; pill on mobile and tablet.
Cursor blob and card tilt only on devices with a mouse. Respect prefers-reduced-motion.
Content stays visible if JavaScript fails.
How to verify before marking anything done

Run a Playwright check at 320, 375, 768, 1440, 1920px and 812×375 landscape:

document.documentElement.scrollWidth must not exceed the viewport width.
Test cards reach data-state="pass" after scrolling.
.runner is displayed on desktop only; .pill on mobile/tablet only.
No interactive element is under 44px tall on touch widths.
With JavaScript disabled, all content is visible and cards show PASS.

Known fixes already applied (do not regress):

Use overflow-x: clip on html and body (not hidden; hidden broke the sticky panel and left overflow on narrow widths).
.test-body has overflow-wrap: break-word.
Deployment
Ask me before any push or deploy. Never commit secrets or tokens.
After I approve a change: commit with a clear message (e.g. add: identity section), push to main, deploy to Netlify.
Confirm the live URL shows the change before marking it done.
Keep the README live link current.
I have two GitHub accounts. This repo belongs to qa-rafay-sdet. Check git config user.name and the remote before the first push so it does not go out under the other account.
Working style
One section or change per response unless I ask for more.
For edits, show only the changed part, not the whole file.
Short, direct replies. Answer first, no preamble or recap.
Ask at most one batched question when unclear; otherwise assume sensibly and state the assumption in one line.
End each update with: Done: 2/7 (Hero, Identity) | Live: https://rafay-spec.netlify.app