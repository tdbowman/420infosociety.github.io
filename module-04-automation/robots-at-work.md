# Robots at Work

> In robotics, the hard problems turn out to be easy, and the easy problems turn out to be hard.

## 🎯 In This Section

- Get the real numbers on industrial robots worldwide, straight from the industry's own census
- Understand why robots thrive in structured environments and stall in unstructured ones
- Meet Moravec's paradox: why chess fell before laundry-folding
- Watch the humanoid moment with both eyes open, and learn why a demo is not a deployment
- See what happens when foundation models become robot brains, and why the honest survey literature is more cautious than the hype

## Half a Million New Coworkers a Year

Start with the census. The International Federation of Robotics (the industry's own trade association, which is worth remembering as you read) reports in its *World Robotics 2025* release that 542,076 industrial robots were installed worldwide in 2024, and that the global operational stock has roughly doubled over the past decade. Half a million new machine workers a year, joining millions already bolted to the world's factory floors. This is not a forecast or a demo reel. It is installed, purchased, working capital.

They went overwhelmingly into the classic strongholds: automotive plants and electronics factories, doing welding, assembly, painting, and the endless lifting and placing of parts. Warehouses and logistics operations are the fastest-rising site. What these places share matters more than what they make, and it brings us to the most useful idea in this section.

Two cautions before we go on. First, a doubling of robot stock over a decade is real growth, but the number is silent on a lot: nothing about jobs lost or gained, nothing about which countries and industries the machines concentrated in, nothing about how often they sit idle. A census counts bodies, not consequences. Second, remember who is speaking. The IFR exists to promote robotics, so "demand doubles" is a fact and a sales brochure at the same time. Neither point makes the numbers wrong. It makes them numbers to think *with* rather than conclusions.

## Structure Is a Robot's Best Friend

Robots pack automotive plants but not restaurant kitchens, and the reason is not that welding is easier than cooking. A factory can be *engineered around the robot*. A kitchen cannot.

Roboticists distinguish *structured environments*, where the world is arranged to be predictable, from *unstructured* ones, where it isn't. In a structured environment, every part arrives at a known position, in a known orientation, at a known time; lighting is controlled; humans are fenced out or carefully choreographed. Under those conditions a robot's weaknesses (brittle perception, no ability to improvise) never come up, while its strengths in speed, precision, and endurance compound around the clock. The open secret of industrial robotics is that its triumphs are as much achievements of *environment design* as of machine intelligence. We did not build robots that could handle the factory. We rebuilt the factory so robots could handle it.

Step outside the fence and everything inverts. A hotel room, a hospital corridor, a construction site, your kitchen: cluttered, changing, full of soft and slippery and irreplaceable things, and full of people who do not follow choreography. Here the robot needs exactly what the structured world let it skip: rich perception, real-time judgment, and above all *dexterity*, the fine manipulation of objects that vary. Hands turn out to be the crown jewels of evolution. This is **Moravec's paradox**, one of the oldest lessons in AI. The abstract feats we treat as signs of intelligence, like chess and calculus, proved easy for machines, while the sensorimotor skills any toddler has (grasping, balancing, telling a sock from a shadow) remain brutally hard. Reasoning is recent and shallow in our species. Perception and manipulation rest on hundreds of millions of years of evolutionary engineering, so we automated the new stuff first.

| | Structured environments | Unstructured environments |
|---|---|---|
| **Examples** | Assembly line, bottling plant, fulfillment center aisle | Kitchen, hospital room, construction site, sidewalk |
| **The world is...** | Arranged for the machine: fixed positions, controlled light, fenced humans | Arranged for humans: clutter, variation, surprise |
| **Robot performance** | Superhuman speed, precision, and endurance | Slow, brittle, error-prone |
| **Hard part** | Up-front engineering of the environment | Perception, dexterity, judgment in real time |
| **Status today** | Solved and scaling; the IFR's half million a year live here | The research frontier, where the Gu et al. survey lives |

## The Humanoid Moment

Which brings us to the machines everyone is actually talking about. This week's 60 Minutes segment shows Boston Dynamics' Atlas learning factory work: a human-shaped robot walking, crouching, lifting, placing, practicing a job. It is astonishing footage, and you should let yourself be astonished. Then you should start asking questions.

Why build a robot shaped like a person at all, when a bolted-down arm is faster and a wheeled cart is more stable? The bet is environmental. Our built world (stairs, doorways, shelves, tools, vehicles) is shaped around the human body, so a machine with that body could in principle slot into any workplace *without* the expensive re-engineering that classic automation requires. The humanoid is an attempt to skip the structured-environment bargain. Instead of rebuilding the world for the robot, build the robot for the world.

In principle. This week's Gu et al. survey, written by researchers in the field rather than marketers, walks through how humanoids actually work and is admirably blunt about what remains unsolved. Locomotion and whole-body control have advanced enormously, but dexterous manipulation lags far behind. Hardware imposes limits no algorithm can wish away: actuators, hands, batteries, the sheer energy cost of staying upright. Skills trained in simulation degrade when they meet messy reality. Operating safely at speed alongside humans is still an open problem. Read their challenges section carefully. It is the most honest document in this week's materials, and that's because it is a list of things that do not yet work.

:::{warning} Demo ≠ Deployment
A demo shows the best take. A deployment survives the worst day. When you watch any robot video, including this week's, ask a few things. How many takes? Is it teleoperated, scripted, or autonomous, and does the video say? How structured is the "unstructured" environment, and who placed those objects? What happens at hour 10,000, when parts wear and lighting changes and no engineer is standing by? What does it cost, and what does the maintenance contract look like? The distance between a demo and a deployment is measured in the boring variables the camera never shows. The IFR's half million robots a year are deployments. The humanoid moment, so far, is mostly demos. That doesn't make it fake. It makes it *early*.
:::

## Foundation Models Get Bodies

The humanoid moment is happening *now* rather than a decade ago for reasons that are only partly mechanical. The new ingredient is the technology you met in Module 3: foundation models. The same class of large models that learned language and vision at scale is now being wired into robots, as Gu et al. survey, to interpret spoken instructions, recognize arbitrary objects, and propose plans of action. The hope is that instead of hand-programming every task, a robot could inherit general knowledge about the world from its model and adapt on the fly. That would be the full move to the right end of last section's spectrum.

It's a powerful idea, and early results are real. But carry Module 3's central lesson into the physical world with you: fluency is not reliability. A language model that hallucinates produces a wrong sentence. A robot controller that hallucinates produces a wrong *motion*, with a payload, near a person. Text generation forgives errors, since you can shrug and regenerate; physics does not. A system that is right 95% of the time is impressive in a chatbot and unacceptable in a machine handing you a chainsaw. Closing that gap between mostly-right and dependably-safe is not a detail. In robotics it is most of the problem. The honest summary of the field is that foundation models have given robots much better *understanding* than they had five years ago, while the old bottlenecks of dexterity, dependability, safety, and cost still guard the door to deployment.

So we have half a million real robots a year thriving inside structured environments, plus a thrilling, unproven push to escape the fence: machines that finally move like us but aren't yet trusted to work beside us. Now we can ask the question that was waiting underneath all of it. When people watch Atlas practice a factory job, most are not wondering about actuator torque. They are wondering about themselves.

## Up Next

Fear of automation is older than the robots, older than the assembly line, older than the word "technology" in its modern sense. In [Automation Fears and Facts](automation-fears-and-facts.md), we trace two centuries of that fear, examine what drives it today, and weigh it against what the current evidence shows (and carefully does not show) about AI and work.
