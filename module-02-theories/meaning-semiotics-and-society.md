# Meaning, Semiotics, and Society

> A signal arrives the moment it is received. Information arrives only when someone makes sense of it.

## 🎯 In This Section

- Meet the counter-tradition: theories that refuse to separate information from meaning
- Distinguish semantic, semiotic, and social/domain approaches to information
- Use Tredinnick's survey as a map of the theoretical landscape
- Apply Hjørland's "levels of disagreement" to understand why the field argues — and why that's healthy
- See why your choice of theory quietly decides how search engines rank, moderators moderate, and AI companies build

## The Message That Arrived Empty

In 1799, French soldiers in Egypt dug up a slab of granodiorite covered in three bands of writing. As a Shannon-style signal, the Rosetta Stone was in decent shape: the inscriptions were physically present, the "channel" of two thousand years had added noise (a broken corner, worn characters) but most of the marks survived. Yet for the Egyptian hieroglyphic portion, no information arrived at its European destination for more than two decades — because nobody could read it. The signal was there. The meaning was not. Only when scholars finally cracked the script did the same unchanged marks suddenly deliver a flood of information about a vanished civilization.

Every theory you'll meet in this section starts from some version of that puzzle. If information can sit inert in a perfectly preserved signal, then information can't simply *be* the signal. Something else — truth, interpretation, a community that knows how to read — must be part of the story. Shannon deliberately bracketed that something. The counter-tradition is the seventy-five-year project of unbracketing it.

## Putting Truth Back In: Semantic Information

The first move is the philosopher's move: information isn't just structured signal, it's *meaningful* structured signal — and, in the strongest version, it has to be true. This is the position Tredinnick's survey associates most prominently with Luciano Floridi, whose account of semantic information requires well-formed, meaningful data that is also truthful. On this view, a false statement isn't "bad information" — it fails to be information at all, the way a forged banknote isn't unusual money but simply not money.

You can feel the pull of this. When you say a witness "provided information" to investigators, you mean something stronger than "emitted decodable signals." But notice the cost. If information must be true, then measuring how much of it flows through a network becomes philosophically fraught — is a fiber optic cable carrying less information when it streams a conspiracy documentary than when it streams a physics lecture? The semantic theorist says, in an important sense, yes. The engineer stares in disbelief. Both are using the same word, calibrated to different jobs. Keep this trade-off in mind; it returns with practical teeth at the end of this section.

## Signs Need Readers: The Semiotic Turn

The second move goes further: even meaning-plus-truth isn't enough, because meaning doesn't float free — it happens *to someone*. Semiotics, the study of signs, insists that a sign involves three things, not two: the mark or sound itself, the thing it points to, and an interpreter for whom the pointing works. Smoke means fire only to a creature that has learned the connection. A red octagon means *stop* only inside a community trained in traffic conventions.

On the semiotic view, Shannon's diagram is missing its most important box: the one where interpretation happens. Information is not delivered like a package; it is *achieved*, every time, by an interpreter applying learned codes — and different interpreters, with different histories, can achieve different information from the identical signal. This week's optional Brier chapter (PDF on Canvas) pushes this line furthest, arguing in his "cybersemiotic" framework that no purely statistical theory can ever account for how living, feeling, culturally embedded beings make signs mean. Tredinnick treats the semiotic tradition as one of the major poles of the field for good reason: it explains everything Shannon's model handles as a special case — the case where sender and receiver already share so much convention that interpretation looks automatic.

## Information Lives in Communities: The Social and Domain View

The third move is the information scientist's move, and it's the one this course leans on most. Ask: where do those shared codes and conventions come from? Answer: from communities. A radiologist looking at a chest X-ray sees pneumonia; you see gray clouds. The image is identical — the *information* differs because the radiologist belongs to a domain with training, vocabularies, journals, and standards that make certain differences visible and important.

This is Birger Hjørland's territory. In this week's reading, Hjørland argues that information science's core concepts can't be settled by picking better definitions, because the field's disagreements operate at several distinct levels at once. Roughly:

| Level | What's being disputed | Example |
|---|---|---|
| Terminology | Which words we use for which concepts | Is it "information seeking" or "information behavior"? |
| Theory | Which claims about the world are right | Does relevance reside in documents or in users' situations? |
| Metatheory | What kind of thing a good theory even is | Should information science model itself on physics, on psychology, or on the humanities? |

The deepest fights, Hjørland shows, are metatheoretical: an engineer measuring channel capacity, a cognitive scientist modeling minds, and a domain analyst studying scholarly communities aren't offering rival answers to one question — they're asking different questions, under different assumptions about what counts as an answer. That's why the "what is information?" debate never ends. It isn't a bug or a scandal. It's what happens when a concept has to serve engineering, philosophy, and social science simultaneously.

:::{note} Why "It Depends" Is a Rigorous Answer
Students sometimes find Hjørland's conclusion deflating: seventy-five years of theory and the answer to "what is information?" is *it depends on your framework*? But compare physics, where "what is heat?" got different, useful answers from thermodynamics and statistical mechanics, or biology, where "what is a species?" still has competing definitions serving different research programs. Mature fields don't always converge on one definition; they get precise about which definition is doing the work in which context. That precision — not a final dictionary entry — is what this module is training you in.
:::

## Why Your Theory Chooses Your Technology

Here is where the abstraction cashes out, and it's the move you should practice for the rest of the course: whenever you look at an information system, ask *which theory of information it silently embodies* — and who benefits from that choice.

Search engines are the cleanest example. A ranking algorithm built on pure signal-statistics — click rates, link counts, engagement — is Shannon's heir: it optimizes measurable properties of message flow and stays agnostic about truth. The moment a search engine demotes "low quality" pages or boosts "authoritative" health sources, it has smuggled in semantic and social commitments: somebody decided truth matters and somebody decided which communities (medical associations, fact-checkers, encyclopedias) get to anchor it. Content moderation is the same fork in the road: treat posts as signals and you moderate by volume, virality, and pattern-matching; treat them as claims made by interpreters inside communities and you're forced into the messier work of context, intent, and domain expertise. And the training pipelines of large language models replay the whole debate at industrial scale — every dataset choice is a judgment about whose text counts as good information, made by teams that mostly don't think of themselves as doing information theory at all.

There is no theory-neutral option. Choosing to "just use the data" is choosing the mathematical theory and its famous omission. That doesn't make the engineers wrong — it makes the choice consequential, and mostly invisible until someone like you learns to see it.

## Up Next

We've put meaning, interpreters, and communities back into the picture. Now for the hardest test any theory of information has ever faced: machines that generate fluent, confident, humanlike text about anything, for anyone, instantly. What happens to *knowing*? Continue to [Knowing in the Age of AI](knowing-in-the-age-of-ai.md).
