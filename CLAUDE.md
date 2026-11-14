rafay.spec — QA Portfolio

Personal portfolio for Rafay (QA engineer, 1.5+ years in QA). Every approved change ends with a working live URL.

Links
Repo: https://github.com/qa-rafay-sdet/rafay-qa-portfolio (branch: main)
Live (production): https://rafay-spec.netlify.app (Netlify project name: rafay-spec)
Always share the production URL, never a per-deploy preview link.
Deployment protection stays OFF so the link opens without a login.
Current status (as of 2026-11-15)

Done: 7/7 (Hero, Identity, Skills, Projects, Posts, Automation, Contact + final report)

Built so far:

Foundation: one self-contained index.html, inline CSS/JS, no build tools.
Sticky test-runner panel (desktop) and bottom progress pill (mobile/tablet).
Reusable test-card component: data-state goes QUEUED → RUNNING → PASS when scrolled into view.
Cursor blob and card tilt, mouse-only, off under prefers-reduced-motion.
Hero section: humanized copy (no generic claims), "1.5+ years in QA", photo as WebP with JPG fallback. Photo sits above the text on mobile and beside the terminal on desktop.
No-JS fallback: all cards render as PASS so content stays visible.

Not done / open issues:

Projects: three placeholder cards. Replace when I supply real samples.
LinkedIn posts: three placeholder cards. Replace when I supply the links.
Netlify is NOT connected to the repo, so a push does not go live. Deploy by uploading only index.html, assets/rafay.jpg and assets/rafay.webp from a clean folder (Netlify MCP deploy). Do not upload CLAUDE.md, README.md or assets/profile_picture_rafay.png.
"Creative strategy" was removed from the skills on purpose. Storytelling is enough.
The "same bug, two reports" demo in Identity is a made-up example and is labelled as such on the page.
Tilt is on the small inner cards (.tilt), not on the big test cards.

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