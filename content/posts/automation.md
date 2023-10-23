# Automation and institutional friction

_re Adam Marblestone’s ‘General automation, and Science’_

Adam Marblestone has a thought-provoking [post](https://longitudinal.blog/2023/01/10/general-automation-and-science/) on how much he expects AI to speed up science. He suggests breaking down skills into three types (types 1, 2, and 3). 

Type 1 skills operate in ‘kind’[^1], game-like domains (Chess, Go, etc). Type 2 skills have lots of demonstration data but not obvious score (e.g. writing essays in response to prompts). Type 3 basically refers to everything else (‘wicked’ tasks like e.g. automating a warehouse).

Technical feasibility is a necessary but not sufficient condition for automation. Marblestone’s model is helpful but I think it would benefit from adding a component. I’ll call this _institutional friction_[^2]. 

## Automation often requires institutions to adapt

Back when I was first introduced to deep learning in 2017, the task that was all the rage was predicting whether a given chest X-ray had a tumor. Since diagnosing X-rays is a type 2 skill, it shouldn’t be a surprise that we soon saw [CNNs doing better than radiologists](https://www.nature.com/articles/s41586-019-1799-6.epdf?sharing_token=tdtY2hFG1HJfaboE0pOQ1tRgN0jAjWel9jnR3ZoTv0M5zwPVx5jT4z_z-YkUZTBTbM27UWphyoF6vHoR667kKgqCi8GNWj2oxgaEK9QGM_J8TQydlaQ1nMXBUQrsn-83UCUXO7SuwGbD3s5OuqoOSNwRSESFwlfAfcnd7hRZOIeMaq8iogyPZ0Vk6Nv-wGyC51YHKn17_cu-KM0xhudbaQ%3D%3D&tracking_referrer=www.bbc.com) in [controlled settings](https://www.nature.com/articles/s41746-019-0189-7). Yet we still don’t see deep learning models widely used in clinical diagnosis. I claim that the reasons for this are mostly rooted in institutional friction, rather than technological inadequacy. 

New technologies often face barriers at the legal, social, and organizational level. The software might [not be approved by the FDA](https://radiologybusiness.com/topics/artificial-intelligence/legal-considerations-artificial-intelligence-radiology-and). HIPAA-like privacy may prevent its use in some states. The hospital’s insurance policy might balk at the new technology. Radiologists might refuse to use the new tool.

Before a technology is deployed in a given setting, there has to be consensus among the people who adopt the technology. As evidenced by the examples above, many of their considerations are neither economic nor technological.

## Difficulties facing scientific automation

I gave an example in healthcare because those problems are more legible to me. Marblestone specifically asks about science, so I’ll throw in my two cents. 

**1: Research closer to humans faces more institutional friction.**

The Belmont Report has jurisdiction over research involving human subjects. It demands procedures like getting informed consent before proceeding[^3]. This slows down the rate of research but also puts an absolute cap on research speed; no matter how quickly you submit the IRB, you still need to wait for their approval.

Beyond interactions with internal review boards, which uphold the Belmont Review, human research is legally risky (they might sue you) and finicky (you can’t really control the human living environment very well). 

If experimentation speedup happens in science, I would be quite surprised if human-facing research was at the forefront of that speedup.

**2: Science automation will continue at a similar pace**

The bottleneck is not performing the tasks — there is already heavy machine automation, but ‘metarational’ considerations like “should I run this assay again because it looks weird?” or else the speed of reality (i.e. Zebrafish still take 3 months until adulthood).

I’ll also quote from David Chapman's [writing on the limits to experimental induction](https://betterwithout.ai/limits-to-induction#fn_mark_small):

> Inductive reasoning blesses data as knowledge using formal methods. There is no generally correct way of doing this. A statistical analysis is sound only relative to unavoidable assumptions that cannot be justified rationally; particularly a small-world assumption that limits what factors it considers. Those assumptions must be chosen meta-rationally. This means the “artificial scientist” project is quite different from what is usually imagined, and probably much more difficult. We have much less idea how to automate meta-rationality than rationality...

> Large-scale laboratory automation is already in routine use in pharmaceutical discovery. It is of some value, but no magic bullet. Scaling it up by building or buying way more robots is perfectly feasible, and wouldn’t be expensive on the scale of pharmaceutical research costs. We don’t do that because it wouldn’t help. Robot count is not a bottleneck.

I don’t expect science in general to be automated at a significantly different rate with the rise of ‘paradigm models’ but before putting numbers down, I would want to much more narrowly specify the domain.

## On assuming linearity of progress in speeding up science

I feel pretty suspicious about the following reasoning:

> Let’s say that the coding part of robotics progress is highly **elastic** relative to the above “Best of Existing Skills Instantaneously in Anyone’s Browser” model of AI-induced changes in the world, and speeds by 10x, but that the in the lab hardware testing part of robotics is less elastic and only speeds by 2x. Let’s suppose that that right now these two components — the highly elastic coding part of robotics R&D, and the less elastic in the lab testing part — take about the same amount of time, R. That’s R/2/2 + R/2/10 = 3x speedup of robotics overall... So that means we are perhaps about 10 to 15 years away from a level of lab automation that we’d be expecting otherwise 30+ years from now

In the 60s, mathematician Dietrich Braess discovered that in many cases, adding a road to road network can actually slow down overall traffic flow[^4]. At least [one scientist](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2841822/) found a biological system with a similar phenomenon[^5]. I wonder if something similar could be said of automation and science. In either case, at the very least what Braess’ paradox suggests to me is that there are often complicated nonlinear interactions when networks are altered, and that it is perhaps best to think through a couple of concrete scenarios and backtest the model that Marblestone proposes first before even relying on its logic as intuition.

P.S. 

“it is obviously false that all possible discoveries with given tech level are mapped out- just had a multi-hour conversation about basic experiments in bacterial growth + metabolism that could have been done in the 60s or even the 40s and yet surprisingly have never been done...” see more in [Adam Strandberg's tweet thread](https://twitter.com/strandbergbio/status/1624442492157411330).  
This implies to me that the bottleneck is not the rate of experimentation but something more like 'framing' / 'asking the right questions'. This is akin to what Chapman refers to as 'metarational considerations'.

---

If you liked this essay, feel free to follow my writing updates [here](https://maxlangenkamp.substack.com).

**Acknowledgements**

Thank you to Soren Bouma and Teddy Collins, for the conversation that clarified my point about institutional adaptation. Thank you to Nick Stares for the proofread.

### Notes

[^1]: To borrow from Rittel and Webber’s (1973) terminology in *A General Theory of Planning*↩

[^2]: Note here that I’m loosely using ‘institution’ in the sense described by Elinor Ostrom. Roughly, it can be thought of as a collection of common knowledge rules. This captures everything from the U.S. legal system to the radiologists’ standards at the Mount Sinai hospital. See Ostrom and Crawford’s “A Grammar of Institutions”, or my summary for more detail: maxlangenkamp.me/posts/institution↩ 

[^3]: I’m glad the Belmont report exists. It’s a good example of institutional learning after the inhumane [Tuskegee Syphilis Study](https://en.wikipedia.org/wiki/Tuskegee_Syphilis_Study).↩

[^4]: In the new situation, the Nash equilibrium does not equate to the optimal flow through the network. In reality, I wonder if the increased supply of road leads generally↩

[^5]: The paper I linked uses a corollary of Braess' paradox; that removing an edge can conversely lead to improved network performance.↩