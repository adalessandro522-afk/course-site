# Module 3: Spreadsheets Made Simple (27 min)

*Outcome 3: use AI to build, clean and analyze spreadsheets and write formulas.*

**Practice file:** the "Practice Spreadsheet" Google Sheet from Stage 3 (see `course/resources/templates-and-checklists.md`). It has fake, messy data only. Tell students never to upload real customer, employee or financial data.

**Tool note to say on camera:** the lessons use general Excel and Google Sheets wording. Menu names and features (like built-in AI helpers or file-analysis tools) vary by app, version and plan. Formulas themselves are much more stable.

---

## Lesson 3.1: Get formulas written and explained (6 min)

### Script

[SCREEN: You on camera. Then a spreadsheet with sales data and an empty column labeled "Total."]

If you've ever Googled "Excel formula for..." and clicked through five confusing forum posts, this lesson is for you.

A formula is an instruction you type into a cell to calculate something. Like adding numbers, or looking up a value. You don't need to memorize them anymore. You need to describe what you want in plain English.

[SCREEN: Show the sheet: columns A to E: Date, Product, Units, Price, Region. Cell F1 says "Revenue."]

Here's my sheet. I want a revenue column: units times price. Let me ask the AI, and I'll tell it exactly how my sheet is set up.

[SCREEN: Type the prompt slowly. Highlight "columns A to E" and "row 1 has headers."]

That detail matters. It needs to know which column is which, where the data starts and which program I'm using, because Excel and Google Sheets are slightly different.

[SCREEN: Paste the formula into F2. Drag it down. Show results.]

It gives me a formula, `=C2*D2`. I paste it in the first row and drag it down. Works.

[SCREEN: Type the follow-up: "Explain that formula in plain English."]

Now the most important habit. Ask it to explain. "Explain this formula piece by piece, so I understand it." If you don't understand a formula, you can't tell if it's right.

[SCREEN: Try a harder one: "Total revenue for the West region only."]

Let's try a harder one. Total revenue for just the West region. The AI suggests a formula with SUMIF. And I ask it to explain that too.

[SCREEN: Test on a few rows by hand, e.g., filter West and sum with a calculator.]

Last step: test it. Pick two or three rows and check by hand. AI formulas are usually right for simple jobs, but always test before you rely on it.

**Good to know:** some spreadsheet apps have a built-in AI assistant, often on paid plans. You don't need it. A separate chat assistant works fine for formulas.

### Worked example
**Scenario:** Jordan runs a small sticker shop and tracks orders.

Columns: A Order date, B Product, C Units, D Unit price, E Shipping. Jordan wants profit per order after a flat $1.50 packaging cost per unit.

```
I'm using Google Sheets. My data starts in row 2 with headers in row 1. Columns: A Order date, B Product, C Units, D Unit price, E Shipping charged to customer. I want a formula for column F that calculates: (units × unit price) + shipping − (units × 1.50 packaging cost). Give me the formula for row 2 and explain each part in plain English.
```
Expected type of answer: `=(C2*D2)+E2-(C2*1.5)`. Jordan tests row 2 by hand.

### Prompt templates
```
I'm using [Excel / Google Sheets]. My data starts in row [2], headers in row 1. Columns: [A: name, B: name, C: name…].
I want [describe the goal in plain English] in [cell or column].
Give me the formula for the first row, explain it piece by piece, and tell me if there's anything I should double-check.
```
```
Explain this formula in plain English, one part at a time: [paste formula]
```

### Do it in 10 minutes
Open the practice sheet or make five rows of fake data. Ask AI for a formula that calculates something useful (a total, an average, a count), test it by hand on two rows, and ask for an explanation.

### Quiz
1. **What details should you give when asking for a formula?** The app, the column names and layout, where data starts, and your goal.
2. **Why ask the AI to explain the formula?** So you can understand and verify it.
3. **How do you check a formula?** Test it by hand on a few rows.

---

## Lesson 3.2: Clean messy data (6 min)

### Script

[SCREEN: You on camera. Then the messy sheet: names in different cases, dates in mixed formats, phone numbers with dashes and without, duplicate rows, extra spaces.]

Messy data is the reality of spreadsheets. Names in all caps, dates written five different ways, duplicate rows, extra spaces. It takes forever to fix by hand, and AI can help.

First, safety. **Make a copy of your sheet before you touch anything.** Rename it "Original—do not edit." Work on the copy. Always.

[SCREEN: Right-click the sheet tab, duplicate it. Rename.]

Second, **never upload real personal data**. Names, emails, phone numbers of real people, or private business info don't belong in a public AI tool. Use fake data to practice, or remove the sensitive columns first.

[SCREEN: Show the practice sheet.]

Here's my practice data. Let's fix the names first. They look like "jOHN smith," "MARIA LOPEZ," and "  aisha khan ". I ask: "I'm using Google Sheets. Column A has full names in inconsistent capitalization with extra spaces. Give me a formula to clean into Proper Case."

[SCREEN: Show result: `=PROPER(TRIM(A2))`. Paste it into column F. Drag down.]

I get a formula: trim removes extra spaces, proper capitalizes each name. Paste it in a new column. Don't overwrite the original.

[SCREEN: Now dates. Show mixed formats: "3/4/25," "March 4, 2025," "2025-03-04".]

Dates are trickier. I'll say: "Here are five example dates in different formats. Tell me how to convert them all to one format, and warn me about anything ambiguous." Look at this: 3/4/25 could be March 4th or April 3rd. A good answer flags that. That's a human decision, not the AI's.

[SCREEN: Now duplicates. Use Remove duplicates tool or show a formula to flag them.]

For duplicates, don't ask the AI to delete them. Ask how to flag them first. Then review them, then delete.

[SCREEN: On camera.]

The pattern: copy the data, ask for a formula or steps, apply it in a new column, check a sample, and only then replace.

### Worked example
**Scenario:** Maya has a fake contact list from a club event: names, emails, signup dates, a "Year" column with entries like "Sr", "senior", "SENIOR", "4th".

```
I'm using Excel. Column D has class year entries like "Sr", "senior", "SENIOR", "4th", "Jr", "junior", "3rd". Give me a formula to standardize them into "Freshman", "Sophomore", "Junior", "Senior". Tell me what happens if an entry doesn't match, and how to flag those.
```
Maya checks unmatched entries by filtering the new column for a flag like "CHECK".

### Prompt templates
```
I'm using [Excel / Google Sheets]. Column [X] has [describe the mess, with 3–5 fake examples]. Give me a formula or steps to [clean into this format]. Show it for row 2, tell me about edge cases, and how to flag anything it can't handle.
```
```
Here are 8 rows of sample data from my sheet (no real personal info): [paste]. Suggest a cleaning plan: what's inconsistent, what should be standardized, and what needs a human decision.
```
```
How can I flag duplicate rows in [app] without deleting anything? Column [X] is the key.
```

### Do it in 10 minutes
Duplicate the practice sheet. Clean one column using an AI-generated formula in a new column and test it on five rows.

### Quiz
1. **What should you do before cleaning data?** Make a copy of the original.
2. **Why put cleaned results in a new column?** So you keep the original and can compare.
3. **Why not upload real personal data?** It's private information, and public AI tools may store or use it. Use fake data or remove sensitive columns.

---

## Lesson 3.3: Analyze and summarize your data (6 min)

### Script

[SCREEN: You on camera. Then a clean sheet of 40 rows of made-up monthly sales for a small shop.]

You have clean data. Now what does it say? AI can help you find patterns, summarize, and suggest ways to show the results. But this is where you need to be extra careful, because it's very easy to get confident-sounding wrong numbers.

[SCREEN: Show two options: paste a small sample into chat; or upload a file.]

There are two ways to work. Option one: copy a small sample of rows into the chat. Option two: upload the file. **Good to know:** file upload and data analysis features vary by tool and often need a paid plan. The paste method works on free versions but only for small tables.

[SCREEN: Paste 20 rows. Prompt: "What are three notable patterns? What questions should I ask next?"]

Let's ask something open: "Here's a sample of my data. Describe three notable patterns and suggest questions I should investigate." AI is good at spotting things like "sales dip in February" or "one product drives most revenue."

[SCREEN: Now ask a specific numeric question. "What's the total revenue?"]

Now a specific number: total revenue. It gives me an answer. Is it right?

[SCREEN: Run =SUM in the sheet. Compare. Show them matching or not.]

Here's the rule I use at work: **AI suggests, the spreadsheet calculates.** Don't trust math done by a chat assistant. Ask it for the formula, and let Excel do the calculation. That way the calculation is visible and checkable.

[SCREEN: Ask: "What formula would give me total revenue by product?" then build a small summary table. Ask for chart suggestions.]

So I ask it for the formula, build a summary table, then ask: "What chart would best show this, and why?" It says a bar chart for comparing products, a line chart for change over time. I make the chart in the spreadsheet.

[SCREEN: On camera. Show a slide: "Correlation ≠ causation. Small samples mislead. Ask 'what else could explain this?'"]

One more caution. If AI says "sales went up because of the promotion," that's a guess. Data can show that two things happened together, not that one caused the other. Ask it: "What other explanations could there be?" Use it to generate questions, not conclusions.

### Worked example
**Scenario:** Jordan has 3 months of sticker-shop orders (fake data, 60 rows).

```
Here's a sample of my sales data (columns: Date, Product, Units, Revenue). Don't calculate totals yourself. Instead:
1) Describe 3 patterns you notice.
2) Give me spreadsheet formulas to calculate total revenue, revenue by product, and average order size.
3) Suggest one chart for each question.
4) List 3 other explanations I should consider before drawing conclusions.
Data: [paste]
```
Jordan builds the formulas, compares one against a hand calculation, and notes which claims need more data.

### Prompt templates
```
Here is a small sample of my data: [paste]. Describe up to 3 patterns, and list questions I should investigate. Don't state any exact totals; give me formulas instead.
```
```
I want to answer: [question]. My columns are [names] in [app]. Give me the formula or pivot-table steps and what the result will look like.
```
```
What chart best shows [question] with this data, and why? Suggest one alternative and when it would be worse.
```
```
You said [claim]. What other explanations could there be, and what data would help tell them apart?
```

### Do it in 10 minutes
Use the practice sheet. Ask for patterns, then ask for the formula for one number. Compare it with what the AI first said (if it gave a number).

### Quiz
1. **What's the rule for calculations?** AI suggests; the spreadsheet calculates.
2. **Can AI prove that A caused B?** No. It can point out patterns, which need further investigation.
3. **What should you avoid uploading?** Real personal or confidential data.

---

## Lesson 3.4: Build a simple tracker or budget (5 min)

### Script

[SCREEN: You on camera. Then a blank spreadsheet.]

You don't have to start from a template you found online and then bend to fit. You can describe what you need and have AI design the layout. Let's build a simple monthly budget.

[SCREEN: Type the prompt: "I'm a college student with a part-time job... Design a simple monthly budget spreadsheet layout."]

I tell it what I track, and I ask for a layout: column headers, and what goes in each. I say "Don't use real numbers; use placeholder values."

[SCREEN: Show the proposed layout. Type it into the sheet.]

It suggests: a section for income, a section for fixed costs, a section for variable spending, and a total row for each. I create the columns.

[SCREEN: Ask for the formulas. Paste them.]

Then I ask: "Give me formulas for each total, and for money left over." I paste them in and test with easy numbers, like ten and twenty, to make sure the totals work.

[SCREEN: Add a simple rule: conditional formatting for negative amounts.]

Want to go further? Ask for a step-by-step way to highlight negative amounts in red, or to make a dropdown list of categories. "Give me the steps for Google Sheets" is enough.

[SCREEN: Show different trackers: assignment tracker, job application tracker, workout log.]

You can do this with almost anything: an assignment tracker with due dates and status, a job application tracker with company, date applied and follow-up date, an inventory list for a side project.

[SCREEN: On camera.]

Keep it simple. Version one should take ten minutes. You can always add features later. And a note: for real financial decisions, treat this as a planning tool, not financial advice.

### Worked example
**Scenario:** Maya wants a job application tracker.

```
I'm using Google Sheets. Design a job application tracker. I want to track: company, role, date applied, link, status (Applied, Interview, Offer, Rejected), and follow-up date. Suggest column headers, a dropdown for Status, a formula that highlights rows where the follow-up date is today or earlier, and step-by-step instructions to set it up.
```
Maya builds it, then tests by entering one fake row.

### Prompt templates
```
I'm using [app]. Design a simple [tracker/budget] spreadsheet for [my situation]. I want to track [list]. Give me: column headers, a dropdown for [field] with these options [list], formulas for [totals], and step-by-step setup instructions. Use placeholder values, and keep it simple.
```
```
Give me step-by-step instructions in [app] to [add a dropdown / highlight cells / freeze the header row / make a chart].
```

### Do it in 10 minutes
Build a tiny tracker for one thing in your week (assignments, applications, expenses). Enter three fake rows and test every formula.

### Quiz
1. **What should the AI use for numbers in a template?** Placeholder values.
2. **How do you test a new formula?** Use simple numbers you can check in your head.
3. **Is a budget spreadsheet financial advice?** No. It's a planning tool.

---

## Lesson 3.5: Debug errors and check the math (4 min)

### Script

[SCREEN: You on camera. Then a spreadsheet full of errors: #REF!, #N/A, #DIV/0!, #VALUE!.]

You've seen these. Those little error codes in your cells. They look scary, but they're actually clues, and AI is a good translator.

[SCREEN: Click on a cell with an error. Copy the formula.]

Here's how to debug. Copy the formula and the error, and ask: "This formula returns #N/A. Here's the formula and what each column contains. What's the most likely cause and how do I fix it?"

[SCREEN: Show the answer: a lookup value doesn't match because of an extra space or wrong data type.]

Often it's something like a lookup value with a trailing space, or a number stored as text. It tells you what to check, and you look.

[SCREEN: Show a table: #DIV/0! = dividing by zero; #REF! = a deleted or invalid reference; #VALUE! = wrong type of data; #N/A = value not found.]

Quick decoder. Divide by zero. Bad reference. Wrong type of data. Value not found. AI can help with each.

[SCREEN: Now show a formula that runs without errors, but gives a wrong number.]

Now the more dangerous problem: a formula that runs fine but gives the wrong answer. No error, no warning. Maybe it's summing the wrong range, or double counting.

[SCREEN: Show three sanity checks on screen.]

Three quick checks. One: does the total match a rough estimate you can do in your head? Two: recalculate two or three rows by hand. Three: use a different method, like a pivot table or a filter, and see if it gives the same answer.

[SCREEN: On camera.]

And ask the AI itself: "What are common ways this formula could give a wrong answer with my data?" It's good at brainstorming edge cases.

For anything that matters, like grades, invoices, or money, a person double-checks. Always.

### Worked example
**Scenario:** Jordan's `VLOOKUP` returns #N/A for "Sticker Pack A" even though it's in the table. Cause: the table has "Sticker Pack A " with a trailing space. Fix: use `TRIM`.

```
This formula returns #N/A: [paste formula]. My lookup value is in A2 and the table is in Sheet2!A:B. The value "Sticker Pack A" seems to be in the table. List the 4 most likely causes in order, and how to check each.
```

### Prompt templates
```
This formula shows [error]: [formula]. Here's what my cells contain: [describe with fake examples]. What are the most likely causes, and how do I check each?
```
```
This formula runs without errors, but I'm not sure the answer is right: [formula]. What are common ways it could be wrong with data like [description], and what quick checks can I run?
```

### Do it in 10 minutes
Create a deliberate error in the practice sheet (divide by an empty cell). Use the debug prompt, then confirm the fix works.

### Quiz
1. **What does #DIV/0! usually mean?** Dividing by zero (or an empty cell).
2. **Name one way to check a formula that has no error.** Compare with a mental estimate, hand-calculate rows, or use a different method.
3. **Who should double-check high-stakes numbers?** A person, not just AI.
