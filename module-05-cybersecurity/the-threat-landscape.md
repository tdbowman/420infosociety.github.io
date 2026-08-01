# The Threat Landscape

> A society that runs on information can be attacked anywhere information runs.

## 🎯 In This Section

- See why cybersecurity became a societal problem the moment hospitals, pipelines, and phone networks became information systems
- Build a working vocabulary: ransomware, phishing, social engineering, vulnerability exploitation
- Ground that vocabulary in evidence from the 2026 Verizon Data Breach Investigations Report
- Meet the three broad categories of attacker — criminals, states, and hacktivists — and learn what each one wants
- Examine Salt Typhoon, the espionage campaign inside U.S. telecom networks, as the state-sponsored case

## The Pharmacy Counter Test

In late February 2024, people across the United States walked up to pharmacy counters and were told their insurance couldn't be verified. Some paid hundreds of dollars out of pocket for medication that should have cost a copay. Some walked away without it. Most of them had never heard of the company whose computers had just been locked by criminals — and that is precisely the point.

Here is the test this module keeps applying: when a "computer incident" happens, who feels it, and where? If the answer is "an IT department feels it, in a server room," you're looking at a technology problem. If the answer is "a diabetic feels it, at a pharmacy counter" — or "a city feels it, at the gas pump," as during the Colonial Pipeline shutdown of 2021, or "everyone with a phone feels it," as you'll see shortly — then you're looking at a *societal* problem that happens to travel through technology. Everything this course has told you about the information society — that information processing has been woven into healthcare, finance, energy, logistics, and communication — has a dark corollary. The weave is the attack surface. The more essential information systems become, the more essential attacking them becomes, for anyone who wants money, secrets, or leverage.

That's why this module sits in week five and not in an elective for computer science majors. You cannot understand the information society without understanding what it looks like under attack, any more than you could understand cities without understanding fires.

## A Working Vocabulary, With Receipts

Security conversations drown in jargon, so let's fix four terms precisely — and, unusually for this field, attach evidence to them. Each year Verizon publishes its Data Breach Investigations Report (DBIR), an analysis of real security incidents contributed by companies, insurers, and law enforcement worldwide. The 2026 edition analyzed more than 31,000 incidents, over 22,000 of which were confirmed *breaches* — cases where data was actually exposed, not merely threatened. When a claim in this module has a number attached, this is where it comes from.

**Ransomware** is malicious software that encrypts a victim's systems and data, making them unusable until a ransom is paid — usually in cryptocurrency, usually with a deadline, and increasingly with a second threat layered on: pay, or we also publish the data we stole before locking you out. This is not an exotic scenario. The 2026 DBIR found ransomware present in roughly 48% of breaches — nearly half of everything in the dataset. If the information society has a signature crime, this is it.

**Phishing** is the fraudulent message — an email, a text, a login page that looks exactly like the real one — designed to trick a person into surrendering credentials or running malware. It is the retail storefront of cybercrime: cheap, mass-produced, and effective because it targets people rather than machines.

**Social engineering** is the broader craft phishing belongs to: manipulating humans into defeating their own security. A caller impersonating the help desk, an "urgent" message from the boss, a fake job recruiter — social engineering is as old as the con artist, upgraded with perfect corporate letterhead. Keep this term in mind when we reach AI later in the module, because generative AI is very good at exactly the thing social engineering needs: fluent, personalized, confident text at zero cost.

**Vulnerability exploitation** is the technical route: finding a flaw in software that's exposed to the internet — a web portal, a VPN gateway, a file-transfer server — and using it to walk in without any credentials at all. According to the 2026 DBIR, exploitation of vulnerabilities has become the top initial entry vector — the most common first step attackers take into victim networks. That finding deserves a pause. It means the most common way in is not a hoodie-wearing genius "hacking the mainframe" but attackers systematically scanning the internet for unpatched software — flaws that are publicly known and fixable — and getting there before the fix is applied. Much of cybersecurity failure is not a battle lost; it is maintenance not done.

:::{note} Incidents, Breaches, and Why the Difference Matters
Security statistics are slippery, and the first trick to reading them is the incident/breach distinction the DBIR is careful about. An *incident* is any event that compromises a system — including attacks that were caught and contained. A *breach* is an incident where data was confirmed exposed. Headlines routinely blur the two, which is one reason public numbers about "cyberattacks" range from alarming to apocalyptic. When you cite figures in your own Case Analysis, say which one you mean. Ask of every statistic what Module 1 taught you to ask of every definition: who is counting, and what counts?
:::

## Who Is Attacking, and What Do They Want?

"Hackers" is a nearly useless word — it lumps together a teenager, a criminal cartel, and a military intelligence unit. The threat landscape makes far more sense once you sort attackers by motive.

| Attacker type | Primary motive | Typical operations | This module's example |
|---|---|---|---|
| Criminal groups | Money | Ransomware, data theft and extortion, fraud | ALPHV/BlackCat (Change Healthcare) |
| State-sponsored groups | Intelligence, strategic advantage | Long-term espionage, pre-positioning in infrastructure | Salt Typhoon |
| Hacktivists | Ideology, attention | Defacements, leaks, denial-of-service | Various, usually short-lived |

Criminal groups dominate the numbers. The modern ones operate like software companies — literally. *Ransomware-as-a-service* groups build the malware, run the payment infrastructure and the "customer support" that walks victims through paying, and lease the toolkit to *affiliates* who carry out the actual intrusions in exchange for a cut of the ransom. Remember this division of labor; it becomes darkly important in the next section, when a ransomware operator decides to cheat its own affiliate.

State-sponsored groups play a different game entirely. They rarely announce themselves, because their product is not ransom but *presence*: quiet, durable access to systems worth spying on — or worth disabling later, if relations ever turn hostile. Hacktivists, the third category, attack for ideology or spectacle; they matter less by volume but keep the landscape unpredictable.

## Salt Typhoon: The Spies in the Phone Network

For the state-sponsored case, consider the campaign that U.S. officials disclosed in late 2024 under the name Salt Typhoon. As this week's PBS NewsHour segment reports, hackers attributed to China infiltrated at least eight U.S. telecommunications companies — the carriers that route American calls and texts — with officials describing a sweeping espionage effort against the communications infrastructure itself, including access relevant to systems used for lawful wiretap requests and to communications of senior political figures.

Sit with the audacity of the target selection. Salt Typhoon did not attack particular people's phones; it attacked the network everyone's phones depend on, the layer of the information society we treat as neutral plumbing. That is the state-sponsored logic in its purest form: why compromise a thousand targets individually when you can compromise the infrastructure they all share? And notice the asymmetry with the criminal attacks in the DBIR data: no ransom note, no encryption, no announcement — the entire value of the operation depended on never being noticed. If ransomware is a smash-and-grab, Salt Typhoon is a mole hired into the phone company, years ago, still on the payroll.

The optional Reveron and Savage reading gives this module's underlying claim its academic name: *convergence*. Your personal security, your employer's security, and national security used to be separable concerns handled by different institutions. On shared infrastructure, they collapse into one problem — the same telecom breach touches the teenager's texts, the corporation's deals, and the government's secrets simultaneously.

One more thing the landscape now contains: the DBIR's 2026 edition added new data on AI-assisted threats — attackers using AI to write malware and craft more convincing phishing at scale. Hold that thread; the final section of this module pulls it hard.

## Up Next

You now have the map: the vocabulary, the numbers, and the cast of attackers. Time to zoom all the way in on a single pin on that map — the breach that turned a company you'd never heard of into a national healthcare emergency. Continue to [Anatomy of a Breach](anatomy-of-a-breach.md).
