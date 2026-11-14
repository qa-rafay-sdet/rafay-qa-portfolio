# rafay.spec — QA Portfolio

A portfolio that runs a "live test run" on its owner: each section is an `it('should …')` test card that goes QUEUED → RUNNING → PASS as it scrolls into view. A runner panel (desktop) or progress pill (mobile) tracks the suite, and a final report shows the real elapsed time.

**Live:** https://rafay-spec.netlify.app

## Sections
1. Hero: `it('should introduce the tester')`
2. Identity: tester, UX eye, storyteller, plus a "same bug, two reports" demo
3. Skills: daily testing, UX, storytelling, tools, learning now
4. Projects: placeholder cards until real samples are added
5. LinkedIn posts: placeholder cards until links are added
6. Automation: fails on purpose, retries once, passes ("still compiling")
7. Contact, then the final report with confetti and a re-run button

## Notes
- One self-contained `index.html`, inline CSS/JS, no build tools. Images live in `/assets`.
- Works from 320px to 1920px+. With JavaScript off, every card shows PASS and all content stays visible.
- The contact form is visual only.
