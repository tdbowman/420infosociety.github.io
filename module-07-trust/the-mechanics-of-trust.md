# The Mechanics of Trust

> Trust is the tax you never see on every transaction you ever make, and the only tax that gets cheaper the more everyone pays it.

## 🎯 In This Section

- See why trust is the invisible infrastructure of the information society, presumed by every login, purchase, and share
- Learn Riegelsberger, Sasse, and McCarthy's framework: contextual and intrinsic trust-warranting properties, and the signals that carry them
- Distinguish *symbols* of trustworthiness (easy to fake) from *symptoms* (hard to fake), and spot both in the platforms you use daily
- Master the distinction between trust and trustworthiness, and why confusing them is profitable for the wrong people
- Build the conceptual toolkit the rest of this module applies to machines, institutions, and chatbots

## Count Your Leaps of Faith

Reconstruct your morning. You unlocked your phone and believed the time it showed you. You tapped a card against a reader and assumed a chain of banks you cannot name would move your money and not someone else's. You ordered coffee through an app, trusting a stranger to make it, another stranger to carry it, and a corporation to have vetted both. Maybe you got into a car because an app told you the driver was named Marcus and had 4.9 stars. By nine in the morning you had extended trust to dozens of people you will never meet and systems you cannot inspect, and it never once felt like a decision.

That is what this module means by calling trust the *invisible infrastructure* of the information society. Like plumbing or the power grid, it only becomes visible when it fails: the breach notification, the counterfeit product, the review section that turns out to be bought. Every transaction, login, purchase, and share presumes it. And like physical infrastructure, it was engineered by people making deliberate design decisions about what you would see, when you would see it, and why it would make you feel safe.

Before we can ask whether that engineering is honest, we need a precise vocabulary. Social scientists define trust as a willingness to make yourself vulnerable to another party based on the expectation that they will act in your interest, even though you cannot control them and could be hurt if you're wrong. Two ingredients are essential. There must be *risk*: if nothing bad can happen, nothing is being trusted. And there must be *uncertainty*: if you can verify everything in advance, you don't need trust, you have proof. Trust is the bridge we build over the gap where proof runs out.

## Riegelsberger's Machine: Properties and Signals

This week's Riegelsberger, Sasse, and McCarthy reading was written in 2005, when buying anything online still felt slightly reckless, and it asks the question underneath all of e-commerce: what makes it *rational* to trust a stranger? Their answer has become a classic framework, and it is worth learning cold.

Picture two parties. The *trustor* is the one taking the risk: the buyer, the guest, the user. The *trustee* is the one being relied upon: the seller, the host, the platform. The trustor's problem is that trustworthiness is invisible. You cannot see honesty the way you see a price tag. What you can see are *signals*. What the signals advertise, when the system works, are the trustee's *trust-warranting properties*, the actual facts about them that make trusting them a good bet.

:::{figure} images/trust-mechanics.svg
:name: trust-mechanics
:alt: A framework diagram showing a trustor box on the left and a trustee box on the right, connected by two horizontal arrows: a teal signals arrow carrying symbols and symptoms of trustworthiness from trustee to trustor, and a gray trusting-action arrow from trustor to trustee. Above them sits a contextual-properties box listing temporal, social, and institutional embeddedness; below sits an intrinsic-properties box listing ability and motivation; dashed lines show both feeding into the signals.
:width: 100%

The mechanics of trust, after Riegelsberger, Sasse, and McCarthy (2005). Contextual properties give a trustee reasons to behave well; intrinsic properties make it able and willing. The trustor never sees the properties directly, only the signals that carry them.
:::

The properties come in two families. *Contextual properties* are pressures from the situation that give the trustee a reason to behave well, whatever their character. Riegelsberger and colleagues name three. **Temporal embeddedness**: we will deal with each other again, so cheating me today costs you my business tomorrow. Economists call this the "shadow of the future." **Social embeddedness**: others will hear how you treated me, so your reputation is on the line with every exchange. **Institutional embeddedness**: rules, contracts, and sanctions stand behind the transaction, whether that means a regulator, a court, or a platform that can ban you.

*Intrinsic properties* live inside the trustee. **Ability**: can they actually do the thing? The most honest surgeon in the world is not trustworthy for your operation if she trained as an accountant. **Motivation**, including benevolence: do they *want* to do right by you, even when nobody is watching, because they care or identify with you or hold values that say so?

Look at the platforms you use through this lens and they snap into focus as embeddedness machines. eBay's feedback system took social embeddedness, which is to say village gossip about who cheats, and rebuilt it at planetary scale, so that a seller in Osaka has a reputation you can read in Ohio. Airbnb layers all three: hosts want your repeat business (temporal), reviews follow them forever (social), and the platform holds payment in escrow and mediates disputes (institutional). A verified badge on a social platform is a claim of institutional embeddedness: *someone checked*. These designs let strangers borrow the trust machinery of small towns without the small town.

## Symbols, Symptoms, and the Art of Faking It

This next distinction will make you a sharper reader of every interface you'll ever see. Signals, Riegelsberger and colleagues note, come in two kinds, and the difference is how hard they are to fake.

*Symbols* are signals created specifically to advertise trustworthiness: trust seals, padlock icons, verified badges, professional web design, a reassuring privacy pledge. Their weakness is built into their nature. Because they exist only to signal, anyone who can copy the signal gets the trust without the property. A scam site can display a security seal it never earned. *Symptoms*, by contrast, are byproducts of actually having the property. Thousands of detailed reviews accumulated over years are a symptom of a real track record; they are expensive to counterfeit precisely because the cheapest way to get them is to actually serve thousands of customers. A pattern of publicly fixing your mistakes is a symptom of accountability. As a rule of thumb: the more a signal costs to produce dishonestly, the more you can lean on it.

:::{warning} The Verified Badge Problem
When a signal becomes valuable, faking or buying it becomes an industry. Reviews can be purchased in bulk, follower counts inflated, "verification" sold as a subscription perk, and AI can now generate warm, error-free, professional-looking text for pennies, though that text was once a decent symptom of a real organization behind the website. Every trust signal you rely on is a target. The question to keep asking is not "does this look trustworthy?" but "what would it cost a bad actor to make it look exactly this way?"
:::

## Trust Is Yours; Trustworthiness Is Theirs

One distinction ties this whole section together, and the course will lean on it for weeks: *trust* is something the trustor gives; *trustworthiness* is something the trustee has. They are different things, and they can come apart in both directions. You can trust the untrustworthy. That is every scam victim's story: trust flowing toward well-crafted symbols with no properties behind them. You can also withhold trust from the trustworthy, dismissing the reliable news source or ignoring the accurate diagnosis, which quietly costs societies just as much.

The goal, for a person or a society, is not maximum trust. It is *well-placed* trust: trust that tracks trustworthiness. That reframing matters because an enormous amount of design effort in the information society goes into manufacturing the feeling of trust, and the feeling is profitable whether or not it is deserved. A designer can use Riegelsberger's framework to help honest actors show their real properties, or to help dishonest ones fake the signals. Same knowledge, opposite ethics. Which use you are looking at, in any given interface, is one of those questions this course keeps teaching you to ask: who benefits from this feeling being produced in you?

Keep the toolkit from this section within reach: trustor and trustee, contextual and intrinsic properties, symbols and symptoms, trust versus trustworthiness. Everything that follows is this machinery under new stress.

## Up Next

We built the framework on human strangers: sellers, hosts, drivers. But your most frequent counterpart these days may not be human at all. What happens to the mechanics of trust when the trustee is a machine that has ability without motivation, fluency without accountability? Continue to [Trusting Machines](trusting-machines.md).
