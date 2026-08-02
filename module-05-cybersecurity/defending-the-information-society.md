# Defending the Information Society

> <span style="font-size: 150%;">Attackers need one open door. Defenders answer for every door, and for deciding, as a society, which doors matter most.</span>

## 🎯 In This Section

- Understand defense in depth: why security is built in layers rather than walls
- See the policy layer in action by comparing the 2023 and 2026 national cybersecurity strategies
- Recognize why cybersecurity is politics, meaning contested choices about responsibility and power, and not just engineering
- Trace AI's arrival on both sides of the fight, from DBIR trend data to the first reported AI-orchestrated espionage campaign
- Connect this module to your Case Analysis decision this week

## No Wall Holds

If the last section taught anything, it's that single defenses fail. A password failed at Change Healthcare. Somewhere right now, a patch is missing, a backup is silently broken, an employee is about to click. The organizing idea of modern security accepts this from the start. **Defense in depth** means building layers, each one assuming the previous one has already failed. MFA assumes the password is stolen. Network segmentation assumes the intruder is inside and walls off what they can reach. Monitoring assumes the walls were climbed and watches for the climber. Offline backups assume the ransomware fired and make the ransom refusable. Incident-response plans assume all of the above and rehearse the bad day before it comes.

Run last section's chain through these layers and the point makes itself: every stage of the Change Healthcare breach is a layer that wasn't there or didn't hold. The mitigations in the CISA advisory you skimmed are this same list in official prose. Defense in depth is not a secret, and the advisory urging it on the healthcare sector predated the catastrophe it describes. So if the playbook is public, why doesn't everyone run it? Partly cost, since every layer takes money, staff, and friction that organizations feel every day, weighed against attacks that arrive rarely. Partly incentives: as with Change Healthcare, much of the damage lands on patients and clinics rather than on the balance sheet that chose the security budget. When the party choosing the protection isn't the party bearing the harm, underinvestment is not an accident. It's the predictable result. Fixing incentive problems is not an engineering task but a governance task, which is why every information society ends up needing a policy layer above the technical ones.

## The Policy Layer: A Tale of Two Strategies

That policy layer is where this week's most unusual reading assignment lives: two documents from the same building, written three years apart, by administrations from opposite parties. In 2023, the Biden administration published the implementation plan for its National Cybersecurity Strategy, now preserved on the archived White House site. In March 2026, the Trump administration published *President Trump's Cyber Strategy for America*. You're reading them side by side not to memorize either one, but to run the course's signature move on both: which assumptions is each document making, and who benefits?

As you compare, work through questions like these. Where does each strategy place responsibility: on individuals, on companies, on government? What does each treat as the main threat, and as the main tool? Regulation, market incentives, offensive capability, alliances? What vocabulary appears in one and vanishes from the other? What survives the transition untouched, and doesn't that continuity tell you which threats are treated as facts rather than politics?

The deeper lesson is that the comparison is possible at all. Bridges do not get re-argued every election. National cyber strategy does, because it is genuinely political. A cybersecurity strategy decides who must spend money, who gets blamed after a breach, how much power government has over private networks, and how aggressive a nation will be inside other nations' systems. Those are questions about the distribution of burdens and power, which is the definition of politics. "Cybersecurity is politics, not just engineering" doesn't mean the engineering is optional. It means the engineering happens inside choices that engineers don't get to make. The whiplash has costs of its own: the defenders at hospitals and utilities, and adversaries like the Salt Typhoon operators you met earlier, both plan on horizons longer than one administration. Whether a society that redraws its defensive doctrine every few years can hold ground against opponents who don't is one of the open questions of this decade. By December, whichever way current events break, you'll have a framework for reading them.

:::{seealso} Primary Sources Are a Habit Now
This is the second time this module has sent you to primary documents: first a joint federal advisory, now two White House strategies. See how differently they read from news coverage *about* them, and what officials emphasize, hedge, and omit. If you choose Track B of the Case Analysis, this habit is your competitive edge. Build your paper on advisories, filings, and strategy documents, and use journalism as the connective tissue rather than the foundation.
:::

## AI Joins Both Sides

This course keeps insisting AI is the running thread of the information society, and cybersecurity is where the thread now glows. Start on the attackers' side, with the trend data. The 2026 DBIR added new findings on AI-assisted threats, with attackers using AI to generate more convincing phishing lures and to speed up their operations. Recall from the first section what social engineering needs in order to scale: fluent, personalized, confident text at near-zero cost. Generative AI is a social-engineering factory, and the DBIR's data shows the factory is running.

Then, in November 2025, came a qualitative jump. Anthropic, the AI company whose safety research you've met before in this course, published a report on what it called the first publicly reported AI-orchestrated cyber espionage campaign. A state-sponsored group had used an AI agent to carry out roughly 80 to 90 percent of the campaign autonomously. This was not AI helping a hacker draft an email. It was an AI agent executing the bulk of the intrusion work itself, with humans supervising rather than performing the operation. Read that against your Module 3 Brundage reading. In 2018, Brundage and colleagues forecast that AI would expand existing threats by making attacks cheaper and more scalable, and would change their character by reducing the human labor each attack requires. Seven years later, an AI company was documenting a live campaign matching the forecast. That is what it looks like when a speculative-sounding risk report turns into an incident report, and it's worth remembering the next time you're tempted to dismiss forecasts about emerging technologies as science fiction. Some are. The way to tell the difference is the discipline you're practicing in this course: check the argument, then check back later against the evidence.

Defenders are not standing still, and the same properties that make AI useful to attackers (speed, scale, tirelessness) serve defense too. Security teams drown in alerts, the vast majority of them false alarms, and machine-speed attacks are hard to counter with human-speed triage. AI systems that filter, prioritize, and investigate that flood are among the most promising defensive applications. In Module 11 you'll read about the U.S. Air Force using AI for exactly this kind of alert triage, and you'll be able to evaluate it with this module's picture of what defenders are up against. Whether the AI era ultimately favors offense or defense is unsettled, which makes it exactly the kind of forecast Brundage taught you to treat as a hypothesis to track rather than a fact to accept.

:::{tip} Choosing Your Case Analysis Track
This week you commit to a track for the Case Analysis. If this module hooked you, Track B (Cybersecurity Incident) asks you to investigate a significant breach or campaign: its causes, effects, and dilemmas. Change Healthcare and Salt Typhoon are both strong choices with rich primary sources, but any significant incident is fair game with instructor approval. Whichever track you pick, start collecting primary sources now. Your draft goes to peer review in Module 9.
:::

## Wrapping Up Module 5

This module argued one thesis three ways: cybersecurity is a societal condition, not a technical specialty. The first section showed you attacks measured in DBIR statistics but felt at pharmacy counters and inside phone networks. Change Healthcare showed you how a single missing safeguard, amplified by a single point of failure, became a national emergency, and how even paying the ransom bought less than promised. This section showed you the defense: technical layers that are well understood, incentive and policy layers that are genuinely contested, and an AI arms race arriving on both sides at once. Keep the Change Healthcare chain in your head as the course moves on. You'll meet its ethical questions again in Module 13, its AI questions in Module 11, and its trust questions everywhere.

**Up Next:** [Module 6: Information Ethics](../module-06-ethics/information-ethics.md)
