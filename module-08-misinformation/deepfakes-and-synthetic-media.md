# Deepfakes and Synthetic Media

> Seeing used to be believing. Now it's a hypothesis.

## 🎯 In This Section

- Distinguish cheapfakes from deepfakes, and see why the crude version still does most of the damage
- Understand what generative AI changes about the misinformation economy: cost, scale, and personalization
- Examine the evidence that AI-written propaganda actually persuades
- Meet the liar's dividend: how the *existence* of deepfakes lets real evidence be dismissed as fake
- Compare the two big technical responses, detection and provenance, and see why the field is betting on the second

## The Day the Video Stopped Being Proof

For most of the past century, a photograph or a recording settled arguments. Editing was possible but expensive, detectable, and rare enough that "there's video" functioned as a conversation-ender in journalism, courtrooms, and everyday life. That era is closing. Sam Gregory, whose TED talk anchors this section, has spent years at the human-rights organization WITNESS helping activists use video as evidence. That work gives him an unusual vantage point. For him, identifying synthetic media is a practical necessity, because real atrocity footage has to remain believable.

Two terms organize the field. A **deepfake** is media synthesized or substantially altered by AI: a face swapped onto another body, a voice cloned from samples, a video of an event that never occurred. A **cheapfake** needs no AI at all. It's authentic media made deceptive through cheap tricks, like slowing a video to make a politician seem impaired, cropping out context, or simply relabeling old footage as new. The distinction matters because our attention is captured by the sophisticated threat while the crude one does the daily damage. Recall the malinformation example from the last section: a real convoy photo, wrongly captioned, needed no neural network. Cheapfakes exploit our trust in *context*; deepfakes exploit our trust in the *medium itself*.

| | Cheapfake | Deepfake |
|---|-----------|----------|
| Technique | Editing, mislabeling, selective cropping, speed changes | AI synthesis: face swaps, voice clones, generated video and images |
| Skill and cost | Minimal; anyone with a phone | Falling fast; consumer tools now suffice |
| What it exploits | Trust in context and captions | Trust in the recording itself |
| Detection | Reverse image search, provenance checks often work | An arms race; detectors lag behind generators |

## The Frontier-AI Turn

Synthetic media used to be a niche forensic curiosity. This week's Shoaib et al. survey explains why it isn't one now: frontier AI models have collapsed the cost, skill, and time needed to produce convincing synthetic media across every format at once, including text, image, audio, and video. What once required a studio or a state now requires a prompt. The survey's threat catalog runs from non-consensual intimate imagery (the most common real-world deepfake harm) through voice-clone fraud, fabricated political events, and synthetic "evidence" injected into breaking news. It frames all of this as an industrialization of the disinformation supply chain we traced in the last section. Creation was the expensive stage of the lifecycle. It isn't anymore.

Machine-made persuasion does in fact persuade, and this week's Goldstein et al. experiment in *PNAS Nexus* is where you'll see it. The researchers took real covert propaganda articles (actual foreign influence-campaign material), had GPT-3 write new propaganda making the same claims, then measured how persuasive each was to American readers. The result: the AI-written propaganda was nearly as persuasive as the real thing. Read that finding precisely. It doesn't say AI propaganda is irresistible, or better than human propaganda. It says the quality bar has been met, by a model that was already outdated when the study was published. What remains for a propagandist is a question of scale and price, and generative AI answers both in the propagandist's favor. A troll farm once needed fluent writers who understood the target culture. Now one operator can generate unlimited, idiomatic, audience-tailored variants at negligible cost.

:::{note} The AI thread, tied off
This is the course's running AI theme at its sharpest. In Module 3 we saw Brundage et al. *forecast* in 2018 that AI would be misused for influence operations; Goldstein et al. is what the receipts look like. The same generative systems we discussed as creativity tools and workplace assistants are, without modification, engines for the misinformation machine. The technology is *indifferent* rather than neutral or malicious, and in an adversarial setting indifference is enough.
:::

## The Liar's Dividend

Gregory's talk pivots on the twist that makes deepfakes different from every previous forgery technology. The biggest harm may come from real content being *disbelieved*. Once everyone knows convincing fakes exist, "that's a deepfake" becomes a universal solvent for inconvenient evidence. A politician caught on tape, a soldier filmed committing abuses, a CEO recorded making promises: all can now shrug and invoke the possibility of fabrication. Scholars call this the **liar's dividend**: the mere existence of synthetic media pays out to liars, no fakery required.

This should remind you of Module 7. Trust, we saw, is what lets us act on information we can't personally verify, and recorded media was one of modern society's great trust technologies. The liar's dividend attacks that infrastructure directly. The endgame of synthetic media is a world where belief itself becomes optional, where every piece of evidence can be waved away, and where "nothing is true" quietly becomes "so I'll believe whatever suits me." Disinformation researchers sometimes note that the goal of the most sophisticated campaigns is exhaustion rather than persuasion. A population too cynical to believe anything can't coordinate around the truth.

## Detection Versus Provenance

Two technical strategies compete for investment, and the difference between them matters.

**Detection** tries to spot fakes after the fact, with classifiers hunting for statistical artifacts, inconsistent lighting, impossible blinks. Both Shoaib et al. and Gregory are sobering here. Detection is an arms race in which the generators improve at least as fast as the detectors. Detection tools work worst on the compressed, re-uploaded media that actually circulates. And the people who most need them, journalists and fact-checkers outside wealthy newsrooms, as Gregory emphasizes, have the least access to them. Detection can never *prove* authenticity; at best it fails to find evidence of fakery.

**Provenance** flips the problem: instead of proving the fake is fake, prove the real is real. Cryptographically sign media at capture, record its edit history, and let anyone verify where an image came from and what's been done to it. That's the approach behind emerging content-credential standards backed by camera makers, news organizations, and platforms. Gregory calls the broader strategy "fortifying the truth": since we cannot reliably catch every fake, we strengthen the verifiability of authentic content instead. Provenance has real limits. It requires adoption across the whole media pipeline, most existing media has no credentials, and absence of a signature can't be allowed to condemn authentic footage from a bystander's old phone. But it points at the deeper lesson of this section. The response to synthetic media cannot be purely technological. It's an infrastructure problem, and the work is to rebuild, deliberately, the trust in media that we used to get for free.

## Up Next

Detection and provenance defend one link in the lifecycle. The final section, [Fighting Back](fighting-back.md), zooms out to the whole countermeasure toolkit (prebunking, fact-checking, platform design, media literacy, and law) and asks what the evidence says actually works.
