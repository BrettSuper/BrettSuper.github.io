# Cutting with the BS — Setup & Publishing Guide

No coding required. Everything happens in a web browser.

---

## Part 1: Put the site online (one time, ~15 minutes)

1. **Create a GitHub account** at github.com (free). Pick any username.

2. **Create a repository.** Click the "+" in the top right → "New repository."
   - Name it exactly: `YOURUSERNAME.github.io` (replace YOURUSERNAME with
     your actual GitHub username — this exact name is what makes it a free
     website)
   - Set it to Public
   - Click "Create repository"

3. **Upload the site files.** On the new repository page, click
   "uploading an existing file." Drag in everything inside this folder:
   - `index.html`
   - `style.css`
   - the `issues` folder (drag the whole folder)
   - Click "Commit changes" at the bottom.

4. **Wait ~2 minutes**, then visit `https://YOURUSERNAME.github.io`
   — your site is live.

---

## Part 2: Before you share it (5 minutes)

1. Open `index.html` and `issues/issue-01.html` on GitHub (click the file,
   then the pencil icon to edit).
2. Find `YOUR-EMAIL-HERE@example.com` (it appears in both files) and replace
   it with the email address you want subscribers to use.
3. Replace the placeholder text in `issues/issue-01.html` with your real
   essay — the file has comments (the lines starting with `<!--`) telling
   you exactly what goes where. Paragraphs go inside `<p>` tags.
4. Update the date on the issue page ("Month 2026" → the real month).
5. Click "Commit changes" after each edit. The live site updates in about
   a minute.

---

## Part 3: Publishing a new issue (each time, ~15 minutes)

1. On GitHub, open the `issues` folder, click the newest issue file, and
   use the "Copy raw file" button (or open the pencil editor and copy all
   the text).
2. Back in the `issues` folder, click "Add file" → "Create new file."
   Name it `issue-02.html` (then 03, 04, ...).
3. Paste, then edit: the issue number (it appears a few times), the date,
   the headline, the deck, and the body text. Commit.
4. Open `index.html` and:
   - Update the "LATEST ISSUE" block at the top to point to the new issue
     (the comments in the file walk you through it)
   - Add the previous issue as a new line at the top of "The Record"
     archive list (copy an existing `<li>` block and edit it)
   - Commit.
5. Send your email with a link to the new issue page:
   `https://YOURUSERNAME.github.io/issues/issue-02.html`

---

## The email side (you're handling this — quick notes)

- Keep the email itself simple: a subject line, a 2–3 sentence hook, and
  the link to the issue on the site. Email clients will mangle fancy
  formatting; the site is where the design lives.
- A plain Gmail BCC works for the first few dozen subscribers. Past
  ~50–100, look at Buttondown (buttondown.com) — it's built for exactly
  this, and its signup form can replace the mailto link in the subscribe
  box (the HTML comments show you where).

---

## Optional: a custom domain later

If you buy a domain (e.g. cuttingwiththebs.com, ~$12/year from Namecheap
or Cloudflare), GitHub Pages can use it for free: repository → Settings →
Pages → Custom domain. The registrar's help pages walk through the DNS
step, or ask Claude when you get there.

---

## If anything breaks

Every change is saved in the repository's history, so nothing is ever
truly lost. If a page looks wrong after an edit, the usual culprit is a
deleted `<` or `>` character. Paste the file into a Claude chat and ask
what's off — fastest fix there is.
