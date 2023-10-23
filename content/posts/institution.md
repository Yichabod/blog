---
title: "What is an institution? Introducing 'A Grammar of Institutions'"
date: 2021-10-16
draft: false
---
# What is an institution? Introducing 'A Grammar of Institutions'

This is part of my series on Ostrom. You can also find the root page [here](https://maxlangenkamp.me/posts/ostrom/).

'How should we define institutions?'<sup id="a1">[1](#g1)</sup> This is a difficult but surprisingly important question; at its core, traditional political science is about the study of institutions. Also, if we want to talk about governance, we need also a vocabulary to discuss the setting where governance takes place. Questions like "most open source software repositories are governed democratically" remain painfully vague without a precise vocabulary.

The debate about how best to define institutions has surged over most of the 20th century, especially among economists and political scientists. One big insight has been the movement away from treating institutions as contained entities towards seeing them as composed of separable elements. Instead of modeling E Corporation as a single agent trying to maximize profit, what if we looked at it as a set of optimal strategies that employees use? What if we modeled E Corporation as a set of norms or rules that guide employee behavior?

The attempt to see institutions as composable have resulted in three major approaches: institutions as equilibria (optimal strategies), institutions as norms, and institutions as rules. I won't go into much detail for any of the three stances<sup id="a2">[2](#g2)</sup>, but instead want to focus on what Elinor Ostrom and Sue Crawford  proposed as a framework that encompasses all three.

What Ostrom and Crawford propose is a grammar of institutions. The core concept here is that we can take any institution and describe it using a series of 'institutional statements'. These 'institutional statements' can capture broadly

### Institutional Grammar

There are five components captured by the acronym ADICO: *A*ttributes, *D*eontics, A*i*ms, *C*onditions, *O*r else.

Take the following statement:

"All villagers must not let their animals trample the irrigation channels during harvest season, or else face a fine."

Attributes: a reference to the entity to whom the institutional statement applies (e.g. *All villagers*)

Deontics: Permissions associated with the syntax. The three categories are "must", "must not", or "may" ("All villagers *must not*...")

Aims: Describes the action or outcome that is allowed or not (*let their animals trample the irrigation channels*)

Conditions: Specifies when, where, how the aim is expected to be realized (*during the harvest season*)

Or else: self explanatory (*or else face a fine*)


### Why is this so powerful?

In my view, Ostrom and Crawford's framework is powerful for three reasons.

First, their institutional grammar acts as an interoperable framework between different previously hard-to-compare ideas. From Robert Axelrod's (1986) evolutionary approach to norms to the social norms off Ullmann-Margalit (1977), there has been a wealth of insight from different authors. This institutional grammar provides a platform of synthesis where these models can be talked about more directly.

Their grammar also allows for new types of analysis. We now have a principled way of concretely answering questions like "what is a decentralized autonomous organization?" and "what is the difference between how Linux and Debian are run?"

Finally, the inventive analogy that Ostrom and Crawford draw between institutional descriptions and linguistics is generative. As they acknowledge, theirs is not the only 'grammar of institutions' that can exist — what other ways can we use ideas of composability to see institutions?

### Caveats

The framework does have two notable limitations that are helpful to keep in mind:
First, identifying institutional statements is hard. Like fish in water, members of an institution are often not able to recognize the strategies, norms, or rules that they are part of. As far as I can tell, there also isn't a systematic way to get capture all of the most important institutional statements.


Second, institutional statements on their own do not explain institutional behavior. For that, we also need a theory of action<sup id="a3">[3](#g3)</sup>. A theory of institutional action allows us to identify how conflicting statements are navigated in practice. Ostrom's broader framework of Institutional Analysis and Development better addresses this.


### Applying the framework

It's been nearly thirty years since their paper came out, and there has continued to be active ongoing work. Siddiki and others (2011), for instance, added the 'object' attribute, making the acronym extra catchy: ADIBCO<sup id="a4">[4](#g4)</sup>.

Others have applied the framework to existing institutions. Watkins and Westphal (2015) apply the framework to understand natural resource management systems. It appears to be the most thorough application of the ADICO framework in a real world setting<sup id="a5">[5](#g5)</sup>.

There is actually a whole research group, the [Institutional Grammar Research Initiative](https://institutionalgrammar.org/) (IGRI), that aims to build on Ostrom and Crawford's work. One of the approaches that has garnered some recent attention is an attempt to use natural language processing to categorize institutional grammars<sup id="a6">[6](#g6)</sup>.



In my next essay, I plan to outline the Institutional Analysis and Development framework and how Ostrom and Crawford's institutional grammar fits into it.


———


<b id="g1">1.</b>  A wordier but more precise version of the question is 'What is a useful way to look at the concepts typically referred to by the word 'institution''? The dictionary is unhelpful here mainly because dictionaries are histories of usage, not prescriptions for helpful frameworks

<b id="g2">2.</b>  Briefly, strategies have attributes, aims, and conditions (AIC). Norms have all those plus a deontic (ADIC). Rules have all five components (ADICO). Here's a quick example, taken from Theesfeld (2010).
- Strategy: When I have dropped off my child at the nursery (C), I (A) put myself
immediately to work (I).
- Norm: All members of the Institute (A) must (D) put their used cups into the
dishwasher (I) when they have finished their tea (C).
- Rule: All users of the tram (A) must (D) buy a ticket (I) before getting on (C) or else
they have to pay a fine of 40 € (O).

<b id="g3">3.</b>  Ostrom continues the analogy with linguistics here: "to explain behavior in institutions, one needs to cimbine the behavior of institutions with a theory of action, just as to understand a language one requires a theory of language use (Chomsky 1965). The theory of action animates the structural model of a situation generated by the grammar and by relevant attributes of a physical world (Popper 1967)"

<b id="g4">4.</b>  I feel like there has to be some better alternatives: COIBAD? DABOIC?

<b id="g5">5.</b>  The paper is called "People Don't Talk in Institutional Statements". Despite that, they argue for the usefulness of the grammar as a whole.

<b id="g6">6.</b>  To that I wish them good luck. Having spent no small effort building out a far simpler NLP-based classifier, I would be very impressed if anything usable materializes in the next five years.
