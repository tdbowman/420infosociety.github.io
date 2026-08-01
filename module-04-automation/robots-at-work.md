# Robots at Work

> In robotics, the hard problems turn out to be easy, and the easy problems turn out to be hard.

## 🎯 In This Section

- Get the real numbers on industrial robots worldwide, straight from the industry's own census
- Understand why robots thrive in structured environments and stall in unstructured ones
- Meet Moravec's paradox: why chess fell before laundry-folding
- Watch the humanoid moment with both eyes open — and learn why a demo is not a deployment
- See what happens when foundation models become robot brains, and why the honest survey literature is more cautious than the hype

## Half a Million New Coworkers a Year

Start with the census. The International Federation of Robotics — the industry's own trade association, which is worth remembering as you read — reports in its *World Robotics 2025* release that 542,076 industrial robots were installed worldwide in 2024, and that the global operational stock has roughly doubled over the past decade. Half a million new machine workers a year, joining millions already bolted to the world's factory floors: this is not a forecast or a demo reel. It is installed, purchased, working capital.

Where did they go? Overwhelmingly into the classic strongholds: automotive plants and electronics factories, doing welding, assembly, painting, and the endless lifting and placing of parts — with warehouses and logistics operations as the fastest-rising habitat. What these places share is more important than what they make, and it brings us to the single most useful idea in this section.

Two cautions before we go on. First, a doubling of robot stock over a decade is real growth, but notice what the number *doesn't* say: nothing about jobs lost or gained, nothing about which countries and industries the machines concentrated in, nothing about how often they sit idle. A census counts bodies, not consequences. Second, remember who is speaking. The IFR exists to promote robotics; "demand doubles" is simultaneously a fact and a sales brochure. Neither point makes the numbers wrong — it makes them numbers to think *with*, not conclusions.

## Structure Is a Robot's Best Friend

Why do robots pack automotive plants but not restaurant kitchens? The answer is not that welding is easier than cooking. It is that a factory can be *engineered around the robot* — and a kitchen cannot.

Roboticists distinguish *structured environments*, where the world is arranged to be predictable, from *unstructured* ones, where it isn't. In a structured environment, every part arrives at a known position, in a known orientation, at a known time; lighting is controlled; humans are fenced out or carefully choreographed. Under those conditions, a robot's weaknesses — brittle perception, limited ability to improvise — simply never come up, and its strengths — speed, precision, tirelessness — compound around the clock. The great secret of industrial robotics is that its triumphs are as much achievements of *environment design* as of machine intelligence. We did not build robots that could handle the factory; we rebuilt the factory so robots could handle it.

Step outside the fence and everything inverts. A hotel room, a hospital corridor, a construction site, your kitchen: cluttered, changing, full of soft and slippery and irreplaceable things, and full of people who do not follow choreography. Here the robot needs exactly what the structured world let it skip — rich perception, real-time judgment, and above all *dexterity*, the fine manipulation of objects that vary. Hands turn out to be the crown jewels of evolution. This is *Moravec's paradox*, one of the oldest lessons in AI: the abstract feats we consider signs of intelligence, like chess and calculus, proved easy for machines, while the sensorimotor skills any toddler has — grasping, balancing, telling a sock from a shadow — remain brutally hard. Reasoning is recent and shallow in our species; perception and manipulation rest on hundreds of millions of years of evolutionary engineering. We automated the new stuff first.

| | Structured environments | Unstructured environments |
|---|---|---|
| **Examples** | Assembly line, bottling plant, fulfillment center aisle | Kitchen, hospital room, construction site, sidewalk |
| **The world is...** | Arranged for the machine: fixed positions, controlled light, fenced humans | Arranged for humans: clutter, variation, surprise |
| **Robot performance** | Superhuman speed, precision, and endurance | Slow, brittle, error-prone |
| **Hard part** | Up-front engineering of the environment | Perception, dexterity, judgment in real time |
| **Status today** | Solved and scaling — the IFR's half million a year live here | The research frontier — where the Gu et al. survey lives |

## The Humanoid Moment

Which brings us to the machines everyone is actually talking about. This week's 60 Minutes segment shows Boston Dynamics' Atlas learning factory work: a human-shaped robot walking, crouching, lifting, placing — practicing a job. It is genuinely astonishing footage, and you should let yourself be astonished. Then you should start asking questions.

Why build a robot shaped like a person at all, when a bolted-down arm is faster and a wheeled cart is more stable? The bet is environmental: our entire built world — stairs, doorways, shelves, tools, vehicles — is shaped around the human body. A machine with that body could, in principle, slot into any workplace *without* the expensive re-engineering that classic automation requires. The humanoid is an attempt to skip the structured-environment bargain: instead of rebuilding the world for the robot, build the robot for the world.

In principle. This week's Gu et al. survey — written by researchers in the field, not marketers — walks through how humanoids actually work and is admirably blunt about what remains unsolved. Locomotion and whole-body control have advanced enormously, but dexterous manipulation lags far behind; hardware itself — actuators, hands, batteries, the sheer energy cost of staying upright — imposes limits no algorithm can wish away; skills trained in simulation degrade when they meet messy reality; and operating safely at speed alongside humans remains an open problem. Read their challenges section carefully: it is the most honest document in this week's materials, precisely because it is a list of things that do not yet work.

:::{warning} Demo ≠ Deployment
A demo shows the best take; a deployment survives the worst day. When you watch any robot video — including this week's — ask: How many takes? Is it teleoperated, scripted, or autonomous, and does the video say? How structured is the "unstructured" environment — who placed those objects? What happens at hour 10,000, when parts wear and lighting changes and no engineer is standing by? What does it cost, and what does the maintenance contract look like? The distance between a demo and a deployment is measured in exactly the boring variables the camera never shows. The IFR's half million robots a year are deployments. The humanoid moment, so far, is mostly demos — which does not make it fake, but does make it *early*.
:::

## Foundation Models Get Bodies

The reason the humanoid moment is happening *now*, rather than a decade ago, is only partly mechanical. The new ingredient is the technology you met in Module 3: foundation models. The same class of large models that learned language and vision at scale is now being wired into robots — as surveyed in Gu et al. — to interpret spoken instructions, recognize arbitrary objects, and propose plans of action. Instead of hand-programming every task, the hope runs, a robot could inherit general knowledge about the world from its model and adapt on the fly: the ultimate move to the right end of last section's spectrum.

It is a genuinely powerful idea, and early results are real. But carry Module 3's central lesson into the physical world with you: fluency is not reliability. A language model that hallucinates produces a wrong sentence; a robot controller that hallucinates produces a wrong *motion*, with a payload, near a person. Text generation forgives errors — you can shrug and regenerate — while physics does not, and a system that is right 95% of the time is impressive in a chatbot and unacceptable in a machine handing you a chainsaw. Closing that last gap between mostly-right and dependably-safe is not a detail; in robotics it is most of the problem. The honest summary of the field is that foundation models have given robots vastly better *understanding* than they had five years ago, while the ancient bottlenecks — dexterity, robustness, safety, cost — remain the gatekeepers of deployment.

So: half a million real robots a year thriving inside structured environments, and a thrilling, unproven push to escape the fence — machines that finally move like us, not yet trusted to work beside us. Now we can ask the question that was waiting underneath all of it. When people watch Atlas practice a factory job, most are not wondering about actuator torque. They are wondering about themselves.

## Up Next

Fear of automation is older than the robots, older than the assembly line, older than the word "technology" in its modern sense. In [Automation Fears and Facts](automation-fears-and-facts.md), we trace two centuries of that fear, examine what actually drives it today, and weigh it against what the current evidence shows — and carefully does not show — about AI and work.
