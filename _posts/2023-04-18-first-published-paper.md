---
layout: post
title: Yet another model of decision-making?
subtitle: well, yeah, but mine is cool!
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [PhD,writing, paper,decision-making, modelling]
comments: true
---

tl;dr: I created a non-linear model of decision-making where the rate of evidence accumulation at each time depends on the starting point. We showed that it fits data better than the DDM, that it is computationally simpler than other non-linear models (like OU processes) and that it could account for other effects, such as time that passes, in a more efficient way than the DDM.

tl;dr (shorter): my covid side project is now published and can be found here: [https://www.nature.com/articles/s41598-023-32841-9](https://www.nature.com/articles/s41598-023-32841-9)

Decision-making is a main aspect of everyday life: deciding what to have for dinner, which outfit to wear to make your ex jealous, where to study, whom to marry are all life-altering decisions that impact our survival (from a biological and societal point of view). It is no surprise that psychology, neuroscience and economy have tried to theoretize it.

In neuroscience and psychology (also economy, but with additional constraints), scientists are particularly interested in perceptual decision-making, which are the decisions made in reaction to an element perceived in the environment: stopping at a red traffic light, picking a raspberry tart instead of a lemon pie (in both cases, this is the only acceptable decision to be made). Even in these seemingly simplistic situations, people do make mistakes sometimes, resulting in the cataclysm of tasting dish soap instead of the sour sweetness of the red berry of heaven. 

How do we make these decisions? It is widely accepted that the brain gathers proofs (or "accumulates evidence", as we say in scientific papers) until you decide that enough evidence is collected in favor of one alternative to opt in favor of that option (i.e. until a boundary is reached). In classical models, evidence is accumulated at a steady pace. This is what we call the Diffusion Decision Model (or DDM). However, some scientists, including me, have found it a little odd that this should be the case. Why then do we respond faster when we correctly anticipate events? Of course, if we start already close to the boundary, the responses become faster. However, past research has shown that the rate of evidence accumulation is also likely to change upon expectation. 

So we developped the nl-DDM (understand non-linear DDM), in which the shape of the evidence accumulation rate depends on where we start accumulating evidence. More precisely, the closer to the boundary we start, the easier it will be to collect evidence in favor of the corresponding alternative. To give an analogy, it is similar to that phenomenon when you are convinced that a specific color is very fashionable, and you see it more and more around you, convincing you even more that it is indeed in fashion. And guess what? Responses times are indeed better predicted by the nl-DDM than by the DDM! We also compared it to other models, and ours is more efficient (understand: you need less parameters or less fine tuning to account for data). 

Another problem with more classical models is that they consider variability, which is the way that our responses vary across people and across repetitions made by the same person, as noise. However, there are many explainable phenomena that can account for variations of responses: tiredness, arousal, motivation, training... Therefore, we looked at how we could consider one of these parameters with the nl-DDM compared to the DDM. The parameter we chose was the timespent doing the experiment: we expect that people are better trained, but more tired and less motivated at the end of the experiment compared to the beginning, and that should impact the decision-making policy in the brain. And again, the nl-DDM captured this effect better than the DDM, and with fewer and fewer parameters than the DDM as you increased the precision of the time scale used.

In conclusion, this model could explain better why sometimes you would pick the wrong tart or why you got infatuated with very debatable people. And more seriously, this (objectively pretty cool) project would help us better understand the decision-making processes and incorporate many more influences beyond the sole presence of an external signal prompting you to react.

To learn more about this project (that I started completely on the side during Covid and that became one of the main studies of my PhD), you can read the article here: [https://www.nature.com/articles/s41598-023-32841-9](https://www.nature.com/articles/s41598-023-32841-9)
