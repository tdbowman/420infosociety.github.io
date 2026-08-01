# Ethical Frameworks for Technology

> "Technology is neither good nor bad; nor is it neutral."
> — Melvin Kranzberg, "Kranzberg's Laws" (1986)

## 🎯 In This Section

- Meet the five ethical frameworks you'll use all semester: consequentialism, deontology, virtue ethics, care ethics, and justice as fairness
- Apply all five to the *same* system — an algorithm that screens job applicants — and watch them reach different verdicts
- Learn what each framework sees clearly and what it is structurally blind to
- Understand information ethics as a field, organized around privacy, accuracy, property, and access
- Practice the move you'll need for Case Analysis Track A: analysis, not vibes

## One Algorithm, Five Verdicts

Here is the running example for this entire section, so hold onto it. A mid-sized company gets four thousand applications for every opening. It buys a screening system: a model trained on ten years of the company's own hiring records that reads each résumé and scores it. Recruiters only see the top two hundred. The system is fast, cheap, consistent, and never gets tired at 4 p.m. It is also trained on the company's past decisions — including whatever patterns of preference and prejudice those decisions contained. Candidates are never told a model screened them, and there is no way to appeal a score nobody will ever show them.

Is this system ethical? Notice what happens in your head when you read that question: you probably reached for a gut verdict within seconds. Ethical frameworks exist to slow that reflex down. Each framework is a disciplined way of asking *what matters* about a situation — and because they disagree about what matters, they can disagree about the verdict. That disagreement is not a failure of ethics. It is the discipline working: each framework surfaces a consideration the others underweight. Your job this week is to learn to run all five, then argue for a judgment.

## The Big Three: Consequences, Duties, Character

**Consequentialism** says an act is right if it produces the best overall outcomes; the most famous version, utilitarianism, tells you to maximize total well-being. A consequentialist audits our hiring algorithm by adding up its effects. On the plus side: thousands of hours saved, more applications actually read (a human recruiter skims; the model at least scores everyone), and possibly more consistency than a tired, biased human. On the minus side: if the training data encodes a past preference for certain schools, zip codes, or genders, the model reproduces it at scale — and because rejected candidates never enter the company, the system never learns what it missed, quietly compounding the harm year after year. The consequentialist verdict is conditional: the system is acceptable *if* measurement shows the benefits outweigh the harms. Which reveals the framework's structural weakness — it is only as good as your ability to measure consequences, and the people choosing what to measure are usually the people who bought the system.

**Deontology**, associated above all with Immanuel Kant, says some things are required or forbidden regardless of outcomes, because persons must be treated as ends in themselves and never merely as means. A deontologist doesn't need the harm data. The system judges human beings through statistical proxies they never consented to, conceals its own existence from them, and offers no reasons and no appeal. That fails the duty of respect on its face: a person reduced to a score, produced in secret, with no opportunity to contest it, is being treated as an object to be sorted rather than an agent owed reasons. The deontological verdict is not "measure the harms" but "certain features of this system are wrong even if it works" — and the fixes it demands are disclosure, explanation, and appeal, not better accuracy.

**Virtue ethics**, descending from Aristotle, changes the subject from the act to the actor: what would a person (or organization) of good character — honest, just, practically wise — do here? The virtue ethicist asks what it says about a company that it outsources judgment about *people* to a system nobody in the building fully understands, then declines to mention this to the people being judged. Hiring is a practice with internal goods: discernment, fairness, the giving of chances. A company that automates the practice while abandoning those goods hasn't just risked bad outcomes; it has made itself worse — less honest, less just, less capable of judgment. The verdict here is about formation: what kind of institution are we becoming, one automated decision at a time?

## Two More Tools: Care and Fairness

The big three dominate textbooks, but two further frameworks do work the others miss.

**Care ethics** starts from relationships and vulnerability rather than rules or aggregates. It notices what the other frameworks abstract away: the single applicant, three months unemployed, whose résumé has a two-year gap from caring for a dying parent — a gap the model, trained on uninterrupted careers, silently penalizes. Care ethics insists that ethical judgment attend to particular people in particular circumstances of dependency and unequal power. Its verdict on the hiring algorithm focuses on the asymmetry: the company risks a bad hire; the applicant risks a livelihood. Any system that cannot see context — cannot distinguish a caregiving gap from a disqualifying one — fails the vulnerable first.

**Justice as fairness** is the philosopher John Rawls's great thought experiment. Design your institutions from behind a *veil of ignorance*: you don't know whether you'll be the hiring manager or the applicant, the Stanford graduate or the community-college transfer, the person the training data resembles or the person it has never seen. Would you approve this screening system without knowing which position you'd occupy in it? Rawls adds that inequalities are tolerable only when they work to the benefit of the least advantaged. A system that speeds things up for recruiters while systematically burying nontraditional candidates flunks that test — unless it is redesigned so that the people the old process served worst are the ones the new process serves best.

| Framework | Core question | On the hiring algorithm |
|---|---|---|
| Consequentialism | What produces the best overall outcomes? | Acceptable only if audited benefits demonstrably outweigh harms — including harms nobody is measuring |
| Deontology | What duties do we owe persons as ends in themselves? | Secret, reasonless, unappealable judgment is wrong regardless of accuracy |
| Virtue ethics | What would a person or institution of good character do? | Outsourcing judgment about people, and hiding it, corrodes the institution's character |
| Care ethics | What do the vulnerable and dependent need from this relationship? | A system blind to context fails precisely the applicants with the most at stake |
| Justice as fairness | Would you accept this design without knowing your place in it? | Fails the veil of ignorance unless the least advantaged benefit from the change |

:::{tip} Frameworks Are Lenses, Not Vending Machines
Do not treat these frameworks as machines where you insert a case and a verdict drops out. In Case Analysis Track A, the weakest papers name-drop "utilitarianism says..." and move on. The strongest papers show two frameworks *disagreeing* about the same facts, explain what each one is seeing that the other isn't, and then argue — with reasons — for a position. Disagreement between frameworks is where the analysis lives.
:::

## Information Ethics as a Field

The frameworks are ancient; the field that applies them to information is not. Information ethics emerged as computing did, and it has long organized itself around four recurring issue clusters, memorably framed in the 1980s by information scholar Richard Mason as the *PAPA* issues: **privacy** (who may know what about you, and who decides?), **accuracy** (who is accountable when information about you is wrong?), **property** (who owns information and the value it creates?), and **access** (who gets to the information — and the tools — that participation in society now requires?).

Run the hiring algorithm through PAPA and notice that it lights up all four. Privacy: the model may infer things — health, parenthood, age — that no interviewer could lawfully ask. Accuracy: a parsing error that mangles your job history is invisible to you and uncorrectable. Property: your résumé, and the ten years of past applicants' data behind the model, generate value that none of those people share. Access: candidates who know how to keyword-optimize a résumé for machines — a skill that tracks privilege — get systematically better odds. The PAPA issues are older than AI, which is exactly the point: AI didn't invent information ethics' problems; it industrialized them. When you read the Values and Principles sections of this week's UNESCO Recommendation, you will recognize both the ancient frameworks and the PAPA issues under new names — dignity, fairness, transparency, accountability — a hint of where this module ends up: ethics trying to become law.

## Up Next

You now have five lenses and a field to point them at. Next we survey what the lenses reveal when aimed at AI specifically: the classic problem map, the strange new problems generative AI added, and a fight about which dangers deserve your attention. Continue to [The Ethics of AI](the-ethics-of-ai.md).
