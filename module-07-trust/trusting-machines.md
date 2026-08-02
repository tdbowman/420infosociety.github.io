# Trusting Machines

> <span style="font-size: 150%;">We forgive our friends a hundred errors and our software none, until it starts talking, and then we forgive it everything.</span>

## 🎯 In This Section

- See what changes in the mechanics of trust when the trustee is a machine instead of a person
- Learn Glikson and Woolley's distinction between cognitive and emotional trust in AI, and what shapes each
- Understand the calibration problem: why over-trust and under-trust are both dangerous, and why the goal is neither more nor less trust but *better-fitted* trust
- Map Afroogh and colleagues' taxonomy of trust-makers and trust-breakers, technical and ethical
- Situate your own attitudes in the global picture: who trusts AI, who uses it anyway, and where the gap yawns widest

## The Driver Who Obeyed the Map

Every so often a news story surfaces about a driver who followed GPS directions into a lake, a cornfield, or a staircase. We laugh, a little nervously, because we recognize the impulse: the machine sounded so sure. Meanwhile, in hospitals, the opposite failure plays out with no comedy at all. Clinicians and patients sometimes discount an algorithmic recommendation that was, in fact, correct, because it came from a machine. Between the driver in the lake and the discarded diagnosis lies the whole problem of this section: humans are not naturally good at deciding how much to trust machines, and both directions of error have victims.

Run last section's framework on a machine trustee and you can see why the machinery grinds. Ability? Often superhuman in a narrow band and absurdly brittle outside it, with no reliable way for you to tell where the band ends. Motivation and benevolence? A machine has no wants at all. Behind it stand the motivations of the company that built and deployed it, which is who you are actually trusting. Embeddedness? Partial at best: a chatbot suffers no shame, faces no gossip among its peers, and until recently operated with thin institutional oversight. So the trust-warranting properties are strange or missing, while the *signals* are lavish. Fluent language, confident tone, instant answers: in the human world these are symptoms of competence and care. From a machine, they are symptoms of nothing but statistical mastery of how competence and care *sound*. That mismatch between rich signals and uncertain properties is the defining hazard of trusting machines.

## Two Kinds of Trust, One Confused Human

This week's Glikson and Woolley reading, a sweeping review of two decades of empirical research on human trust in AI, gives us the sharpest available lens. Trust in machines, they show, runs on two distinguishable tracks.

*Cognitive trust* is the head's track: a judgment of competence and reliability. Does it work? How often does it fail, and how badly? Performance and transparency build it, and visible errors demolish it fast. *Emotional trust* is the gut's track: an affective sense of comfort, safety, even attachment, largely indifferent to performance statistics. Glikson and Woolley find it is fed by different inputs entirely: *tangibility* (a physical robot you can see and touch feels different from an invisible algorithm), *anthropomorphism* (a name, a voice, a face, an "I"), and the sheer social warmth of an interaction.

| | Cognitive trust | Emotional trust |
|---|---|---|
| Rooted in | Judged competence and reliability | Affective comfort and attachment |
| Built by | Accurate performance, transparency, track record | Human-likeness, voice, warmth, tangibility |
| Damaged by | Visible errors, opacity, inconsistency | Creepiness, betrayal of the relationship's feel |
| Characteristic failure | Misjudging what the system can actually do | Bonding with a system regardless of what it can do |

The two tracks matter because modern conversational AI pulls them apart. A chatbot's warmth cranks the emotional track to levels no spreadsheet ever reached, while the cognitive question (*what is this system actually reliable at?*) gets harder to answer, not easier, as the fluency improves. Anthropomorphism, in Riegelsberger's vocabulary, is a symbol wearing a symptom's clothing: warmth that is evidence of nothing.

## Calibration: The Only Goal Worth Having

It is tempting to conclude that we should simply trust AI less. That conclusion is about half right. The research consensus Glikson and Woolley synthesize points somewhere subtler: the goal is *calibrated* trust, trust proportioned to actual trustworthiness, task by task. Over-trust produces automation complacency: the driver in the lake, the lawyer filing a brief full of cases the chatbot invented, the student repeating a confident hallucination. Under-trust produces disuse, with the accurate screening tool ignored and the correct warning dismissed. A society can lose to both errors at once, in different corners.

Afroogh and colleagues' 2024 systematic review, another of this week's readings, is effectively a parts catalog for calibration. They comb hundreds of studies and sort what they call *trust-makers* and *trust-breakers* into technical and ethical families. On the technical side, trust is made by reliability, transparency, explainability, and robustness, and broken by errors, opacity, and fragility under unusual conditions. On the ethical side, trust is made by fairness, accountability, and respect for privacy, and broken by bias, surveillance, and the sense that no one answers when the system harms you. That is Riegelsberger's two families again. The technical factors are ability signals; the ethical factors are motivation and embeddedness signals. People, it turns out, ask machines the same two ancient questions they ask strangers: *can you do this?* and *whose side are you on?*

:::{tip} Calibrate Like a Professional
Pilots are trained to treat automation with a specific discipline: know what the system is certified to do, monitor it inside that envelope, and take over outside it. You can run a civilian version. For each AI tool you use, write one sentence: "I trust this system to ____, and I verify anything involving ____." If you can't fill in the blanks, your trust isn't calibrated. It's just a mood.
:::

## Aversion, Appreciation, and the Global Ledger

When do people lean each way? The optional Qin and colleagues meta-analysis pulls together years of contradictory findings on "algorithm aversion" and "algorithm appreciation" into a usable rule: people prefer the algorithm when it seems more capable than the human alternative *and* the task doesn't feel like it requires personalization, and they swing toward humans when the task feels subjective, personal, or about *them* in particular. We accept the machine's route to the airport and bristle at its verdict on our essay, even when its judgment is demonstrably better. Perceived capability and perceived need for a human touch, not actual accuracy, do the deciding. Sit with that one, because it means our aversion and our appreciation can both be misplaced.

Zoom out to the widest available frame and the picture gets stranger. The Gillespie team's 2025 global study, which surveyed more than 48,000 people across 47 countries between November 2024 and January 2025, finds widespread use of AI running alongside deeply ambivalent trust. Most people use these systems regularly while remaining wary of them, a combination you might call *reliance without confidence*. The trust is also unevenly distributed in a direction that surprises many students: respondents in emerging economies report substantially more trust in AI than those in advanced economies, where skepticism runs highest even as usage climbs. Whatever trust in AI is, it is not a simple function of exposure or development. It is entangled with what people expect technology to do for them, and with how much they trust the institutions deploying it.

Hold that last thread. Trust in machines never floats free; it borrows from, and lends to, trust in the companies, governments, and institutions behind them. What happens when *that* trust is the thing collapsing?

## Up Next

We have been assuming the old trust infrastructure of institutions, professions, and verification still stands behind the machines. But the same decade that made AI conversational has watched trust in institutions sag, while emotional bonds with machines deepen. That squeeze is the story of the final section. Continue to [Trust in Crisis](trust-in-crisis.md).
