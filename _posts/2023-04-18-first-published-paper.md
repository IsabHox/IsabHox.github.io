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

tl;dr (shorter): my covid side project is now published and can be found here: (https://www.nature.com/articles/s41598-023-32841-9)[https://www.nature.com/articles/s41598-023-32841-9]

Decision-making is a main aspect of everyday life: deciding what to have for dinner, which outfit to wear to make your ex jealous, where to study, whom to marry are all life-altering decisions that impact our survival (from a biological and societal point of view). It is no surprise that psychology, neuroscience and economy have tried to theoretize it.

In neuroscience and psychology (also economy, but with additional constraints), scientists are particularly interested in perceptual decision-making, which are the decisions made in reaction to an element perceived in the environment: stopping at a red traffic light, picking a raspberry tart instead of a lemon pie (in both cases, this is the only acceptable decision to be made). Even in these seemingly simplistic situations, people do make mistakes sometimes, resulting in the cataclysm of tasting dish soap instead of the sour sweetness of the red berry of heaven. 

How do we make these decisions? It is widely accepted that 
