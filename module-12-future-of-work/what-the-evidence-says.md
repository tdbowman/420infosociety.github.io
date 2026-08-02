# What the Evidence Says

> We are being afflicted with a new disease of which some readers may not yet have heard the name, but of which they will hear a great deal in the years to come: namely, technological unemployment.
> - John Maynard Keynes, 1930

## 🎯 In This Section

- Meet the four best pieces of evidence we currently have about AI and employment, and what each can and cannot tell you
- Understand why Brynjolfsson and colleagues chose "canaries in the coal mine" as their metaphor, and why its precision matters
- See the global picture: who is exposed to generative AI, and why exposure is not elimination
- Learn what real usage logs reveal about automation versus augmentation, and what people actually hand off to AI
- Practice holding "entry-level effects are real" and "there is no mass unemployment" in your head at the same time

## A Debate Older Than the Computer

Keynes wrote that sentence in 1930, before the transistor, before the computer, almost a century before ChatGPT. Every major technology since has triggered the same argument on schedule: this time the machines will take the jobs. And every previous round eventually cooled, because economies kept generating new work even as old work disappeared. That track record is why economists greet each new panic with raised eyebrows.

But "it never happened before" is a probability, not a law. And this round has something the previous rounds did not: unusually good data, available unusually fast. We don't have to argue from anecdotes about a cousin's laid-off coworker or a CEO's confident keynote. We have payroll records, global occupational surveys, and, for the first time in this debate's long history, logs of what people actually ask the technology to do. This section lays out four rulers. None settles the debate. Together, they tell you what an honest position has to account for.

## The Canaries: Entry-Level Effects Are Real

The most important single piece of evidence this week comes from Erik Brynjolfsson, Bharat Chandar, and Ruyu Chen at the Stanford Digital Economy Lab. Their 2025 paper is built, deliberately, as six facts rather than one grand claim, a structure worth noticing because it models how to argue carefully about a noisy question.

The headline fact: analyzing payroll data, they find a roughly 13 percent relative decline in employment for early-career workers in the occupations most exposed to AI, while overall employment kept growing. Read that sentence again slowly, because both halves matter. Entry-level hiring in exposed fields really did fall relative to comparable groups. And the labor market as a whole really did keep adding jobs. Anyone who quotes you one half without the other is selling something.

The title metaphor is chosen with the same care. Canaries in coal mines were an early-warning system: small, sensitive creatures that reacted to danger before the miners could feel it. Entry-level workers in exposed occupations play the same role here. They are the most sensitive point in the labor market, because the tasks that make up a first job (drafting, summarizing, routine analysis, boilerplate code) overlap heavily with what current AI does well, and because firms adjust hiring long before they resort to layoffs. A distressed canary told miners something real was in the air. It did not tell them the mine was collapsing. Both the signal and its limits are built into the metaphor, and the authors put the question mark in their title on purpose.

:::{warning} What the Canaries Don't Prove
It is tempting to extrapolate: if entry-level hiring in exposed occupations is down now, surely everyone's job is next. Resist the reflex. The same data shows overall employment growing, and a relative decline among the least-experienced workers in the most-exposed occupations is also the pattern you'd expect from firms cautiously experimenting. The canary metaphor claims *early warning*, not *proof of collapse*. Your debate brief should be equally precise.
:::

## The Map: Who Is Exposed, Worldwide

The Stanford data is rich but national. For the global picture, this week's International Labour Organization update is the standard reference. Its central estimate: about one in four workers worldwide are in occupations with some degree of generative-AI exposure. "Exposure" is a measurement term worth defining carefully. It means an occupation contains tasks that current generative AI could plausibly perform, not that the occupation is about to vanish. On that point the ILO is blunt: for most exposed occupations, the likely outcome is transformation (some tasks change hands, the job gets redefined) rather than elimination.

Two patterns in the map turn a technology story into a fairness story. First, exposure skews strongly by gender, largely because clerical and administrative work, historically dominated by women in much of the world, sits close to the center of what generative AI does well. Second, exposure is graded by country income level: richer countries, with more employment in information-handling occupations, have more exposed workers. The same technology, released everywhere at once, lands on a labor market that was never level to begin with. Remember those gradients when you reach the "it's about power and distribution" position in the last section. This is its best evidence.

## The Usage Logs: What People Actually Delegate

Exposure studies ask what AI *could* do. The Anthropic Economic Index asks what people actually *use* it for, drawing on real usage data to map which occupational tasks people delegate to a model. This is a genuinely new kind of evidence in a very old debate, and it complicates both the doom story and the hype story.

The report distinguishes two modes of use. In **automation**-style usage, the model performs the task in the person's place: the user hands over a job and takes back a finished product. In **augmentation**-style usage, the model works *with* the person, iterating, critiquing, explaining, drafting material the human then reshapes. Both patterns show up at scale, split rather than dominated by either. The same underlying capability flows into both modes, and that is the point worth holding onto: nothing in the technology dictates which one you get. That's a choice made in deployment, by employers, by product designers, by the person typing the prompt.

The Index also documents how uneven adoption is, across countries and across enterprises. Whatever the future of work turns out to be, it is not arriving everywhere at once; it is pooling in some places and occupations while barely touching others. Averages will mislead you.

:::{figure} images/augmentation-automation.svg
:name: augmentation-automation
:alt: A diagram showing a single box labeled the same AI capability at the top, with two arrows leading down to two contrasting panels, the left panel labeled automation and described as the task is done instead of you with examples such as routine support replies sent without human review, standard translations published as-is, and forms processed end to end, and the right panel labeled augmentation and described as the task is done with you with examples such as a nurse drafting chart summaries and verifying each one, a programmer iterating on model-drafted code, and an analyst asking the model for counterarguments, above a footer note stating that which mode you get is a deployment choice made by people and organizations, not a property of the technology.
:width: 100%

One capability, two modes. The same AI system can replace a task or reshape it, and the Anthropic Economic Index finds real usage split between the two. The difference lies in how people and organizations deploy it, not in the model.
:::

## Holding Two Truths at Once

Now add the fourth ruler, which you've already met. Back in Module 4, the Yale Budget Lab examined broad labor-market indicators and found no detectable economy-wide disruption from AI. The aggregate statistics look, so far, stubbornly normal. Set all four findings side by side and notice that they do not contradict each other, even though the headlines built from them do.

| Source | What it measures | What it found | What it can't tell you |
|---|---|---|---|
| Brynjolfsson, Chandar, & Chen (2025) | Payroll records, by occupation and career stage | Early-career employment down ~13% (relative) in the most AI-exposed occupations; overall employment still growing | Whether the canaries stay canaries, or the effect spreads |
| ILO (2025) | Global occupational exposure | About 1 in 4 workers in occupations with some generative-AI exposure; skewed by gender and country income; transformation more common than elimination | What happens inside "transformed" jobs |
| Anthropic Economic Index (2025) | Real AI usage: tasks people delegate | Usage split between automation-style and augmentation-style; adoption uneven across countries and enterprises | What non-users do |
| Yale Budget Lab (Module 4) | Economy-wide labor statistics | No detectable aggregate disruption so far | Whether "so far" is reassurance or lag |

This is the discipline the rest of the module depends on: entry-level effects in exposed occupations are real, *and* there is no mass unemployment. A quarter of the world's workers are exposed, *and* exposure mostly means transformation. People genuinely automate tasks away, *and* they genuinely collaborate with the machine. If someone's account of the future of work requires you to drop one of these findings, you are hearing a sales pitch rather than a forecast. The question the next section takes up is what a person entering this labor market should actually do about it.

## Up Next

The evidence says the ground is shifting under entry-level work in particular, which is exactly where you're standing. In [Skills and Adaptation](skills-and-adaptation.md), we turn from measurement to strategy: upskilling, reskilling, and the human skills that machines make more valuable rather than less.
