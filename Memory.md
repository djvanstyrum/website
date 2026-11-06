# Project notes

Decisions, progress, learnings and key takeaways for the website. Newest at the top.

## 2026-11-06 — Code on GitHub

### Progress
- The website code is now on GitHub in a **private** repository: https://github.com/djvanstyrum/website (only DJ can see it).
- Installed on the Mac: Apple's command line developer tools (includes Git) and GitHub CLI (`~/bin/gh`, signed in as djvanstyrum).
- Commits use DJ's private GitHub "noreply" email, so the real email address isn't stored in the code history.

### Decisions
- Private repository, only for storing the code. Not putting the site online via GitHub Pages yet (on a free account that would need a public repository).

### How it works from now on
- After each change, Claude saves a version ("commit") and sends it to GitHub ("push"). Just ask: "save this to GitHub".

### Learnings
- Git = the tool that keeps track of versions of your files. GitHub = the website where those versions are stored online.
- A "repository" (repo) is a project folder on GitHub.
- Signing in to GitHub from the Mac is done once, with a one-time code at github.com/login/device. You never give Claude your password.

## 2026-11-05 — First version of the website

### Progress
- Built the first version: `index.html` (one page, everything in one file).
- Sections: intro, About (Over mij), Work (Werk, a timeline), Contact (LinkedIn button).
- Language switch NL/EN at the top right. Default is Dutch, or English if the visitor's browser is set to another language. The site remembers the visitor's choice.
- Checked on a phone-sized screen and on desktop.

### Content used (from LinkedIn, nothing invented)
- Founder, treebytree (2022 – present)
- Owner, Impact360 (2019 – present), impact investing
- Strategy & Partnerships, Justdiggit (2019 – 2022), with LinkedIn's description of Justdiggit
- Co-founder, Xindao (1986 – 2018)
- Erasmus University Rotterdam; based in the Netherlands
- LinkedIn's "About" section is empty, so the About text is a short summary of the jobs above.

### Decisions
- Design: simple, modern, minimal. Off-white background, dark text, a dark green accent colour (a nod to trees/impact). Fonts: Fraunces (headings) and Inter (body text). Automatic dark mode when the visitor's device is set to dark.
- Contact via LinkedIn only for now. No email address on the site yet (spam risk; DJ to decide).

### Open / next steps
- Add a photo of DJ (put it in `content/`).
- Decide whether to show an email address.
- Possibly a few lines about what treebytree does, and DJ's own words for the About text.
- Put the site online (hosting + domain name).

### Learnings
- Folders vs. files: Finder's "New Folder" makes a folder even if you name it `.md`. Text files are made with TextEdit (Format → Make Plain Text) or by Claude.
- Projects live in `~/Projects` (reachable via the Finder sidebar). Each project has its own CLAUDE.md and Memory.md.
- To preview the site locally, Claude starts a small web server and opens http://127.0.0.1:8000. You can also just double-click `index.html` to open it in your browser.

## 2026-11-05 — Setup
- Project folder set up in ~/Projects/website.
