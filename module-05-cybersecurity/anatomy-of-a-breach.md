# Anatomy of a Breach

> Every catastrophic breach looks inevitable in hindsight and impossible the day before.

## 🎯 In This Section

- Reconstruct the February 2024 Change Healthcare breach stage by stage, using Moore's timeline
- See how one set of stolen credentials, on a system without multi-factor authentication, became a nationwide healthcare outage
- Read a real joint government advisory (CISA, FBI, and HHS) on the group responsible
- Understand what the breach reveals about single points of failure in the information society
- Preview the ransom-payment dilemma you'll wrestle with properly in Module 13

## The Company Nobody Knew

Before February 2024, you could have asked a hundred Americans what Change Healthcare was and gotten a hundred shrugs. Yet the company, a subsidiary of UnitedHealth Group, the largest health insurer in the United States, sat at the center of American medicine. It operated as a clearinghouse: the switchboard through which pharmacies, hospitals, and clinics send insurance claims and receive payments. Every time a pharmacist checked your coverage or a clinic billed your insurer, there was an excellent chance the transaction passed through Change Healthcare's systems. An enormous share of the country's health transactions flowed through this one intermediary.

This is the shape of the modern information society that Module 1 promised you'd keep meeting again: invisible intermediaries, consolidated through mergers, achieving efficiencies by centralizing what used to be scattered. Efficiency and fragility are the same architecture viewed from different angles. On February 21, 2024, the other angle came into view.

## The Chain, Link by Link

This week's Moore reading assembles the timeline of what happened, and its most shocking feature is how unshocking the opening move was. The attackers, an affiliate of the ransomware-as-a-service operation ALPHV (also called BlackCat), did not deploy some exotic zero-day exploit against a hardened perimeter. They logged in. They used stolen credentials for a remote-access portal, and that portal was not protected by **multi-factor authentication** (MFA), the now-standard second check, like a code on your phone, that makes a stolen password insufficient by itself. One password, no second factor, and the front door of the switchboard of American healthcare swung open.

From there the chain ran with grim logic, as the figure below traces. Inside the network, the intruders moved and gathered, doing reconnaissance and stealing data. Then came the detonation. Ransomware encrypted Change Healthcare's systems, and the company took its platforms offline to contain the damage. Because those platforms were the pipes, shutting them shut the flow: claims processing and billing seized up for a huge share of U.S. pharmacies, hospitals, and clinics. Patients hit the pharmacy-counter wall you met in the last section. Providers went weeks without reimbursement, and small practices that live claim-to-claim borrowed money to make payroll. A ransom of roughly $22 million was paid. Then the story took a turn that no one's incident-response playbook anticipated. ALPHV's operators pulled an *exit scam*, taking the ransom money, cutting out the affiliate who had actually carried out the intrusion, and vanishing. The affiliate still had the stolen data, so a second extortion demand followed. Paying the criminals had purchased neither the data's destruction nor even the criminals' cohesion. Ultimately, data belonging to roughly a third of Americans was implicated in the breach.

:::{figure} images/breach-anatomy.svg
:name: breach-anatomy
:alt: A flowchart tracing the Change Healthcare breach through seven linked stages arranged in two rows (stolen credentials on a portal with no multi-factor authentication, network intrusion, ransomware deployment, nationwide outage of claims and billing, a roughly 22 million dollar ransom payment, the ALPHV exit scam, and a second extortion demand), with a note that data of roughly a third of Americans was implicated.
:width: 100%

Anatomy of the Change Healthcare breach, February 2024. One weak link, stolen credentials on a portal without MFA, cascaded into a nationwide outage, a $22 million ransom, and, after the criminals cheated each other, a second extortion. Based on the timeline in this week's Moore reading.
:::

Walk the chain backward. Every link had to hold for the catastrophe to complete, which means any link could have broken it. MFA on the portal stops the login. Faster detection catches the intruder before the ransomware fires. Less centralization means an outage that inconveniences a region instead of a nation. Security professionals think in these terms, in attack chains with multiple stages, because defense doesn't have to win everywhere. It has to win once. That idea, defense in layers, is the spine of the next section.

## Reading the Government's File on BlackCat

Alongside Moore's journalism, this week you're skimming a different genre entirely: the joint advisory on ALPHV/BlackCat issued by CISA (the Cybersecurity and Infrastructure Security Agency), the FBI, and the Department of Health and Human Services, catalogued as AA23-353A. Advisories like this are how the U.S. government pushes threat intelligence to the public: who the group is, how its ransomware-as-a-service business operates, the technical fingerprints its intrusions leave, and the concrete mitigations organizations should apply.

The document is a primary source, the defenders' own working file published in something close to real time, and it was issued in December 2023, *before* the Change Healthcare attack. The government had named this group, described its methods, and urged the healthcare sector specifically to harden itself, months ahead of the disaster. Knowing about a threat and being defended against it are, as ever in the information society, two very different states. When you write your own Case Analysis, an advisory like this is the kind of source that separates a research paper from a summary of news coverage. It lets you check journalists' claims against the technical record.

:::{warning} Hindsight Is Cheap
It is easy to narrate a breach as a sequence of obvious blunders, and this section has been doing exactly that. Resist letting it curdle into contempt. Change Healthcare's defenders were protecting thousands of systems inherited through years of mergers, and the attackers needed to find one gap. The honest lesson is not "they were careless and we would not be." It is that at sufficient scale and complexity, *someone's* portal is always missing MFA. That's why the deeper questions in this module are structural ones: how much should any one node be allowed to matter, and who checks that the checks are in place?
:::

## The Single Point of Failure Problem

The deepest lesson of Change Healthcare is not about passwords. It's about topology. A clearinghouse is efficient because everyone connects to it, and dangerous for the same reason. The consolidation that let one company process a vast share of the nation's health transactions guaranteed that one company's bad day would be the nation's bad day. Economists and engineers have names for this, systemic risk and single point of failure, and you have now watched it operate at full scale in the one sector where downtime is measured in missed medications.

Here the module's societal framing pays off. If cybersecurity were only an IT problem, the fix would be Change Healthcare's alone: patch, add MFA, move on. Seen as a societal problem, the questions multiply and change character. Should any single intermediary be allowed to carry that share of a critical system? Is a company that processes a third of the nation's health data infrastructure, like a power grid, and should it be regulated like one? Who owes what to the small clinics that nearly went under, or to the patients whose data ended up in criminal hands? None of those are questions a firewall can answer.

And hovering over all of it, the ransom. UnitedHealth paid roughly $22 million, and the exit scam meant even that bought less than promised. Was paying wrong? It may have been the fastest route to restoring a system the country needed urgently. It also funded a criminal industry and advertised that attacking healthcare pays. Every ransom payment is a private decision with public consequences. Sit with the discomfort of that trade-off. Module 13 takes up the ethics of ransom payments, and the arguments for banning them, in full.

## Up Next

You've now seen the information society attacked at its weakest point and its most central node at once. The obvious question is what defending it should look like: at the level of logins, of organizations, and of nations that can't agree with their own previous administrations about the answer. Continue to [Defending the Information Society](defending-the-information-society.md).
