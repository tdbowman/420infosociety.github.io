# Ethical Hacking

> The difference between a security researcher and a criminal can be a single email asking permission.

## 🎯 In This Section

- Meet the hacker taxonomy (white, gray, and black hats) and see why the neat categories smear in real life
- Understand why authorization, not skill or intent, is the bright line that separates legal security work from crime
- Work through the vulnerability disclosure dilemma: four paths, each with different winners and losers
- See how bug bounties turned an ethical gray zone into a job market
- Confront Flechais and Chalhoub's uncomfortable finding: security practitioners face ethical dilemmas daily, with nothing like medicine's professional infrastructure behind them

## The Person Rattling Your Locks

Picture a stranger walking down your street at midnight, trying every door handle. Alarming? Now suppose the stranger says: "I'm testing which houses are vulnerable, and I leave a note so owners can fix their locks before a burglar arrives." Better? Worse? Now suppose your neighborhood association *hired* her. Your answer probably just changed again, and that progression from intruder to volunteer to professional is the whole moral problem of hacking in miniature.

The security world sorts hackers by hat color, a convention borrowed from old Westerns. This week's Yaacoub survey lays out the taxonomy: **white hats** break into systems with permission, to find weaknesses before criminals do; **black hats** break in for profit, spite, or power; and **gray hats** occupy the vast, contested middle: probing systems without authorization but, at least by their own account, without malice, often disclosing what they find. The survey's real lesson, though, is how unstable these labels are. The same scan, the same exploit, can be a felony, a public service, or a paycheck depending entirely on context. Skills don't come in colors. And people drift: yesterday's teenage gray hat is today's corporate penetration tester, and occasionally the drift runs the other way.

Keren Elazari's TED talk gives the sympathetic reading of this ecosystem: hackers as the internet's immune system, the irritating-but-essential agents that find infections before they spread. It's a powerful metaphor, and in the spirit of this course you should ask what it smuggles in. Immune cells don't have mortgages, egos, or the option of selling what they find. Hackers do.

## Authorization: The Bright Line

If hat colors are fuzzy, the law is not, or at least tries not to be. In the United States, the Computer Fraud and Abuse Act and similar statutes elsewhere generally make *unauthorized access* the offense. Not malicious access. Not harmful access. Unauthorized. A researcher who finds a catastrophic flaw in a hospital's patient portal without permission has, in most jurisdictions, committed a crime, even if she reports it immediately and saves lives by doing so. Good intentions are not a legal category; permission is.

This is why **penetration testing** (hacking a system at its owner's request, under a contract that spells out exactly what may be attacked, how, and when) is the profession's bedrock. The Yaacoub survey walks through how pen testers simulate real attacks, from scanning networks to crafting phishing emails against a client's own employees, all inside a negotiated scope. That scope document carries enormous ethical weight. It converts an act that would otherwise be criminal into a service, the same way consent converts surgery from assault into medicine. Step outside the scope, poke a server the contract didn't name, keep data longer than agreed, and the pen tester is back in the gray zone with everyone else.

:::{warning} Curiosity Is Not a Defense
Students sometimes assume that finding a flaw "to help" is legally safe. It usually is not. Probing a system you don't own and weren't invited to test can be a crime in most jurisdictions regardless of your intentions, and organizations have prosecuted the researchers who reported flaws to them. If you're drawn to security work, learn on systems built for practice, in courses, competitions, and bug-bounty programs with published rules, never on live systems that haven't invited you.
:::

## Four Doors: The Disclosure Dilemma

Now for the decision at the heart of security ethics. Suppose a researcher, authorized or not, discovers a serious vulnerability. What should she do with it? There is no move that helps everyone, and the field has argued about this for decades.

:::{figure} images/disclosure-paths.svg
:name: disclosure-paths
:alt: A flowchart showing a box labeled researcher finds a vulnerability on the left, with arrows fanning out to four paths on the right: full public disclosure, annotated as forcing the issue into the open but arming attackers before any patch exists; a highlighted coordinated disclosure chain running from disclosure to vendor through patch developed and released to publish findings, annotated as protecting users but hinging on the vendor acting; sell to a broker or government, annotated as rewarding the finder while the flaw stays secret and possibly weaponized; and do nothing, annotated as leaving the flaw for someone less scrupulous to find.
:width: 100%

The disclosure decision. Each path distributes risk, reward, and knowledge differently, which is why researchers, vendors, and governments have never fully agreed on the "right" one.
:::

**Full public disclosure**, publishing everything immediately, sounds reckless, and sometimes is: it hands working attack instructions to every criminal on earth before a fix exists. But its defenders have a serious argument. For years, vendors ignored privately reported flaws, quietly leaving customers exposed; publication was the only pressure that reliably worked. Full disclosure treats users as adults who deserve to know their locks are broken *now*, not when the locksmith gets around to it.

**Coordinated disclosure** (you'll also see "responsible disclosure," a name researchers dislike for implying every alternative is irresponsible) is the compromise the industry has mostly settled on: tell the vendor privately, allow a reasonable window to build and ship a patch, then publish. It protects users when it works. It also asks the researcher to stay silent, sometimes for months, trusting a vendor whose incentive is often to delay, downplay, or lawyer up.

**Selling** the flaw to a broker or a government agency pays best. Brokers resell to intelligence and law-enforcement agencies, which stockpile undisclosed flaws for surveillance and offensive operations. The flaw never gets fixed; it becomes ammunition. Whatever you think of any particular government's purposes, this market prices vulnerabilities in *your* software according to their value as weapons against someone else.

**Doing nothing** looks like the null choice, but it isn't. Vulnerabilities are rediscovered; the flaw the careful researcher walks away from is still there for the careless or the criminal one.

**Bug bounties** (programs in which companies publicly invite hackers to probe their systems and pay for what they find) are the industry's attempt to collapse this whole dilemma into a job. They institutionalize the gray hat: authorization in advance, money on delivery, rules published for everyone. They've turned thousands of would-be gray hats into a legitimate global workforce, though critics note the fine print sometimes buys silence as much as security.

## A Profession Without a Professional Code

Here is the part that should genuinely unsettle you. A physician facing a hard call can lean on centuries of accumulated infrastructure: codes of ethics drilled in from the first year of training, licensing boards with the power to end careers, ethics committees on call in every hospital. This week's Flechais and Chalhoub reading asks what the equivalent looks like in cybersecurity, and finds mostly empty space. Interviewing practitioners across the field's domains (mapped against CyBOK, the field's attempt to catalogue its own body of knowledge), they document professionals encountering ethical dilemmas as a routine part of the job: What do I do with sensitive data I stumbled across? Whose interests come first when my client and their users conflict? When do I escalate, and to whom?

What they don't find is a shared way of answering. There is no license to lose, no hacking equivalent of the medical board, no standard ethics training, no profession-wide code with teeth: just fragmentary guidelines and individual conscience, exercised under deadline pressure. The people guarding hospital networks, power grids, and your own data are working from personal judgment. AI is raising the stakes on both sides of the fight, since the same models that help defenders triage alerts help attackers write convincing phishing at scale. It's a dual-use pattern you'll recognize from Module 3, now aimed at a profession with no ethics board to call.

:::{seealso} The Comparison to Sit With
Medicine took centuries, and scandals, to build its ethical infrastructure. Flechais and Chalhoub's implicit question: does cybersecurity get its own infrastructure before or after its equivalent of the scandals that forced medicine's hand? Carry that question into the next section, where the stakes escalate from bug reports to war.
:::

## Up Next

Individual hackers, at least, mostly operate in peacetime. But what happens when hacking becomes a weapon of war, and when the hackers are volunteers who never enlisted? In [Cyber Conflict and the Laws of War](cyber-conflict-and-the-laws-of-war.md), the Red Cross tries to hand out rulebooks on a digital battlefield.
