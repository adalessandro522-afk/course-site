# Module 1: Prompting Foundations (24 min)

*Outcome 1: write clear, effective prompts and fix bad outputs.*

---

## Lesson 1.1: What AI is actually doing (4 min)

### Script

[SCREEN: You on camera.]

Quick question. When AI writes something and it's wrong, why does it still sound so sure of itself?

The answer explains most of the mistakes beginners make, so it's worth four minutes.

[SCREEN: Show a phone's autocomplete: type "See you at" and show suggested words.]

You know autocomplete on your phone? You type "See you at" and it suggests "the", "home", "6". It's predicting the next word based on patterns.

The AI tools we use are called large language models. Fancy name, same core idea, but trained on an enormous amount of text and much more capable. When you send a prompt, it doesn't look up the answer in a database of facts. It generates the most likely useful-sounding response, one small piece at a time.

[SCREEN: Slide with two columns: "Great at" / "Risky at".]

That makes it great at some things: drafting, rewriting, summarizing, brainstorming, explaining, organizing messy information, changing tone. Language jobs.

It's risky at others: exact facts, numbers, quotes, sources, recent events, and anything where being wrong has consequences. Because it's producing likely text, not verified truth, it can produce something that reads perfectly and is false. People call that a hallucination, which just means the AI made something up.

[SCREEN: Ask the AI: "Give me three academic sources on the effect of sleep on exam performance, with links." Show the output. Don't verify yet; say you will in Module 7.]

Look at this. It gave me sources that look real. Some might be. Some might not exist. I'd have to check every one. We'll practice that later.

One more thing. It doesn't remember you between separate chats unless a memory feature is turned on, and it can only use what's in the current conversation. **Good to know:** memory and web search features differ by tool and plan.

So here's the mental model. Treat AI like a very fast, very eager intern. It writes quickly, never complains, and sometimes says something wrong with total confidence. You'd never send an intern's work to a client without reading it. Same rule.

### Worked example
**Scenario:** ask the AI, "What was our class's average on the midterm?" It has no access to that, but a weak tool might still make up a number. Use it to show the AI doesn't know what it can't know, and how phrasing ("if you don't know, say so") changes the answer.

### Prompt template
```
Answer the question below. If you're not sure or don't have enough information, say so instead of guessing, and tell me what I should verify.

Question: [your question]
```

### Do it in 10 minutes
Ask your AI one factual question you already know the answer to (about your school, hometown or a hobby). See whether it's right, and how confident it sounds either way.

### Quiz
1. **Does AI look up answers in a database of facts?** No. It generates likely-sounding text based on patterns.
2. **What's a hallucination?** A made-up or incorrect statement presented as fact.
3. **Which is a better use: drafting an email, or quoting a source from memory?** Drafting an email.

---

## Lesson 1.2: The 4-part prompt formula (6 min)

### Script

[SCREEN: You on camera, then a slide with the letters R-C-T-F.]

Most bad AI answers come from thin prompts. So here's a simple formula: Role, Context, Task, Format. R, C, T, F.

[SCREEN: Type each part as you explain. Use this running example.]

**Role.** Who should the AI act like? "Act as a career advisor." "Act as a patient tutor." That points it toward the right style and knowledge.

**Context.** What does it need to know? Who you are, who it's for, what's going on, what you've already tried. Context is the biggest difference between a generic answer and a useful one.

**Task.** What exactly do you want it to do? One clear action. Draft, summarize, compare, rewrite, list, explain.

**Format.** What should the answer look like? A short email. Five bullets. A table with three columns. Under 150 words.

[SCREEN: Show a weak prompt: "Help me prepare for my interview." Then the output: generic tips.]

Here's a weak prompt: "Help me prepare for my interview." I get generic advice I could find anywhere.

[SCREEN: Type the RCTF version. Then show the output.]

Now with the formula: "Act as an interviewer for entry-level marketing roles. I'm a college senior applying for a marketing coordinator job at a small skincare company; I have one internship doing social media. Ask me five likely interview questions, one at a time, and wait for my answer before giving feedback. Keep feedback under three sentences."

Much better. It's specific to me, it's interactive, and it's the right length.

[SCREEN: Show the "ask me questions first" trick.]

Here's a bonus trick. If you're not sure what to include, add: "Before you answer, ask me any questions you need to do this well." The AI will ask you for the missing context, and that saves you guessing.

You don't need to use all four every time. For a quick question, task and format is fine. But when the result matters, use all four.

**Good to know:** longer isn't automatically better. Clear beats long. If a detail wouldn't change the answer, leave it out.

### Worked example
**Scenario:** Maya is a new analyst who needs a summary of a 12-page report for her manager.

**Weak:** "Summarize this report."

**Formula:**
```
Role: Act as a business analyst writing for a busy manager.
Context: I'm a new analyst. My manager, who isn't a specialist in this topic, has 2 minutes to read. The report is attached [or pasted below].
Task: Summarize the main findings and any risks.
Format: 5 bullets, then one sentence starting "Recommended next step:". Avoid jargon.
```
**Point out:** each line does a different job, and it works for many other tasks.

### Prompt templates
```
Act as [role]. I'm [who you are and situation]. [Any background the AI needs.] Please [one clear task]. Format the answer as [format, length, tone]. Before you answer, ask me any questions you need to do this well.
```
Quick version:
```
[Task]. Format: [format and length]. Audience: [who will read it].
```

### Do it in 10 minutes
Take the task from Lesson 0.3 (or a new one) and rewrite the prompt using all four parts. Compare with your first attempt.

### Quiz
1. **What do the four letters stand for?** Role, Context, Task, Format.
2. **Which part usually makes the biggest difference?** Context.
3. **What's one prompt trick when you don't know what context to give?** Ask the AI to ask you questions first.

---

## Lesson 1.3: Examples, tone and not sounding robotic (6 min)

### Script

[SCREEN: You on camera, then a screenshot of an obviously AI-sounding paragraph, with words like "delve," "in today's fast-paced world," "I hope this finds you well" highlighted.]

You know when you read something and think "AI wrote this"? It's usually the same tells. Grand openings. Long sentences. Words nobody says out loud. Everything sounds like a brochure.

The fix isn't a magic prompt. It's giving the AI a sample of how you actually write, then editing.

[SCREEN: Open a doc with two or three short things you've written: a text to a friend, a discussion post, an email. Highlight them.]

Step one. Find two or three short things you've written that sound like you. An email, a discussion post, a message to a teammate. **Only use text that's yours and that you're comfortable pasting** (we'll talk more about privacy later).

[SCREEN: Paste them into the prompt.]

Step two. Ask the AI to describe your style. This is really useful: "Here are examples of my writing. Describe my style in five bullet points: sentence length, tone, vocabulary and habits."

[SCREEN: Show the description. Copy it into a note called "My voice."]

Save that description. It's your voice note.

Step three. Use it. "Write [task] using this style: [voice note]. Avoid clichés like 'I hope this email finds you well', and don't use exclamation points unless I do."

[SCREEN: Show before/after of an email.]

Look at the difference. The second one has shorter sentences, my usual phrases, and none of the fluff.

Another trick: use a "do" and "don't" list. "Do: keep sentences short, be direct, sound friendly. Don't: use buzzwords, be overly formal, exaggerate."

And one more: give an example of what good looks like. "Here's a good reply I wrote last month. Write the new one in the same style."

[SCREEN: On camera.]

Last thing, and it's important. Even with all this, read it out loud. If you wouldn't say it, change it. That's the final filter, and it's what makes the writing yours.

### Worked example
**Scenario:** Jordan wants a discussion-board post for a sociology class that doesn't sound like a robot.

Jordan's voice note (created by AI from Jordan's own writing): "Short sentences. Casual but respectful. Often starts with a direct opinion. Uses 'honestly' and 'I think.' Rarely uses exclamation points."

```
Write a 120-word discussion post for my sociology class responding to this prompt: [paste prompt]. Use my style: [voice note]. Include one example from my own experience: [1–2 sentences]. Avoid clichés and jargon. Do not invent statistics or quotes.
```
Then Jordan reads it out loud and changes two phrases.

### Prompt templates
**Step 1: extract your voice**
```
Below are three samples of my own writing. Describe my writing style in 5 bullets (sentence length, tone, vocabulary, habits, things I avoid). Be specific enough that someone could imitate it.

Sample 1: [paste]
Sample 2: [paste]
Sample 3: [paste]
```
**Step 2: use it**
```
Write [task] for [audience]. Use this style: [voice note]. Avoid: clichés, buzzwords, phrases like "I hope this email finds you well," and exclamation points. Don't invent facts. Keep it under [length].
```

### Do it in 10 minutes
1. Collect two or three short samples of your own writing.
2. Run the Step 1 prompt and save the result as "My voice."
3. Use Step 2 for a real message and read it out loud before editing.

### Quiz
1. **What's the best way to make AI writing sound like you?** Give it samples of your own writing, save a style note, and edit the result.
2. **Name one tell of robotic writing.** Any of: clichéd openings, overlong sentences, buzzwords, over-formality.
3. **What's the last check before you use the text?** Read it out loud and change anything you wouldn't say.

---

## Lesson 1.4: Fixing bad outputs (5 min)

### Script

[SCREEN: You on camera.]

Nobody gets a perfect answer on the first try. Not even people who use AI daily. The skill isn't writing a perfect prompt. It's knowing what to say next.

[SCREEN: Show a mediocre AI output, e.g., a wordy, generic paragraph.]

Here's an output I don't love. Too long, too generic. Instead of starting over, I'll follow up in the same chat, and I'll be specific about what's wrong.

[SCREEN: Type each follow-up and show the result improving. Use a list overlay of these five fixes.]

Fix one: **Shorten or expand.** "Cut this to 80 words." "Add more detail on the second point."

Fix two: **Change tone.** "Make it warmer." "More direct." "Less formal."

Fix three: **Point at the problem.** "The third sentence sounds pushy. Rewrite just that one." Precise feedback beats "make it better."

Fix four: **Add what's missing.** "You didn't mention the deadline. Add it." Or paste in the real facts it didn't have.

Fix five: **Ask for options.** "Give me three different openings." Then choose one, or combine.

[SCREEN: Show a wrong answer, e.g., a math or fact error.]

And if the answer is wrong, not just weak, say so specifically. "Check your work. The total should be the sum of the three items above. Show your steps." Sometimes it fixes itself. But don't trust the correction automatically. Verify it.

[SCREEN: Show a long chat that has gone off track. Then click "new chat" and paste a short summary.]

If a chat gets long and messy, or the AI keeps making the same mistake, start a new chat. Paste in the best version so far and the instruction. A fresh start beats fighting a confused conversation.

[SCREEN: On camera.]

Quick recipe: Look at the output. Name what's wrong. Give one specific fix. Repeat. Two or three rounds usually gets you there.

### Worked example
**Scenario:** Maya asks for a LinkedIn post announcing her internship and gets a long, cheesy result.

1. "Too long and too salesy. Cut to 60 words and remove buzzwords."
2. "Good. The line 'thrilled to embark on this journey' sounds fake. Replace it with something simple."
3. "Give me three options for the first sentence."
4. She picks one and edits by hand.

### Prompt templates (fix-it toolbox)
```
Make this shorter: about [X] words. Keep [the key points].
```
```
Change the tone to [warmer / more direct / more professional / more casual]. Keep the meaning the same.
```
```
The part that says "[quote]" isn't working because [reason]. Rewrite only that part.
```
```
You left out [missing fact]. Add it, and don't change anything else.
```
```
Give me 3 different versions of [the opening / the subject line / the closing]. Label them A, B, C.
```
```
Check your answer for mistakes. List anything you're unsure about, and show your steps.
```

### Do it in 10 minutes
Take any AI output you've generated so far and run three different fixes on it. Save the version you like best.

### Quiz
1. **Why is "make it better" a weak follow-up?** It doesn't say what's wrong or what better means.
2. **When should you start a new chat?** When the conversation is long, confused, or repeating the same mistake.
3. **If the AI corrects a factual mistake, can you trust the correction?** No. Verify it yourself.

---

## Lesson 1.5: Build your personal prompt library (3 min)

### Script

[SCREEN: You on camera.]

You've now written some prompts that worked. Don't lose them. The people who get the most out of AI aren't better at typing. They just reuse what works.

[SCREEN: Open a blank document or notes app. Type a title: "My Prompt Library."]

Create a simple document, in Notes, Google Docs, Notion, whatever you already use. Make headings for the categories you need: Email, School, Work, Job Search, Side Project.

[SCREEN: Paste in a prompt from earlier. Show the structure: title, when to use it, prompt with [brackets].]

For each prompt, save three things. A short title. When to use it. And the prompt itself, with [brackets] where the details change.

Then when you have a new task, you don't start blank. You grab the template, fill in the brackets, and go.

[SCREEN: Show the downloadable Prompt Library from the course.]

I've put over fifty ready-made prompts in the course downloads. Start there. Copy the ones that fit your life, and improve them over time. When a prompt works well, add it. When one keeps failing, fix it and save the new version.

[SCREEN: Show a "Notes" line at the bottom of a prompt: "Works best when I paste the full email."]

Add a note to yourself, like "works best when I paste the whole email." Small notes save time later.

Do this now, and you'll thank yourself in a week.

### Worked example
Show a finished library entry:

**Title:** Polite follow-up email
**Use when:** No reply after a week
**Prompt:** "Write a polite follow-up to [name] about [topic]. I sent my first message on [date]. Keep it under 70 words, friendly, and not pushy. Don't invent facts."
**Notes:** Add the original email to get a better tone match.

### Prompt template
```
Turn this prompt into a reusable template. Replace details that change with [brackets], add a one-line description of when to use it, and suggest one improvement.

Prompt: [paste the prompt that worked]
```

### Do it in 10 minutes
1. Create your library document with five category headings.
2. Save three prompts from this module as templates.
3. Copy five prompts from the course prompt library that match your week.

### Quiz
1. **What three things should each saved prompt include?** A title, when to use it, and the prompt with [brackets].
2. **Why use brackets?** They mark the details you swap out each time.
3. **How can you improve a saved prompt over time?** Add notes and update it whenever a version works better.
