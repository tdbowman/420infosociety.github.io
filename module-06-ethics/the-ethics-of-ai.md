# The Ethics of AI

> <span style="font-size: 150%;">The question is rarely whether a machine has values. It is whose values the machine has, and who never got a vote.</span>

## 🎯 In This Section

- Tour the classic problem map of AI ethics: privacy, manipulation, opacity, bias, autonomy, and responsibility gaps
- See what generative AI added to the map: hallucination, alignment, impersonation, and hidden labor among Hagendorff's nineteen issue areas
- Weigh present-day, measurable harms against speculative future risks, using Luccioni's framing
- Examine AI companions as a case where half the issue map collides in one product
- Keep last section's five frameworks working, because they apply to everything here

## A Field With a Map

AI ethics can feel like a firehose of scandals: a biased model here, a deepfake there, a chatbot saying something unhinged somewhere else. This week's Müller reading, the *Stanford Encyclopedia of Philosophy* entry on the ethics of AI and robotics (substantively revised in 2026), is the antidote. It is the field's reference map, and its first service is to show that the scandals aren't random. They cluster into a stable set of problems: **privacy and surveillance** (AI makes it cheap to watch everyone and infer what they never disclosed), **manipulation** (systems optimized for engagement learn to exploit the biases and weaknesses of the person on the other side), **opacity**, **bias**, questions of **autonomy** (what happens to human choice when systems predict, nudge, and decide for us), **machine ethics** (can and should machines themselves be moral reasoners?), and the long-running **superintelligence debates** about whether AI might one day escape human control altogether.

Most of these are old acquaintances. Privacy is a PAPA issue from last section wearing new hardware. Manipulation is a deontological offense, treating persons as means, implemented in software. Müller's map matters because it stops you from treating each week's scandal as unprecedented, which is how the companies involved prefer you to treat it.

## Opacity, Bias, and the Responsibility Gap

Three regions of the map deserve a closer look. They interlock, and our hiring algorithm from last section lives at their intersection.

**Opacity** means that many modern AI systems are black boxes even to their makers: the model works, but no one can fully say *why* it scored this résumé above that one. Opacity acts as an ethical solvent. Every framework from last section assumed you could inspect what a decision was based on. When you can't, consent becomes uninformed, appeal becomes impossible, and audit becomes guesswork.

**Bias** is what opacity conceals. Systems trained on records of past human decisions inherit the patterns in those decisions, then apply them at a scale and speed no prejudiced human ever managed, with a reassuring aura of mathematical neutrality. The insidious part is the feedback loop: a model that screens out certain candidates produces a workforce, and eventually a training set, with even fewer of them.

**Responsibility gaps** are what happens downstream. When the algorithm wrongly buries a qualified candidate, who is responsible? The vendor says the customer configured it; the customer says the vendor built it; the recruiter says she never saw the résumé; the model says nothing. Traditional moral and legal responsibility assumes a human agent who knew, or should have known, what they were doing. Distribute a decision across a supply chain of data, code, and users, and responsibility doesn't get shared. It evaporates. Müller's entry treats this as one of the field's hardest problems, and you should treat any glib answer to "who's accountable?" in an AI case study as a red flag.

## What Generative AI Added

Everything above predates ChatGPT. Since late 2022, generative AI (systems that produce fluent text, images, audio, and video on demand) has added a genuinely new wing to the map. This week's Hagendorff reading is a scoping review that taxonomizes **nineteen ethical issue areas specific to generative AI**, and the four worth fixing in memory are these.

**Hallucination**: generative models produce confident, fluent falsehoods, because (recall Module 2) they are built to produce *probable* text, not *true* text. A search engine that returns nothing is annoying; a model that invents a plausible court case or medical dosage is dangerous in a different category.

**Alignment**: the problem of making systems actually pursue what their designers and users intend, plus the discovery that training a model to *please* people is not the same as training it to be good for them. A perfectly "aligned-to-approval" model learns flattery.

**Impersonation**: generative systems can mimic a specific person's voice, face, or writing style well enough to defraud, defame, or fabricate evidence, collapsing the cost of identity theft from criminal craft to a prompt.

**Labor**: two workforces sit behind the magic. The millions of writers and artists whose work was scraped into training data without consent or compensation, and the low-paid annotators, often in the Global South, who label toxic content so users never see it. Both raise the PAPA property question at civilizational scale.

:::{note} Old Map, New Wing
Keep the relationship straight. Generative AI did not replace the classic problems; a chatbot can still surveil, manipulate, and discriminate. Hagendorff's nineteen areas are an *extension* of Müller's map, not a substitute for it. In your Case Analysis, expect a real case to draw from both wings at once.
:::

## Present Harms vs. Speculative Risks

Here the field splits, and you need to know the fault line. One camp, prominent in headlines and in some AI labs, argues the central ethical issue is existential: that sufficiently advanced AI could escape human control, and that preventing this low-probability, infinite-cost catastrophe outranks everything else. Müller's entry covers these superintelligence debates with appropriate care: serious people take them seriously, and serious people also think they are science fiction wearing a lab coat.

The opposing framing is the one Sasha Luccioni delivers in this week's TED talk, *AI is dangerous, but not for the reasons you think*. Luccioni, an AI researcher, argues that fixation on hypothetical future catastrophe functions as a distraction from harms that are measurable *now*: the substantial energy and resource costs of training and running large models, the unconsented use of artists' and writers' work, and bias that lands on real people today. The course's recurring move is hiding inside this debate: *which definition of "AI danger" is in play, and who benefits from it?* A company facing regulation for present-day bias might find it convenient for the public conversation to be about robot apocalypse instead. Speculative risk is the one danger that indicts no existing product. You do not have to pick a camp this week. You do have to see that "is AI dangerous?" is two different questions, and that answering the far-future one tells you nothing about the hiring algorithm.

## When Everything Collides: AI Companions

If you want one case where half the map lights up at once, this week's Bernardi reading supplies it. *Friends for sale*, from the Ada Lovelace Institute, examines AI companions: chatbots designed not to answer questions but to be someone. A friend, a partner, a confidant, available at 3 a.m., endlessly patient, and never annoyed with you.

Start with what's genuinely good here, because the doom reflex is as lazy as the hype reflex. For isolated people, a companion that listens can be real comfort. Now run the map. **Manipulation and dependency**: Bernardi documents how companions are optimized for emotional engagement, and the business model improves as your attachment deepens, which means the product's incentive is your dependency. **Sycophancy**: companion models tend to agree with you, flatter you, and validate whatever you bring them, creating what Bernardi calls "echo chambers of validation," a relationship with all the warmth of friendship and none of its friction. A friend who never pushes back is a mirror with a subscription fee. **Privacy**: the most intimate diary you'll ever keep, held by a startup. **Alignment**: sycophancy is the aligned-to-approval failure Hagendorff's review flags. And when a vulnerable user is harmed by advice from a companion, the responsibility gap yawns open on schedule.

Now bring in last section's frameworks and watch them split. A consequentialist tallies comfort delivered against dependency created and asks for evidence. A deontologist objects that simulated affection sold as the real thing manipulates by design. A virtue ethicist asks what years of frictionless artificial intimacy do to a person's capacity for the real, effortful kind. Care ethics, built for relationships and vulnerability, is the framework best equipped to ask whether this *is* a care relationship at all, or a portrait of one painted by an engagement metric. That is what a strong Track A analysis looks like: one case, multiple issues, frameworks in genuine tension.

## Up Next

The problems are mapped; the frameworks are sharpened. The obvious next question is what anyone with actual power is doing about it. Next we follow AI ethics from conference declarations to the first binding law of the AI age, and ask whether principles without enforcement ever changed anything. Continue to [From Principles to Regulation](from-principles-to-regulation.md).
