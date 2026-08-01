# Promise and Peril

> Every tool is a weapon if you hold it right.

## 🎯 In This Section

- Understand dual-use: why AI's benefits and harms come from the same capabilities, not different ones
- Follow Brundage and colleagues' 2018 forecast of how AI expands, cheapens, and sharpens attacks
- See the three security domains — digital, physical, political — where machine misuse plays out
- Examine the Pew data on the optimism gap between AI experts and the American public
- Apply Module 1's "who benefits from the story?" move to both hype and doom

## The Same Machine, Twice

Consider a model that reads medical images and flags early-stage tumors more consistently than a tired radiologist at hour eleven of a shift. Now consider a model that reads your public social media posts and drafts a message perfectly tuned to make you click a malicious link. Here is the uncomfortable part: these are not different technologies. Pattern recognition, language generation, prediction, optimization — the capabilities are identical. Only the objective changed.

This is the **dual-use** problem, and it is the central concept of this section. Nuclear physics gave us reactors and bombs; biology gives us vaccines and bioweapons; AI belongs on the same list. You cannot build the beneficial version without, in large part, building the harmful one, because they are the same machine pointed in different directions. That means "should we build it?" is rarely the live question. The live questions are the messier ones: who gets access, under what conditions, with what safeguards, and who is accountable when the pointing goes wrong.

## A Forecast Worth Grading

In 2018 — four years before ChatGPT — a team of twenty-six researchers from Oxford, Cambridge, OpenAI, and elsewhere published *The Malicious Use of Artificial Intelligence*, this week's Brundage reading. Rather than vague warnings, they made a structured forecast: as AI systems became more capable and more accessible, malicious use would change in three specific ways.

First, **expansion**: attacks that once required scarce human expertise could be performed by software, so more actors could carry out more attacks against more targets. Second, **cheapening**: the labor-intensive parts of an attack — writing the persuasive email, casing the target, producing the fake persona — could be automated, collapsing the cost per victim. Third, **targeting**: attacks could become simultaneously mass-scale *and* personalized, a combination that used to be impossible. Spear phishing — the hand-crafted con aimed at one specific person — was the canonical example. Historically, an attacker chose between cheap-but-generic spam and expensive-but-effective personal deception. Language-generating AI, Brundage and colleagues predicted, would erase that trade-off.

The report organized the threat landscape into three domains, all of which have since moved from forecast to news cycle:

| Domain | What's threatened | Illustrative misuse |
|---|---|---|
| Digital security | Networks, accounts, data | Automated spear phishing; AI-assisted discovery of software vulnerabilities |
| Physical security | Bodies, infrastructure | Repurposed autonomous systems, such as commercial drones turned into weapons |
| Political security | Public opinion, elections, trust | Tailored propaganda, impersonation, and synthetic media at scale |

Reading Chapters 1–2 in 2026 is an exercise in grading a prediction, and the authors score uncomfortably well — when we reach Module 5, you'll read a 2025 report documenting an AI-orchestrated cyber espionage campaign that reads like their forecast come to life. But notice, too, what the report is *not*. It is not a doom tract: the authors are AI researchers who built these systems because of their benefits, and their recommendations are about governance — rethinking how research is published, learning from how cybersecurity handles disclosure — not abandonment. Dual-use framing cuts both ways: anyone who tells you only the promise, or only the peril, is showing you half the machine.

:::{note} Dual-Use Is Not an Excuse
"Technology is neutral; only uses are good or bad" sounds like the lesson here, but Brundage and colleagues argue nearly the opposite. Because misuse is *foreseeable*, design choices — what to release, to whom, with what safeguards — are moral choices made in advance. A capability released with no guardrails was not neutrally released; someone decided the risk was acceptable, usually on other people's behalf. When you meet an AI product this week, ask what misuse its makers foresaw, and what they did about it.
:::

## The Optimism Gap

So how do people feel about living inside this dual-use experiment? In 2025, the Pew Research Center did something unusual: it surveyed both the general American public and a sample of AI experts, asking the same questions of each. The result, documented in this week's Pew reading, is a portrait of two groups looking at the same technology and seeing different futures.

The experts, on the whole, lean optimistic: far more of them than of the public expect AI to make things better over the coming decades, to benefit them personally, and to improve how people do their jobs. The public leans worried: more concerned than excited, less confident of personal benefit, and more focused on harms like job loss and the erosion of human connection. And on some points the two groups agree in a telling way — notably, majorities of *both* want more control over how AI is used in their lives, and neither group expresses much confidence that government or industry will regulate it well. The gap is not uniform, either: within the expert camp, Pew finds women consistently less optimistic than men, a reminder that "the experts" are not a monolith and that who gets counted as an expert shapes what "expert opinion" says.

## Who Benefits from the Story?

What should you make of the gap? Resist the two lazy readings. The first says the public is simply uninformed — if ordinary people understood AI, they'd relax. The second says the experts are simply captured — they're paid to be optimistic. Each reading conveniently flatters the person making it.

Module 1 gave you a better tool: ask which definition is doing the work, and who benefits from the story. Experts and the public may not even be evaluating the same object. An expert asked about "AI" may picture the technology's trajectory — benchmark scores climbing, drug discovery accelerating. A member of the public may picture their own exposure to it — a chatbot blocking the way to a human customer service agent, a manager musing about headcount, a feed filling with synthetic sludge. Optimism about the *technology* and worry about *one's position in the deployment* can both be accurate, because deployment decides who captures the promise and who absorbs the peril — and the public knows perfectly well who usually absorbs it.

Notice, too, that stories about AI are themselves dual-use. "AI will transform everything" raises venture capital and justifies moving fast; "AI is terrifyingly powerful" can, oddly, do the same work, marketing the product while positioning its makers as the only ones qualified to govern it; "the public just doesn't understand" converts a political question — who decides how this is deployed? — into a PR problem. None of this tells you the claims are false. It tells you to check who is speaking, what they are selling, and what the evidence says — which is why this module pairs the forecasts with survey data and experiments rather than keynote speeches.

## Up Next

Expansion, cheapening, targeting, and the optimism gap all play out at the scale of societies. But AI is also operating at a much more intimate scale — inside your text threads, your group chats, your creative writing. In [AI and Human Connection](ai-and-human-connection.md), we look at what the evidence says happens when the machine joins the conversation.
