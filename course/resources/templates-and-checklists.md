# Templates and Checklists

Everything referenced in the lessons. Each section can be a separate PDF or Google Doc for the download area.

---

## 1. Email Template Pack (15 scenarios)

Fill in the brackets, paste into the C1 prompt from the Prompt Library (or use as a starting point), then edit so it sounds like you.

| # | Scenario | Bullets to give the AI |
|---|---|---|
| 1 | Ask a professor for an extension | course, assignment, honest reason, new date proposed, work done so far |
| 2 | Ask for a recommendation letter | course/year, grade or project, deadline, what to include, thank-you |
| 3 | Reschedule a meeting | conflict, two alternatives, same agenda |
| 4 | Follow up after no reply | date of first email, one clear ask |
| 5 | Decline a request politely | what you're declining, honest reason (optional), alternative |
| 6 | Ask a manager for feedback | project, what you'd like feedback on, best time to talk |
| 7 | Ask for a raise or more responsibility | your contributions, ask, timing (use AI for a draft only, and think carefully first) |
| 8 | Thank-you after an interview | role, one specific thing discussed, interest in next steps |
| 9 | Networking request | how you found them, one specific question, 15-minute ask |
| 10 | Introduce yourself to a new team | role, start date, what you're excited to learn |
| 11 | Report a problem to a landlord or service | what's wrong, dates, previous contact, requested fix and deadline |
| 12 | Group project reminder | task, deadline, who owns what, kind tone |
| 13 | Out-of-office message | dates, backup contact |
| 14 | Follow up on a job application | role, date applied, brief interest restatement |
| 15 | Apology for a mistake at work | what happened, what you did to fix it, how you'll prevent it |

---

## 2. Formula Cheat Sheet (plain English)

Works in Excel and Google Sheets unless noted. Ask AI to explain any of these, and test on a few rows.

| Formula | What it does | Example |
|---|---|---|
| `SUM` | Adds numbers | `=SUM(B2:B20)` |
| `AVERAGE` | Average of numbers | `=AVERAGE(B2:B20)` |
| `COUNT` / `COUNTA` | Counts numbers / non-empty cells | `=COUNTA(A2:A50)` |
| `IF` | Does one thing if true, another if false | `=IF(B2>100,"High","Low")` |
| `SUMIF` | Adds numbers that meet a condition | `=SUMIF(G:G,"West",F:F)` |
| `COUNTIF` | Counts cells that meet a condition | `=COUNTIF(D:D,"Sticker Pack A")` |
| `VLOOKUP` / `XLOOKUP` | Finds a value in a table (XLOOKUP is newer and may not exist in older versions) | `=VLOOKUP(A2,Sheet2!A:B,2,FALSE)` |
| `TRIM` | Removes extra spaces | `=TRIM(A2)` |
| `PROPER` | Capitalizes Each Word | `=PROPER(A2)` |
| `TEXT` | Formats a number or date as text | `=TEXT(C2,"yyyy-mm-dd")` |
| `IFERROR` | Shows a friendly value if there's an error | `=IFERROR(A2/B2,"")` |
| `CONCAT` / `&` | Joins text | `=A2&" "&B2` |
| `TODAY` | Today's date | `=TODAY()` |
| `ROUND` | Rounds a number | `=ROUND(B2,2)` |

**Rule:** AI suggests. The spreadsheet calculates.

---

## 3. Practice Spreadsheet (messy data)

File: `practice-spreadsheet.csv` (import into Google Sheets or Excel). All data is fictional.

Built-in problems to practice on:
- Names in mixed capitalization with extra spaces (Lesson 3.2).
- Dates in three formats, some ambiguous (like 3/4/25).
- A duplicate order (rows 1002 and 1007).
- A trailing space in a product name ("Sticker Pack A ") that breaks lookups (Lesson 3.5).
- Class year written many ways (Fr, freshman, Soph, Jr, 3rd, Sr, senior…).
- A blank Revenue column to fill with `Units × Unit Price`.

---

## 4. Resume Bullet Builder Worksheet

Complete one per experience **before** using AI.

```
Role / organization / dates:
What I actually did (plain language, 3–6 lines):
Tools or methods I used:
Who it helped or who I worked with:
Numbers I actually know (how many, how often, how long, how much):
Anything that went well or improved (with proof, if any):
Things I did NOT do or only helped with (so I don't overstate):
```

---

## 5. Job Posting Match Checklist

- [ ] I listed the must-have requirements from the posting.
- [ ] I matched each must-have to a real bullet, project or class.
- [ ] I noted honest gaps and will not claim them.
- [ ] My resume uses the posting's wording only where accurate.
- [ ] My cover letter names the correct company and role.
- [ ] My cover letter has one specific, true reason for this company.
- [ ] Every claim can be explained in an interview.
- [ ] I checked whether the application asks about AI use, and followed it.
- [ ] Contact details and links are correct.

---

## 6. Study Plan Template

| Day | Time | Topic | Method (recall / practice problems / review) | Done? |
|---|---|---|---|---|
| | | | | |

**Spaced-review checklist**
- [ ] Review new material within 24 hours.
- [ ] Review again after 3 days.
- [ ] Review again after 1 week.
- [ ] End each session with 5 minutes of recall without notes.
- [ ] Log your weakest 2 topics and give them more time.

---

## 7. Side Project 30-Day Planner (one page)

```
Idea (one sentence):
Who it's for:
What problem it solves:
Hours per week I have:   Budget:
Success measure (decide BEFORE starting):
   e.g., "At least 5 people say they'd pay $X."

Week 1: Research and talk to 5 real people. Tasks:
Week 2: Build the simplest version. Tasks:
Week 3: Show it to real people. Tasks:
Week 4: Review and decide. Tasks:

Things to verify (rules, licenses, taxes, platform policies) with official sources:

What happened / what I learned:
Next step (continue, change, or stop):
```

**Idea check questions:** Who is the customer? Why would they pay? Who else does this? How will they find me? What would make me stop?

---

## 8. AI Fact-Check and Privacy Checklist (print and keep)

**Before you trust it**
- [ ] I flagged every number, name, date, quote and source.
- [ ] I verified each one using a reliable source (not the AI).
- [ ] I opened links and confirmed they say what the AI claimed.
- [ ] Anything I couldn't verify was cut or marked unverified.
- [ ] I matched my checking effort to the stakes.

**Before you paste it**
- [ ] No passwords, login codes, ID or account numbers.
- [ ] No medical information.
- [ ] No other people's private details.
- [ ] No confidential school, work or client information.
- [ ] I used placeholders like [CLIENT] where needed.
- [ ] I checked my tool's data and privacy settings.

**Before you use it**
- [ ] It's allowed by my class or workplace.
- [ ] The thinking is mine.
- [ ] I could explain it without AI open.
- [ ] It sounds like me.
- [ ] I'd be comfortable saying how I made it.

---

## 9. Tool Update Guide

AI tools change often. When something looks different:

1. **Look for the same basics:** message box, upload button, new chat, settings.
2. **Names vary:** "temporary chat," "private mode," "memory," "projects," "data analysis" and "web search" are called different things in different tools.
3. **Some features need a paid plan** or aren't in every region. If you can't find something, check the tool's help page, and use the free workaround from the lesson (for example, paste a small sample instead of uploading a file).
4. **Formulas are more stable than menus.** In spreadsheets, ask for the formula and use the app's help for menu steps.
5. **Re-read the privacy settings** after big updates.
6. **The habits don't change:** RCTF prompts, fix-it follow-ups, check it, protect it, own it.

Last reviewed: [date]. Tell [your email/handle] if a lesson looks out of date.
