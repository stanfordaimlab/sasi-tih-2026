# SASI Technology in Healthcare — Fall 2026 Course Hub (starter)

This is the starter scaffold for the Fall 2026 course hub. Push it to GitHub, turn on
Pages, and you have a live site. Everything is Markdown; the theme handles design.

## What this hub is (and isn't)

- The hub is the **single front door** for students: schedule, session pages, reading
  guides, FAQ, logistics. It is the only link we ever share.
- The hub is **not** the workbook. The designed note-taking workbook PDF is a separate
  object, linked from the hub, released once before Session 1.
- The hub is **not private**. Treat every page as public (see Security below).

## Setup (once, ~20 minutes)

1. Create a new GitHub repo (suggested name: `sasi-tih-2026`). Public is fine given the
   security rules below.
2. Copy these files in, commit, push.
3. Repo → Settings → Pages → Source: `main` branch, root folder. Save.
4. Site appears at `https://<account>.github.io/sasi-tih-2026/` within a few minutes.
5. Edit `_config.yml`: set `url` and `baseurl` to match.

The theme is [Just the Docs](https://just-the-docs.com) loaded via `remote_theme` —
no local build needed; GitHub Pages builds it automatically on every push. Sidebar
navigation and search come free.

## Security rules (read before adding any content)

GitHub Pages has **no real password protection** — private repos still publish public
sites. Our posture, same as last year's Miro board:

1. **Unlisted URL** — never posted publicly, shared only in the student Slack and email.
2. **Optional passphrase gate** — run [StatiCrypt](https://github.com/robinmoisson/staticrypt)
   over the built pages to AES-encrypt them behind a shared passphrase (like `SASI2026`).
   Nice-to-have, not required, because of rule 3:
3. **The hard rule: nothing sensitive ever goes on the hub.** No Zoom links or passcodes,
   no student names/emails/PII, no unreleased speaker info, no grades/survey responses.
   Zoom links live in Slack + calendar invites only. The hub links *to* Slack, not the
   other way around for secrets.
4. **No copyrighted PDFs, ever.** Do not commit or upload paywalled papers, book
   chapters, or reports (last year's handout attached a book chapter — we're not
   repeating that). Open-access/CC-licensed papers are fine WITH a license check.
   Everything else gets a reading card that links out. See `readings.md`.

## Update workflow (mid-season)

1. Edit the Markdown, commit with a one-line message describing the change.
2. Add a line to `changelog.md` (students see this page — it's how they trust the hub).
3. Post the change in Slack #announcements: what changed, one sentence.
4. Dara approves anything student-facing before it ships. Small typo fixes: just go.

## File map

| File | Job |
|---|---|
| `index.md` | Home: season-at-a-glance, the one table with all dates/times |
| `logistics.md` | How the program works: session anatomy, Slack, surveys → certificate, absences, contacts |
| `sessions/` | One page per session (1–2 drafted, 3–4 skeletons) + optional lab |
| `readings.md` | Reading cards: orientation blurb + guiding question + link. Copyright rules live here |
| `faq.md` | Corrected FAQ (it's a Fall internship — last year's doc said "Summer" throughout) |
| `changelog.md` | Every student-visible change, newest first |

## Placeholders

Anything in `[BRACKETS]` needs input — most say who from (`[DARA]`, `[LARRY]`).
Search the repo for `[` before launch.
