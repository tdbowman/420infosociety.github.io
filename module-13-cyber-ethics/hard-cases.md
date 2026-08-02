# Hard Cases

> <span style="font-size: 150%;">Principles are cheap until the network goes down.</span>

## 🎯 In This Section

- Put Module 6's ethical frameworks (consequentialist, duty-based, and virtue approaches) to work on three real dilemmas
- Argue both sides of "hack back": self-defense or vigilantism?
- Weigh Teichmann's question of whether paying ransomware attackers should be illegal, from inside a hospital mid-crisis
- Dissect the Arup deepfake fraud, where cybersecurity, ethics, and synthetic media collide
- Turn these cases into fuel for your Futures Portfolio and Friday's discussion

## How to Work a Hard Case

Back in Module 6 you built an ethical toolkit: **consequentialist** reasoning, which judges an act by its outcomes; **duty-based (deontological)** reasoning, which judges it against rules and obligations that hold regardless of outcomes; and **virtue** approaches, which ask what a person of good character, or an institution of good character, would do. The cases in this section are chosen because the frameworks *disagree* about them. That's the point. A dilemma is not a test of willpower. It's a situation where the definitions of "good" pull in different directions. As you read, don't ask "what's the right answer?" first. Ask which framework each argument is secretly running on, and then ask the course's oldest question: who benefits from framing it that way?

## Case One: Hack Back

Your company has been hacked. Customer data is sitting on a server you can actually identify, the criminals are extorting you, and the police, overwhelmed and under-resourced and facing attackers overseas, can't help on any timeline that matters. Your security team says they could break into the attacker's server and delete the stolen data tonight. Current law says they can't: the same statutes that make the criminal's intrusion illegal make your retaliation illegal too. Do you step over the line?

This week's Schaeffer, Spicer, and Olson reading frames the "hack back" debate as it's actually argued in boardrooms and legislatures. The case *for* is consequentialist to its core: victims get little effective protection from the state, attackers act with near impunity from jurisdictions beyond the law's reach, and authorized retaliation could deter crime and recover what was stolen. On this view, forbidding hack back tells victims to lie still while being robbed. Advocates reach for the oldest analogy in ethics: self-defense, a right nobody disputes in the physical world.

The case *against* runs on rules, and on the previous section's hardest lesson: attribution. You are never as sure as you feel about who attacked you. Criminals route attacks through hijacked machines, so the server you counter-attack tonight may belong to an innocent hospital, a small business, or a foreign government that will read your "defense" as aggression. Duty-based reasoning piles on: the state's monopoly on force exists precisely because letting the injured party investigate, judge, and punish in a single furious motion is how feuds work, not justice. And even a consequentialist should flinch at the aggregate outcome: thousands of angry companies retaliating on incomplete evidence, and escalation nobody controls. Vigilantism, Schaeffer and colleagues remind us, always feels like justice from the inside.

The two sides argue from different ground. The *for* side reasons from this victim's outcomes; the *against* side reasons from rules and from everyone's outcomes. Where you land may depend on which seat you're imagining yourself in, which is exactly why the debate stays live.

## Case Two: Pay the Ransom?

Now trade seats. You run a hospital. Ransomware has encrypted your systems at 2 a.m.: schedules, records, lab results. Every hour of downtime is measured in postponed surgeries and ambulances diverted to hospitals farther away. The attackers want millions; your insurer is on the phone; decryption without the key could take weeks. Paying is legal, mostly. You also remember that when the Change Healthcare attack we studied earlier paralyzed claims and payments across American healthcare, the company reportedly paid the attackers $22 million.

This week's Teichmann reading asks the policy question hiding inside your 2 a.m. decision: should paying be *illegal*? The argument for a ban is collective-action logic at its cleanest. Ransomware exists because it pays; every payment funds the next attack and marks payers as targets worth revisiting. Individually rational payments produce a collectively irrational outcome: a thriving criminal industry. Ban payments credibly, the logic runs, and the business model starves. No single victim can escape the trap; only a rule that binds everyone can.

The argument against is standing next to you in the incident room. A ban punishes victims at the worst moment of their institutional lives, and its immediate casualties are not abstractions. They are tonight's patients. Teichmann surveys the responses honestly, including the awkward ones: bans may just push payments underground, into deniable intermediaries and jurisdictions with looser rules, converting a public decision into a hidden one. There's a fairness problem too, since the entities least able to survive a ban (hospitals, schools, small municipalities) are exactly the soft targets attackers prefer.

Run the frameworks. A rule-consequentialist supports the ban for the world it eventually creates; an act-consequentialist standing in your shoes tonight pays. Duty-based reasoning splits down the middle: you have an obligation not to finance criminals *and* an obligation to the patients in your care. Virtue ethics asks what a responsible institution does, and discovers that "responsible" was defined by choices made years earlier, in backup systems and network design, long before the 2 a.m. call. By the time the dilemma arrives, most of the ethics has already happened.

## Case Three: The Colleagues Who Weren't There

In February 2024, an employee in the Hong Kong office of Arup, the global engineering firm behind some of the world's most famous buildings, received a message about a confidential transaction, followed by an invitation to a video call with the company's CFO and several colleagues. The employee was suspicious of the initial message; the call dissolved the suspicion. The people on screen looked right and sounded right. Following the instructions given on the call, the employee made a series of transfers totaling roughly US$25 million before the fraud was discovered. This week's PRMIA case study reconstructs the mechanics: every "colleague" on that call was an AI-generated deepfake.

This is where the module's threads knot together with Module 8's: synthetic media has become an intrusion technique. The Arup attackers compromised no servers and broke no encryption; they compromised *perception*. Every verification habit the employee had been taught (be wary of strange emails, confirm unusual requests with a real person) was satisfied. The call *was* the confirmation. That is what makes this case ethically interesting rather than merely alarming: the human failed at nothing we had trained humans to do.

So run the question the frameworks are worst at: who is responsible? Blaming the employee is emotionally tidy and analytically bankrupt. A security culture that requires every employee to out-perform state-of-the-art AI deception is a system designed to fail and to have someone to blame when it does. The more honest accounting is institutional and procedural: transfers of that size demanded controls that no persuasive conversation could satisfy, including out-of-band verification through channels the attacker doesn't control, multi-party authorization, and deliberate friction. There is a virtue-ethics lesson here about institutions rather than individuals, and a consequentialist one about where prevention money actually works. And there is a warning: the same generative AI you've used all semester as the course's running thread has turned "seeing is believing," the default human trust protocol for a few hundred thousand years, into an exploitable vulnerability.

:::{tip} Feed Your Futures Brief
Any of these three cases would have made a strong Case Analysis Track B, but that ship has sailed; your case analysis is submitted. Use them now as enrichment for the Futures Portfolio instead. If your debate brief touches trust, automation, AI at work, or what skills stay human, this module is a quarry: the Arup fraud is a future-of-work story (what happens to "verify with a colleague" when colleagues can be synthesized?), and the ransomware-ban debate is a governance story your brief can borrow structure from. At Friday's workshop, one of the required review prompts is finding a claim that needs a citation, and the readings above are exactly where sharper citations come from.
:::

## Up Next

Module 13 closes the security arc of the course: hackers and their hats, wars and their missing rulebooks, and three dilemmas that don't resolve so much as trade places. Every hard case here had one thing in common. The decisive move happened *before* the crisis, in the design of institutions, incentives, and defaults. Hold that thought, because next week we turn to the technologies that redesigned social life itself while claiming to be neutral platforms. Continue to [Module 14: Social Media and Society](../module-14-social-media/social-media-and-society.md).
