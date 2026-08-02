# Information Theory and Its Limits

> "The fundamental problem of communication is that of reproducing at one point either exactly or approximately a message selected at another point."
> - Claude Shannon, *A Mathematical Theory of Communication* (1948)

## 🎯 In This Section

- Understand information as *uncertainty reduction*, measured in bits
- Follow a message through Shannon's model: source, encoder, channel, noise, decoder, destination
- See how noise and redundancy explain everything from "u up?" to error-correcting codes
- Grasp why excluding meaning was both a stroke of engineering genius and a philosophical time-bomb
- Trace the direct line from Shannon's 1948 paper to compression, networks, and the token streams of large language models

## A Bet You Can't Lose (Much On)

Start with a game. I flip a fair coin behind my back and you have to find out how it landed. How many yes-or-no questions do you need? One: "Heads?" Now I pick a card from a shuffled deck. How many yes-or-no questions to identify it? If you're clever ("Is it red?" "Is it a heart?"), you can corner any card in six questions, splitting the remaining possibilities in half each time.

That game *is* information theory. In 1948, Claude Shannon, a mathematician at Bell Labs, proposed that information is not about content, importance, or truth. Information is the reduction of uncertainty, and it can be measured by how many yes-or-no questions it resolves. One question's worth of uncertainty, one halving of the possibilities, is one *bit*. The coin flip carries one bit. The card carries about six. A message that tells you something you already knew for certain carries zero bits, no matter how long it is.

It is a strange idea, and a powerful one. A wedding invitation, a stock price, a genome, and a cat video become the same kind of thing: sequences of resolved uncertainty, countable in bits. Before Shannon, engineers building telephone and telegraph systems had no general way to ask "how much information is this line carrying?" or "what's the theoretical limit of this channel?" After Shannon, they did. He called the average uncertainty of a message source its *entropy*, borrowing a term from physics, and proved theorems about exactly how much any channel could carry and how well any message could be compressed. Every design decision in the digital world since has been made inside the walls of those theorems.

## The Diagram That Built the Digital World

Shannon compressed his whole framework into one diagram, and it is worth learning cold, because you will see its skeleton inside every communication system you ever encounter.

:::{figure} images/shannon-model.svg
:name: shannon-model
:alt: A flow diagram showing Shannon's communication model as five boxes connected by left-to-right arrows (information source, encoder, channel, decoder, and destination), with a noise source pushing an arrow up into the channel from below, and a dashed callout above the diagram noting that meaning is deliberately outside the model.
:width: 100%

Shannon's model of communication. A message travels from source to destination through encoding, a noisy channel, and decoding. Meaning never appears in the diagram, by design.
:::

An *information source* selects a message: your voice, your text, your photo. An *encoder* (Shannon called it the transmitter) converts the message into signals suited to the channel, turning sound waves into electrical patterns or letters into binary. The *channel* is the physical medium, whether copper wire, radio spectrum, or fiber optic cable. Along the way, *noise* intrudes: static, interference, cosmic rays flipping bits, a bad Wi-Fi day. A *decoder* reconstructs the message from the corrupted signal, and the *destination* (the person or machine at the far end) receives it.

The villain of the story is noise, and Shannon's hero is *redundancy*: extra, technically unnecessary structure that lets a receiver recover a message even when parts are damaged. English is roughly half redundant, which is why "u up?" survives the loss of most of its letters and why you can read a sentence with a typo without noticing. Engineers add redundancy deliberately. Error-correcting codes are why a scratched DVD still plays and why data returns intact from spacecraft billions of miles away. Compression is the same insight run backward: squeeze out redundancy the receiver doesn't need. When your phone streams video, it is doing Shannon arithmetic millions of times per second, spending exactly as much redundancy as the noise requires and not a bit more.

## The Brilliant, Deliberate Omission

Now look back at the diagram and notice what is *not* in it. Nowhere does it ask whether the message is true. Nowhere does it ask what the message means, or whether the destination understood it, cared about it, or was changed by it. Shannon said so explicitly and up front: the semantic aspects of communication (the meaning) were irrelevant to the engineering problem he was solving.

The omission was deliberate, and it was the move that made everything work. By refusing to model meaning, Shannon made his theory perfectly general: the same mathematics handles Morse code, television, DNA sequencing, and TikTok, precisely because it never has to know what any of it is *about*. Imagine trying to build the internet on a theory that required routers to first determine what each packet meant. The engineering triumph of the last seventy-five years rests on that abstention.

But this week's Tredinnick reading calls the bluff that the rest of us have quietly gone along with. Shannon's theory was so successful that "information," a word that once implied someone being *informed* about something, drifted into meaning "whatever the pipes carry." Tredinnick surveys how the mathematical theory became the default backdrop against which every other theory of information has had to define itself, and how philosophers like Luciano Floridi and Mark Burgin, along with the semiotic tradition, have tried to put back what Shannon set aside. That is next section's story. For now, hold the tension: the theory that built the information society cannot, even in principle, tell you whether anything in the information society is true, meaningful, or worth knowing. A perfectly transmitted lie and a perfectly transmitted cure for a disease are identical to the model.

:::{warning} Don't Confuse the Measure With the Thing
"Information" in Shannon's sense is a property of *signals and probabilities*, not of knowledge. A random string of characters has maximal Shannon entropy, since every character is a surprise, yet it tells you nothing about the world. When someone says a hard drive "contains 2 terabytes of information," they are speaking Shannon. When someone says a whistleblower "revealed explosive information," they are speaking a language Shannon's theory deliberately does not speak. Much confusion in debates about data, media, and AI comes from sliding between the two without noticing.
:::

## Shannon's Grandchildren: From Modems to Language Models

A seventy-five-year-old engineering paper opens a course on the information society because you have never used a digital technology that isn't downstream of it. Every file format, every network protocol, every cell tower and satellite link is an application of Shannon's channel and coding theorems. The Khan Academy playlist for this week retraces this arc visually, and it's worth the hour if you want the intuition without the equations.

The newest grandchild is the one this course keeps returning to. A large language model is, at its mathematical core, a machine for predicting the next *token* (a word fragment) given everything that came before. Prediction and Shannon entropy are two faces of the same coin: a model that predicts text well has, in effect, learned the statistical structure of language, exactly the structure Shannon measured when he estimated the entropy of English by having people guess the next letter of a sentence. When ChatGPT streams words onto your screen, you are watching a direct descendant of Shannon's guessing games.

Here the philosophical time-bomb detonates. LLMs inherit Shannon's mathematics and his omission along with it. They are trained on token sequences alone, with no channel back to the world those tokens describe. The model can tell you which sentences are *probable*; it has no native machinery for which sentences are *true*. Better engineering does not straightforwardly fix that. It is the founding abstention of information theory surfacing in a technology that talks. Whether statistical mastery of signals can ever add up to meaning is one of the live questions of our decade, and you cannot think clearly about it without understanding what Shannon left out and why.

## Up Next

Shannon's critics never disputed his mathematics. They disputed his silence. In the next section we meet the counter-tradition: theories that put truth, interpretation, and community at the center of information, plus Hjørland's explanation of why the argument never ends. Continue to [Meaning, Semiotics, and Society](meaning-semiotics-and-society.md).
