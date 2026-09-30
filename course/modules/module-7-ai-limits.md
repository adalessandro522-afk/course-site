# Module 7: AI's Limits: Use It Wisely (16 min)

*Outcome 7: recognize AI's limits: hallucinations, privacy risks, and when not to trust it.*

**Notes for Antonio:** this module is your credibility peak. It uses what your resume says you did (testing AI-assisted research workflows; back-testing AI-generated forecasts across 31 companies and 249 prediction-versus-actual observations; finding optimism bias and weak directional accuracy). **Only state what you can support, and confirm that your firm is fine with you describing it.** Don't share confidential firm data, and don't imply the results prove anything general about AI. Say "in my testing" and "in that sample."

---

## Lesson 7.1: Hallucinations and the 3-step fact-check (6 min)

### Script

[SCREEN: You on camera.]

Earlier I told you about hallucinations, when AI states something false with total confidence. Now let's make it real.

At my internship, part of my job is testing where AI is reliable in research and where it isn't. In one project, I compared AI-generated forecasts against what actually happened, across dozens of companies. In that sample, the forecasts leaned optimistic, and their direction was often not much better than simple alternatives. The AI wasn't lying. It sounded confident and reasonable. It just wasn't reliable enough to trust without checking.

[SCREEN: Show a slide: "Confident ≠ correct."]

That's the lesson. **Confident is not the same as correct.**

[SCREEN: Show a list of high-risk categories: names and quotes, statistics, dates, citations and links, legal or medical claims, recent events, math.]

Here's where hallucinations show up most. Statistics and numbers. Quotes. Sources, meaning book titles, articles and links that look real but don't exist. Dates. Legal, medical and financial claims. Recent events. And math.

[SCREEN: Ask the AI for sources on a topic. Then search for each source on Google Scholar or a library site. Show one that doesn't exist.]

Watch this. I'll ask for sources, then look each one up. This one exists. This one, I can't find anywhere. If I'd put that in a paper, that's a serious problem.

Now here's my three-step fact-check.

[SCREEN: Show three steps on screen, one at a time.]

**Step one: Flag.** Underline every claim that could be wrong if it's not true: numbers, names, dates, quotes, sources.

**Step two: Verify.** Check each flagged claim against a reliable primary source: the official website, the original document, a textbook, a peer-reviewed article or a government source. Don't verify with the AI itself. Asking "are you sure?" usually just gets you a confident answer either way.

**Step three: Decide.** If you can't verify it, cut it, or say clearly that it's unverified.

[SCREEN: Show an "Ask for uncertainty" prompt.]

You can lower the risk by asking: "Only include information you're confident about. Mark anything uncertain with [VERIFY]. Don't invent sources." That doesn't make it perfect. It just gives you a to-check list.

[SCREEN: Show a risk scale: low, medium, high.]

Also match your effort to the stakes. A brainstorm for a party? Low risk. A resume, a school paper, a business decision, health or money? Check everything.

[SCREEN: On camera.]

AI is a first draft, not a source. If you cite it, you're responsible for it.

**Good to know:** some tools can search the web and show links. That can help, but you still open the links and confirm they say what the AI claims.

### Worked example
**Scenario:** Jordan asks for "three statistics about student sleep and grades" for a class presentation.

The AI returns three confident numbers with source names. Jordan applies the steps:
1. **Flag:** all three numbers and all three sources.
2. **Verify:** searches each source. Two can't be found. One exists, but the number is different.
3. **Decide:** uses only the verified one, with the correct number, cited from the actual source.

### Prompt templates
```
Answer the question below. Only include information you're confident about. Mark anything uncertain with [VERIFY]. Do not invent sources, quotes, statistics or links. If you don't know, say so.

Question: [paste]
```
```
List every factual claim in the text below (numbers, names, dates, quotes, sources) so I can verify each one. Don't say whether they're true; just list them.

Text: [paste]
```
```
What are the most likely ways the answer above could be wrong or out of date? What should I check, and where?
```

### Do it in 10 minutes
Ask AI for three facts about a topic you can check. Flag, verify each with a reliable source, and note how many were right.

### Quiz
1. **What are the three steps?** Flag, verify, decide.
2. **Should you verify a claim by asking the AI "are you sure"?** No. Check a reliable independent source.
3. **Name three types of information that are high-risk for hallucinations.** Any of: statistics, quotes, sources and links, dates, legal or medical claims, math.

---

## Lesson 7.2: Privacy: what never to paste (5 min)

### Script

[SCREEN: You on camera. Then a chat box with a cursor.]

Every time you paste something into an AI tool, you're sending information to a company's servers. That's usually fine for a grocery list. It's not fine for everything.

[SCREEN: Slide with a red list: "Never paste."]

Here's my "never paste" list. Passwords and login codes. Social Security numbers and government ID numbers. Bank, card and account numbers. Medical information. Other people's private details, like classmates' grades or a friend's personal story. And anything confidential from your school, job or clients.

[SCREEN: Highlight "work and school."]

That last one matters. If you have an internship or job, you may have signed a confidentiality agreement, and company policy may prohibit or restrict AI tools. **Read your policy or ask your manager before using AI with anything from work.** In my internship, that's a rule I take seriously. Even something that looks harmless can be confidential.

[SCREEN: Show a "Safer way" slide: replace names with placeholders, remove numbers, summarize instead of pasting.]

The safer way. Replace names with placeholders: [CLIENT], [MANAGER]. Remove account numbers and addresses. Describe the situation instead of pasting the original. Or use a made-up example with the same structure.

[SCREEN: Open the settings of your AI tool. Show data controls.]

Then check your tool's settings. Many AI tools let you turn off using your chats for training, or use temporary or private chat modes. **Good to know:** policies and settings vary by company and plan and they change, so read the current policy yourself, and don't assume a private mode means nothing is stored.

[SCREEN: Show a phone with an AI app asking for microphone and camera access.]

Watch app permissions too. If an AI app asks for access to your contacts, photos or files, ask yourself whether it needs that.

[SCREEN: Show a quick check: "Would I be OK if this appeared on the front page of the school paper?"]

A quick test: would I be okay if this text were seen by someone I didn't choose? If not, don't paste it.

[SCREEN: On camera.]

Privacy mistakes are hard to undo. It takes ten seconds to remove a name. It's worth it.

### Worked example
**Scenario:** Maya wants help with an email about a performance issue with a coworker.

**Risky:** pasting the coworker's name, review details and an internal document.

**Safer prompt:**
```
I need to send a respectful message to a coworker ([COWORKER]) about missed deadlines on a shared project. I want to be clear, not accusatory, and suggest a short check-in. Draft it in under 100 words. I'll add specifics myself.
```
Maya also checks the company AI policy before using the draft, and asks HR for guidance since it's a sensitive matter.

### Prompt templates
```
Help me rewrite the details below with placeholders so I can safely use them in an AI tool. Replace names, companies, numbers, addresses and anything identifying with [PLACEHOLDERS], and list what you replaced.

Text: [paste ONLY if it contains no sensitive data; otherwise describe it yourself]
```
```
Here's a fictional example with the same structure as my real situation: [description]. Draft a [type of message] for it.
```

### Do it in 10 minutes
1. Open your AI tool's privacy settings and note what they say about training and history.
2. Write your own "never paste" list of five items.
3. Check the AI policy of your school or workplace.

### Quiz
1. **Name three things you should never paste into an AI tool.** Any of: passwords, ID or account numbers, medical info, other people's private details, confidential work or school info.
2. **What's a safer alternative to pasting real details?** Placeholders or a fictional example.
3. **Who should you check with before using AI for work?** Your employer's policy or your manager.

---

## Lesson 7.3: Integrity and when not to use AI (5 min)

### Script

[SCREEN: You on camera.]

Last lesson in the core course, and it's about judgment. When should you use AI, and when shouldn't you?

[SCREEN: Show a simple three-column chart: "Good fit," "Use with care," "Skip it."]

**Good fit:** first drafts, brainstorming, rewriting, summarizing your own material, explaining concepts, making practice questions, formatting.

**Use with care:** anything with facts, numbers or sources. Anything private. Anything with rules attached, like class assignments and workplace documents. Here you check, and you follow the rules.

**Skip it:** high-stakes decisions on your own, like medical, legal, mental health or major financial decisions. Anything where you're required to do the work without help. Personal messages where authenticity is the point, like an apology to a friend, a condolence note, or a thank-you that should be in your own words.

[SCREEN: Show a case study: a student submitting AI-written work.]

**Integrity.** Submitting AI-written work as your own where it isn't allowed is cheating, even if it's tempting when you're tired and behind. The consequences can include failing the assignment or worse. And it costs you the skill.

At work, it can be just as serious. Sharing confidential information, sending unchecked AI content to a client, or presenting AI work as your own analysis can damage trust. Where your company or school requires disclosure, disclose. When in doubt, ask.

[SCREEN: Show the human-in-the-loop idea. Use a diagram: AI drafts → You check → You decide → You own.]

This is what I focus on in my own work: a human-in-the-loop approach. The AI helps gather and challenge information. The calculations should be checkable, in something like a spreadsheet. And a person approves the assumptions and owns the final call. Responsibility doesn't move to the AI. You can use that pattern for almost anything.

[SCREEN: Show the "before you send" checklist.]

Before you use anything AI helped make, ask five questions. Is it allowed here? Is it accurate? Is it private-information-safe? Is it in my voice and does it reflect my thinking? Would I be comfortable explaining exactly how I made it?

[SCREEN: On camera.]

If you can answer yes to all five, you're using AI well. That's the goal. Not to avoid AI, and not to depend on it. Just to be good at using it.

### Worked example
**Scenario:** three situations, how to decide.

1. Jordan wants AI to explain a reading before class. **Good fit.** Check against the text.
2. Maya wants AI to write her graded reflection paper. **Skip it** unless her instructor explicitly allows it. Instead, ask for feedback on her own draft if permitted.
3. Jordan wants to send a heartfelt apology to a friend. **Skip it,** or use it only to help organize thoughts, then write it in Jordan's own words.

### Prompt templates
```
I'm thinking of using AI to [task]. Here are the rules I know about: [school/work policy]. Help me think through: (1) is this likely allowed, (2) what could go wrong, (3) a safer or better way to use AI here. Remind me to confirm with [instructor/manager].
```
```
Review this draft and list anything that could count as misrepresenting my own work, privacy risk, or unverified claim: [paste, without sensitive info].
```

### Do it in 10 minutes
Fill in the five-question checklist for one real task you plan to do with AI this week. Note one task you'll choose not to use AI for.

### Quiz
1. **Give one task that's a good fit and one that you should skip.** Good: first drafts or brainstorming. Skip: submitting AI-written work where it's not allowed, or high-stakes medical/legal decisions.
2. **What does human-in-the-loop mean?** A person checks, decides and owns the final result, and AI only assists.
3. **What should you do if you're unsure whether AI use is allowed?** Ask your instructor or manager and follow the policy.
