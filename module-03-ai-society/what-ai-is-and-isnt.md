# What AI Is (and Isn't)

> The question is not whether machines think, but whether we notice what they actually do.

## 🎯 In This Section

- Distinguish rule-based (symbolic) AI from machine learning, and see why the field changed course
- Learn the difference between training and inference, the two lives of every AI model
- Understand what large language models actually do (predict the next token) and why that single trick produces both dazzling fluency and confident nonsense
- Sort out narrow AI from the hypothetical "general" kind
- Practice the course's signature move: swapping "is it intelligent?" for "what does it do, and for whom?"

## Two Ways to Teach a Machine

In 1997, a computer beat the world chess champion. In 2022, a computer wrote a passable college essay in eleven seconds. Those two milestones feel similar (machine outperforms human), but under the hood they represent almost opposite approaches to building intelligence.

The chess machine belonged to the tradition of **symbolic AI** (sometimes called rule-based AI, or "good old-fashioned AI"). In this approach, human experts write down explicit rules (*if the file is empty, slide the rook; if income exceeds this threshold, apply that tax rate*) and the computer follows them very fast. Symbolic systems run much of the boring, reliable software around you: tax preparation, airline scheduling, the logic in your thermostat. They are predictable, inspectable, and utterly rigid. A rule-based chess program cannot play checkers, and no set of hand-written rules has ever been able to tell a photo of a cat from a photo of a muffin, because nobody can write down what a cat looks like in if-then statements.

**Machine learning** flips the recipe. Instead of writing rules, you gather examples, millions of labeled photos or billions of sentences, and let an algorithm find the patterns itself. The programmer specifies *how to learn*, not *what to know*. Within machine learning sits **deep learning**, which uses layered networks loosely inspired by neurons and thrives on enormous datasets, and within deep learning sits the newest branch: **generative AI**, systems that produce new text, images, audio, and code rather than only classifying inputs. The chatbots you know (ChatGPT, Claude, Gemini) are **large language models (LLMs)**, the text-generating members of this youngest branch.

:::{figure} images/ai-family-tree.svg
:name: ai-family-tree
:alt: A diagram showing artificial intelligence as a large container holding two branches, with rule-based symbolic AI on the left as a sibling of machine learning on the right, and machine learning containing a nested deep learning box that in turn contains a generative AI and large language models box, each level labeled with example systems such as chess engines and tax software for rule-based AI, spam filters for machine learning, face recognition for deep learning, and ChatGPT and Claude for generative AI.
:width: 100%

The AI family tree. "Artificial intelligence" is the umbrella; rule-based systems and machine learning are siblings under it, and each nested box inside machine learning is a narrower, newer, more data-hungry specialty.
:::

Keep this map handy all semester. When a headline says "AI did X," your first question should be: *which* AI? A rule-based scheduling system, a spam filter, and a general-purpose chatbot have almost nothing in common except the label.

## Training and Inference: A Model's Two Lives

Every machine learning system lives twice. **Training** is the expensive, one-time phase: the model churns through massive amounts of data, adjusting billions of internal numerical settings (called parameters) until its predictions stop being terrible. For a frontier LLM this takes months, warehouse-scale computing, and a meaningful fraction of the internet's text. **Inference** is everything after: the trained model, its parameters now frozen, answers your questions. When you chat with an AI, you are not teaching it, and it is not looking things up. It is running the patterns it absorbed during training, one prediction at a time.

This split explains several things students find puzzling. A chatbot doesn't know about last week's news because last week happened after training ended. It doesn't remember your conversation from yesterday because inference doesn't change the model (the app may store your chat history, but that's a filing cabinet, not a memory in the model itself). And the company can't simply "delete the wrong fact," because facts are not stored in any one place. They're smeared across billions of parameters like flavor through a soup.

## The One Weird Trick Behind the Chatbot

So what does a large language model actually *do*? Something almost embarrassingly simple: given a sequence of text, it predicts the next small chunk: the next **token**, roughly a word or word-fragment. That's it. It predicts a token, appends it, and predicts again, thousands of times, until an answer appears on your screen.

The astonishing part is what next-token prediction at sufficient scale turns out to require. To reliably continue the sentence "The capital of France is…," the model must have absorbed geography. To continue a half-written proof, some mathematics. To continue a sad email with an appropriate reply, something that functions like a model of human feeling. Training on trillions of tokens forced these systems to compress a great deal of the structure of human knowledge into their parameters, which is why they can draft your cover letter, debug your code, and explain photosynthesis at three reading levels.

The same trick explains their signature failure. An LLM's job is to produce *plausible* text, and truth is only one ingredient of plausibility. When the model doesn't contain the fact you need, it does not stop and say so. It keeps predicting, and out comes a confident, fluent, well-formatted fabrication: a court case that was never decided, a citation to a paper that doesn't exist. Researchers call this **hallucination**. It is not a bug bolted onto the system; it is the system doing exactly what it was built to do, in a situation where plausibility and accuracy part ways.

:::{warning} Fluency Is Not a Credential
Humans instinctively read confident, articulate prose as a sign of knowledge, a heuristic built for a world where producing fluent text was hard. LLMs break that heuristic completely: their prose is equally polished when they're right and when they're inventing. The polish tells you nothing. Verify anything that matters, especially citations, statistics, and quotes.
:::

## Narrow, General, and the Metaphor Wars

Everything described so far is **narrow AI**: superb within a domain, helpless outside it. The chess engine cannot write essays; the LLM cannot drive your car. **Artificial general intelligence (AGI)**, a system matching humans across the full range of cognitive work, remains a research goal and a marketing term rather than a shipped product, though how close it is stands as one of the most genuinely contested questions in the field (you saw the disagreement firsthand in Module 1's *AI 2027* scenario exercise).

Because the technology is genuinely hard to describe, we reach for metaphors, and metaphors smuggle in arguments. In this week's video, Mustafa Suleyman, a co-founder of DeepMind, proposes that we think of AI as a "new digital species." It's a vivid frame, and coming from someone who builds these systems, worth your attention. But consider what the metaphor does: a *species* is autonomous, evolving, not really anyone's responsibility. A *product*, by contrast, has a manufacturer who can be regulated, sued, and questioned. Each popular metaphor quietly assigns credit, blame, and power somewhere different, whether it's "stochastic parrot," "copilot," "digital mind," or "autocomplete on steroids."

## The Question That Actually Matters

Philosophers have argued for seventy years about whether machines can "really" think, and the argument is genuinely interesting. But for understanding the information society, it is mostly a distraction. A system does not need to understand anything to approve your loan, flag your essay as AI-written, filter your job application, or write a persuasive lie at scale. The effects arrive regardless of what's happening "inside."

So this course trades the metaphysical question for three operational ones, and you should apply them to every AI system you meet from now on: *What does it actually do, reliably and measurably? Who does it work well for, and who bears its errors? And who profits from describing it as more, or less, intelligent than it is?* A hiring model that quietly filters out qualified candidates raises no interesting questions about machine consciousness, and urgent ones about power. Those three questions are the toolkit for the rest of this module, where we watch this technology collide with security, public opinion, and your own relationships.

## Up Next

The same next-token trick that drafts your emails can draft ten thousand personalized phishing emails. In [Promise and Peril](promise-and-peril.md), we look at the dual-use dilemma, and at why the people building AI and the people living with it see such different futures.
