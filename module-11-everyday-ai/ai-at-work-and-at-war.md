# AI at Work and at War

> Automation never removes humans from the loop. It decides which loop the humans are left holding.

## 🎯 In This Section

- Learn what the "psychological contract" is and how Braganza and colleagues found AI adoption can quietly break it
- See how algorithmic management turns the adviser-and-agent pattern from Section 1 into a boss
- Follow AI into military cybersecurity, where an Air Force official describes nearly 2.5 million alerts a day and AI as triage for human attention
- Name the pattern that repeats across both worlds — machines handle volume, humans handle judgment — and ask why the line between them keeps moving
- Check the mood of the country: what Pew's survey says Americans actually feel about AI in work and daily life

## The Contract Nobody Signed

Every job comes with two contracts. One is written: salary, hours, duties. The other is not written anywhere, and it matters more. It is the web of unspoken mutual expectations between you and your employer — that effort will be noticed, that loyalty runs both ways, that you will be told the truth about changes that affect you, that doing good work makes your position more secure, not less. Organizational researchers call this the **psychological contract**, and its defining feature is that you only see it clearly when it breaks.

This week's Braganza reading asks what happens to that invisible contract when employers adopt AI. Studying workers in AI-adopting organizations, Braganza and colleagues found that AI adoption can erode the psychological contract — and that as the contract frays, job engagement and trust decline with it. Notice what this finding is *not*. It is not "AI takes jobs." The workers in question were still employed. The damage was quieter: when systems start doing, evaluating, or reorganizing parts of your work without the old human negotiation, the felt promise of the workplace changes. Why invest discretionary effort — the extra care that was always voluntary — in an institution that seems to be optimizing you like a resource? The study's framing in terms of "productive employment and decent work" (language borrowed from global development goals) makes the stakes plain: a workplace can keep every job and still lose its workforce's trust.

This should sound familiar. It is Section 1's delegation story with the roles reversed. At home, you delegate to the AI. At work, increasingly, your *employer* delegates to the AI — and one of the things being delegated is the management of you.

## Managed by the Algorithm

The clearest version of that reversal is **algorithmic management**: the use of software to do things supervisors used to do — assign shifts, route tasks, set pace targets, monitor performance, and sometimes trigger discipline. If you have ever driven for a rideshare app, delivered food, or worked a warehouse shift scheduled by demand-forecasting software, you have been algorithmically managed. The adviser-and-agent spectrum from Section 1 applies here too, except you are not the one doing the delegating: the app recommends, nudges, scores, and eventually decides, and the human manager recedes to the role of exception handler.

Two features make algorithmic management a psychological-contract problem of exactly the kind Braganza and colleagues describe. First, opacity: a human supervisor can be asked *why*; a scoring system usually cannot, at least not by you. Second, asymmetry: the system watches you in fine grain, while you cannot see it at all. Mutual, negotiated expectations — the heart of the psychological contract — struggle to survive a relationship in which one party is measurable and the other is inscrutable.

:::{note} The recurring question, workplace edition
This course keeps asking: which definition is doing the work, and who benefits? Watch how workplace AI gets named. The same system is a "productivity tool" in the vendor's deck, a "decision support system" in the HR memo, and "the algorithm that cut my hours" in the break room. Each name assigns the technology a different place on the delegation spectrum — and quietly assigns the accountability somewhere different, too.
:::

## Triage at Machine Scale

Now raise the stakes. Leave the warehouse and walk into a military cybersecurity operations center — because the same delegation logic is at work there, under far more pressure.

Welch's short news piece in *Breaking Defense* reports a striking figure: an Air Force cyber official said the Department of the Air Force faces nearly 2.5 million cybersecurity alerts *per day*, and that AI could help sort through them. Sit with the number for a moment. No workforce of any size reads 2.5 million of anything a day. Most of those alerts are false alarms or duplicates; a tiny fraction are the early footprints of a real intrusion. The job is finding the fraction — and the finding has to happen fast, every day, forever.

Here the scarce resource is not information. It is the oldest information-society theme in this book, and by now you can name it on sight: **attention**. Machine-generated telemetry has outrun human reading capacity so completely that the only realistic role for people is at the top of a filtered funnel. AI becomes a *triage* layer — the emergency-room nurse who decides which cases reach the doctor. The machines read everything and escalate a little; the humans judge the little that gets escalated.

It is worth pausing on why this is one of the more defensible uses of AI you will meet in this course. Nobody's judgment is being replaced — no human judgment was ever going to touch 2.5 million alerts. The AI is not making the call on what an attack means or how to respond; it is deciding what deserves a human's eyes. If delegation has a best case, "machine reads the haystack, human examines the needles" is a strong candidate.

## Volume for Machines, Judgment for Humans — Until the Line Moves

Put the workplace and the ops center side by side and a single pattern emerges. Institutions adopt AI where volume overwhelms people: alerts, applications, résumés, claims, transactions, tickets. The comforting formula — repeated in nearly every corporate and government AI strategy — is that machines will handle the volume while humans keep the judgment.

The formula is true, and unstable, at the same time. Three quiet forces keep moving the line:

| Force | How it moves the line | Everyday sign |
|---|---|---|
| Economics | Human review is the most expensive stage, so there is constant pressure to trust the filter a little more | "Auto-approve low-risk cases" becomes "auto-approve most cases" |
| Deference | People rubber-stamp systems that are usually right; the human-in-the-loop becomes a human-on-the-loop, then a signature | Reviewers approving at a pace that makes real review impossible |
| Pipeline erosion | Judgment is trained on the routine cases the machine now absorbs — so tomorrow's senior expert loses the apprenticeship that made today's | Fewer junior analyst and paralegal roles doing "the boring work" |

The third force is the sleeper. Triage work — reading ordinary alerts, screening ordinary résumés — was never just labor. It was how novices became the experts who could handle the escalations. Automate the bottom of the ladder, and you have to ask where the top of the ladder will come from. This is Section 1's *skill atrophy* operating at the scale of professions rather than persons, and it connects straight back to Braganza: a workplace that automates the apprenticeship has rewritten the psychological contract for an entire career path, not just a job.

## What the Public Thinks

If this section's pattern has left you ambivalent — impressed by the triage, uneasy about the moving line — you are, statistically speaking, a typical American. The Pew Research Center's 2025 survey of how Americans view AI and its impact on people and society finds concern outrunning excitement overall. The worry is not abstract robot-apocalypse fear; it clusters around exactly the everyday territory of this module — what AI will do to people's relationships, their work, and human creativity, and whether individuals will have any say in the matter.

That last clause deserves emphasis. Running beneath the survey responses is a felt absence of control: AI arriving in workplaces and daily life as something done *to* people rather than chosen *by* them — the pre-checked checkbox from Section 1, scaled up to a society. Which raises the obvious next question: who, if anyone, is steering?

:::{seealso} Two loops, one lesson
Compare the warehouse worker and the Air Force analyst. Both now work downstream of an AI filter. The difference is where judgment lives: the analyst sits *above* the filter, judging what it escalates; the worker often sits *below* it, being judged. When you evaluate any workplace AI system — including ones you will someday be offered — the first question is not "how accurate is it?" but "which side of the filter do the humans sit on?"
:::

## Up Next

Someone is, at least, trying to steer. In [Governing Everyday AI](governing-everyday-ai.md), we compare the current administration's AI Action Plan with its predecessor's approach, ask what an ordinary user can actually influence, and build the most practical skill this module offers: knowing when *not* to delegate.
