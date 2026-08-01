# Deepfakes and Synthetic Media

> Seeing used to be believing. Now it's a hypothesis.

## 🎯 In This Section

- Distinguish cheapfakes from deepfakes — and see why the crude version still does most of the damage
- Understand what generative AI changes about the misinformation economy: cost, scale, and personalization
- Examine the evidence that AI-written propaganda actually persuades
- Meet the liar's dividend: how the *existence* of deepfakes lets real evidence be dismissed as fake
- Compare the two big technical responses — detection and provenance — and see why the field is betting on the second

## The Day the Video Stopped Being Proof

For most of the past century, a photograph or a recording settled arguments. Editing was possible but expensive, detectable, and rare enough that "there's video" functioned as a conversation-ender in journalism, courtrooms, and everyday life. That era is closing. Sam Gregory — whose TED talk anchors this section — has spent years at the human-rights organization WITNESS helping activists use video as evidence, which gives him an unusual vantage point: he needs synthetic media to be identifiable not as an academic matter but because real atrocity footage has to remain believable.

Two terms organize the landscape. A **deepfake** is media synthesized or substantially altered by AI — a face swapped onto another body, a voice cloned from samples, a video of an event that never occurred. A **cheapfake** needs no AI at all: it's authentic media made deceptive through cheap tricks — slowing a video to make a politician seem impaired, cropping out context, or simply relabeling old footage as new. The distinction matters because our attention is captured by the sophisticated threat while the crude one does the daily damage. Recall the malinformation example from the last section: a real convoy photo, wrongly captioned, needed no neural network. Cheapfakes exploit our trust in *context*; deepfakes exploit our trust in the *medium itself*.

| | Cheapfake | Deepfake |
|---|-----------|----------|
| Technique | Editing, mislabeling, selective cropping, speed changes | AI synthesis: face swaps, voice clones, generated video and images |
| Skill and cost | Minimal — anyone with a phone | Falling fast — consumer tools now suffice |
| What it exploits | Trust in context and captions | Trust in the recording itself |
| Detection | Reverse image search, provenance checks often work | An arms race — detectors lag behind generators |

## The Frontier-AI Turn

Why is this a Module 8 topic in 2026 rather than a niche forensic curiosity? This week's Shoaib et al. survey maps the answer: frontier AI models have collapsed the cost, skill, and time needed to produce convincing synthetic media across every format at once — text, image, audio, video. What once required a studio or a state now requires a prompt. The survey's threat catalog runs from non-consensual intimate imagery (the most common real-world deepfake harm) through voice-clone fraud, fabricated political events, and synthetic "evidence" injected into breaking news — and, crucially, it frames these not as isolated tricks but as an industrialization of the disinformation supply chain we traced in the last section. Creation was the expensive stage of the lifecycle. It isn't anymore.

But does machine-made persuasion actually persuade? Here this week's Goldstein et al. experiment in *PNAS Nexus* delivers the uncomfortable answer. The researchers took real covert propaganda articles — actual foreign influence-campaign material — and had GPT-3 write new propaganda making the same claims, then measured how persuasive each was to American readers. The result: the AI-written propaganda was nearly as persuasive as the real thing. Read that finding precisely. It doesn't say AI propaganda is irresistible, or better than human propaganda. It says the quality bar has been met — by a model that was already outdated when the study was published. What remains for a propagandist is a question of scale and price, and generative AI answers both in the propagandist's favor. A troll farm once needed fluent writers who understood the target culture; now one operator can generate unlimited, idiomatic, audience-tailored variants at negligible cost.

:::{note} The AI thread, tied off
This is the course's running AI theme at its sharpest. In Module 3 we saw Brundage et al. *forecast* in 2018 that AI would be misused for influence operations; Goldstein et al. is what the receipts look like. The same generative systems we discussed as creativity tools and workplace assistants are, without modification, engines for the misinformation machine. The technology is not neutral or malicious — it is *indifferent*, which in an adversarial setting is enough.
:::

## The Liar's Dividend

Here is the twist that makes deepfakes different from every previous forgery technology, and it's the pivot of Gregory's talk: the biggest harm may come not from fake content being believed, but from real content being *disbelieved*. Once everyone knows convincing fakes exist, "that's a deepfake" becomes a universal solvent for inconvenient evidence. A politician caught on tape, a soldier filmed committing abuses, a CEO recorded making promises — all can now shrug and invoke the possibility of fabrication. Scholars call this the **liar's dividend**: the mere existence of synthetic media pays out to liars, no fakery required.

This should remind you of Module 7. Trust, we saw, is what lets us act on information we can't personally verify — and recorded media was one of modern society's great trust technologies. The liar's dividend attacks that infrastructure directly. The endgame of synthetic media isn't a world where everyone believes fake things; it's a world where belief itself becomes optional, where every piece of evidence can be waved away, and where "nothing is true" quietly becomes "so I'll believe whatever suits me." Disinformation researchers sometimes note that the goal of the most sophisticated campaigns is not persuasion but exhaustion — a population too cynical to believe anything can't coordinate around the truth.

## Detection Versus Provenance

So what's the technical response? Two strategies compete for investment, and the difference between them matters.

**Detection** tries to spot fakes after the fact — classifiers hunting for statistical artifacts, inconsistent lighting, impossible blinks. Both Shoaib et al. and Gregory are sobering here: detection is an arms race in which the generators improve at least as fast as the detectors, detection tools work worst on the compressed, re-uploaded media that actually circulates, and the people who most need them — journalists and fact-checkers outside wealthy newsrooms, as Gregory emphasizes — have the least access to them. Detection can never *prove* authenticity; at best it fails to find evidence of fakery.

**Provenance** flips the problem: instead of proving the fake is fake, prove the real is real. Cryptographically sign media at capture, record its edit history, and let anyone verify where an image came from and what's been done to it — the approach behind emerging content-credential standards backed by camera makers, news organizations, and platforms. Gregory calls the broader strategy "fortifying the truth": since we cannot reliably catch every fake, we strengthen the verifiability of authentic content instead. Provenance has real limits — it requires adoption across the whole media pipeline, most existing media has no credentials, and absence of a signature can't be allowed to condemn authentic footage from a bystander's old phone. But it points at the deeper lesson of this section: the response to synthetic media cannot be purely technological. It is an infrastructure problem — rebuilding, deliberately, the trust in media that we used to get for free.

## Up Next

Detection and provenance defend one link in the lifecycle. The final section, [Fighting Back](fighting-back.md), zooms out to the whole countermeasure toolkit — prebunking, fact-checking, platform design, media literacy, and law — and asks the only question that matters: what does the evidence say actually works?
