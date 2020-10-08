---
title: Statistical dictionary
author: Zbigniew Truchlewski
date: 2020-09-07 19:34:00 +0000
categories: [Website]
tags: [learning stats]
toc: true
math: true
pin: true
has-code: true
---

Many statistical terms are daunting. They can quickly become confusing. Even scholars themselves do not agree on what some mean. Try asking what a [p-value is at a conference](https://fivethirtyeight.com/features/not-even-scientists-can-easily-explain-p-values/) or, if you want to see academics practice kung-fu, ask them whether one should use fixed or random effects (safety not guaranteed). Sometimes, it is even hard to distinguish statistical concepts from expletives used by [Captain Haddock](https://en.wikipedia.org/wiki/Captain_Haddock#Expletives). Being a non-native speaker compounds these difficulties. For instance, what does significance mean? 

I have not yet come across a statistical book with an accessible glossary. So I hope this simple dictionary (work-in-progress!) will help you (and me) to survive the life statistical. Let me know where I can improve it! Use this dictionary at your own peril.

<!-- https://sgfin.github.io/2019/06/19/Causal-Inference-Book-Glossary-and-Notes/ -->

# Alphabetically

* ***Berkson's paradox:***

* ***Bias-variance trade-off:***

* ***Collider:*** common effect of two causes. In DAGs where two arrows collide. Thus if you condition on this collider, there can be an association between these two causes even though there is no causal relation between them. This is due to the fact that information circulates from one cause to the effect to the second cause. 
	- This leads to *selection bias*: association between A and Y even if A does not cause Y. NB: a common effect is not necessarily a collider: a common effect can be the effect of a collider. Selection bias also arises in this case if we condition on the effect of a collider.

* ***Probability:*** Does probability exist? If yes, what is it? It's surprising to learn that there is no agreement on this. Some people like Bruno de Finetti claimed that probability does not exist - at least not objectively. It's in the eye of the beholder: many people have different probabilities of an event depending on their state of knowledge. Others defined probability base on notions such as a set of events (Kolmogorov), a long run frequency (Venn), or based on all possible outcomes of an experiment (Gosset). 
	- Seel also: The Lady Tasting Tea, Ch. 29. 

* ***Significance:*** distinction between statistical and substantive
	- See also: p-value

<img src="https://zgtruchlewski.github.io/assets/img/sample/StargazingStata3.jpg" width="426" height="281" />

* ***sequential ignorability:*** 

<!-- These are the most important concepts we've seen in McElreath's book and in the course. Try to skim this through and see what sticks and what does not. Also, if you come by better definitions, please do send them to me!

For definitions: Gelman blog, @parkertransparency2016, Gelman about [Rubin](http://www.stat.columbia.edu/~gelman/research/published/rubin.pdf) and @rohrercausation2018. See also scan of Peter John in the folder. 

confirmation bias, inflated effect size, P-hacking, preregistration, replication, selective reporting

See Frank Harrel here: http://biostat.mc.vanderbilt.edu/wiki/Main/CourseBios330Concepts

- *ATE, ATT and all that (LATE):*
- *autocorrelation:* 
- *Bayes factor:* ratio of average likelihoods (see box on p. 192) and also see blog post in Zotero
- *Berkson's paradox:*
- *bias-variance trade-off:* (box on p. 174)
- *censoring:* See also truncation. you decide on which data to report (e.g. only weights under 200kg). truncated differs from censoring in sense that no count of observations beyond the truncation point is known. Censoring: the values of observations beyond the truncation point are lost but their noumber is observed. 
- *Cohen's d:* See this article: https://www.sciencedirect.com/science/article/pii/S1090513818303908#s0090 and reproduce figure 2a. 
- *collider:* common effect of two causes. In DAGs where two arrows collide. Thus if you condition on this collider, there can be an association between these two causes even though there is no causal relation between them. This is due to the fact that information circulates from one cause to the effect to the second cause. This leads to *selection bias*: association between A and Y even if A does not cause Y. NB: a common effect is not necessarily a collider: a common effect can be the effect of a collider. Selection bias also arises in this case if we condition on the effect of a collider.
- *conditioning:* see chapter 7
- *confidence interval:* confidence interval and its many names and [defintions](http://andrewgelman.com/2016/11/26/reminder-instead-confidence-interval-lets-say-uncertainty-interval/)
- *confounder:*
- *collider:*
- *degrees of freedom:* about in the data and in researchers! FOr researchers, see also multiverse. 
- *ecological inference:* see Jeff Gill [here](http://jeffgill.org/papers/EI_oh.pdf)
- *effect of causes vs. causes of effects:* See [Gelman](http://www.stat.columbia.edu/~gelman/research/unpublished/reversecausal_13oct05.pdf)
- *entropy:* 
- *exchangeability:* assumption talked abount in BDA, expand.
- *garden of forking paths:* See Gelman and Loken. see also researcher degrees of freedom in Simmons, J. P., Nelson, L. D., & Simonsohn, U. 2011. False-positive psychology: Undisclosed flexibility in data collection and analysis allows presenting anything as significant. Psychological Science, 20: 1-8. See also Gelman's blog about the analogy between [poker](http://andrewgelman.com/2018/05/21/garden-forking-paths-poker-analogy/#comments) and the Garden of Forking Paths.
- *HARKing:* Kerr, N. L. 1998. HARKing: Hypothesizing after the results are known. Personality and Social Psychology Review, 2: 196-217.
- *Hawthorne effect:* when subjects are aware they are part of an experiments thereby biasing the randomization and so on. See how Instrumental vars can be better here in Schlotter et al. p. 16.
- *Hamiltonian Monte Carlo (HMC):* Also called Hybrid Monte Carlo. See McElreath's blog post. See also Gibbs sampling and Metropolis algorithm.
- *hazard rate:* probability that duration will end after time *t* given that it lasted until time *t*, used in duration models (aka event history analysis). In other words, the hazard rate is the probability that an individual will experience the event at time *t* while the individual is at risk for experiencing the event. See also: survival function, cumulative hazard function. 
- *identification:* ??? ANother difficult question asked by quantitative people who did not listen to the substantial part of your presentation (see also "What about endogeneity?" and "Did you control for X?" [you should make sure that X is necessary and not a collider]). 
- *ignorability:* See Gelman BDA p. 202. study design is called ignorable with respect to the proposed model when the missing data pattern supplies no information and thus the posterior distribution and the posterior predictive distribution of y_mis are entirely determined by the specification of the data model and the observed values. 
- *inference:* talk about stats and hypothesis testing: stats are about drawing inference from samples about a population, contrast with prediction? Also say difference between inference and causal inference
- *instrumental variable:* Define and specify conditions/assumption (exogeneity etc). Bewared that there is an old and new definition in Winship and Morgan. Dunning shows how IV model should be specified after the OLS model (assumption of homogenous partial effects). NB: is IV different in a Rubin POF framework?
- *law of small samples:* From Kahneman THInking Fast and Slow - small samples are more likely to yield extreme results (explain). So when you see a study with a small N you should be skeptical of the results. Explain this more in detail as it is important. 
- *likelihood:* the relative plausibility of an observation (p. 275). Distribution of the data. It's a prior for data. Good definition at 21:00 in lecture W10_18
- *location and scale:* Key parameters of any distribution; that is the mean and the sd.
- *marginal effect:*
- *mediator and mediation analysis:* see ch. 5 on post-treatment bias. When thing between treatment and outcome. See Alan M. Jacob et al 2012 as robustness check (i did not fully understand the mechanism)
- *mnesia:* see ch. 13 and video 16
- *model averaging:* Compare to model stacking. 
- *model stacking:* Compare to model averaging. 
- *moderator:* You want to see whether the main effect of interest changes as a function of another variable. E.g. plant life and life, with water. Also called conditional relation: Need to use interaction effect to see whether moderator amplifyies of reduces mechanisms. See interaction.
- *multiverse:* see [in Zotero](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5122713/) and [here](http://www.stat.columbia.edu/~gelman/research/published/multiverse_published.pdf). 
- *non-centered parametrization:* Ch. 13. 
- *over-dispersion:* See ch. 11 and section 11.3 in particular. Over-dispersion happens when an omitted variable produces additional variance after conditioning on all predictors. In summary, there is more variation than expected. See also under-dispersion.
- *parametric and non-parametric regression:* From reddit, "In a nutshell, parametric regression is: "Here is a model, I think this particular function explains the shape." Whether it's a straight line, a polynomial, some non-linear function. Non-parametric regression is more "Uhh... make it smooth, and let it be wiggly where it needs to be. The function's not important." A typical example of parametric regression is the good ol' linear model, Y = a*X + b. Here, a and b are meaningful parameters. An example of a non-parametric regression is loess (locally weighted polynomials). Sure, you can write down a function that describes loess but it's going to be super complicated and you don't actually care about the coefficients of the basis functions. Another good example is fitting a global polynomial, Y = a1 X + a2 X2 + a3 X3 + ... + b. You might not care so much about all the coefficients, but you've got an explicit model you're fitting, a polynomial. Contrast this with a spline, where you don't really care what's going on as long as it satisfies assumptions about continuity and differentiability. Edit: Ruppert, Wand and Carroll's "Semi-parametric regression between 2003-2007" is a good reference."
- *penalization:* Penalizing more complex models in order to avoid overfitting. 
- *p-hacking:* see also
- *pooling:* Explain James Stein estimator and give original reference. See ch. 12/13 and videos 14-15-16-17. Basically it's regression to the mean. 
- *potential outcomes framework (POF):* Rubin et al. See also and compare to DAG of Judea Pearl.
- *prediction:* Talk about machine learning and contrast with inference: machine learning is about finding generalizable predictive patterns. @jamesintroduction2013, p. 20 Here's the paragraph from the book : An Introduction to Statistical Learning "For example, in a real estate setting, one may seek to relate values of homes to inputs such as crime rate, zoning, distance from a river, air quality, schools, income level of community, size of houses, and so forth. In this case one might be interested in how the individual input variables affect the prices—that is, how much extra will a house be worth if it has a view of the river? This is a inference problem. Alternatively, one may simply be interested in predicting the value of a home given its characteristics: is this house under- or over-valued? This is a prediction problem. " See [this link](https://stats.stackexchange.com/questions/244017/prediction-vs-inference?utm_medium=organic&utm_source=google_rich_qa&utm_campaign=google_rich_qa) 
- *principal stratification:*
- *prior:* Differentiate between fixed - non-adaptive - priors and adaptive priors; also: regularizing priors can be both
- *propensity score:* i.e. restrict analysis to subset of treated and control units with similar distribution of the covariates. Thus propensity score is the probability as a function of the covariates that a unit receives a treatment. 
- *posterior:*
- *regularization:* imposing restrictions on the parameters, to avoid overfitting or unrealistic values of the parameters.
- *researcher degrees of freedom:* see Gelman Loken et al
- *shrinkage:* See ch. 12/13 and videos 14-15-16-17
- *Simpson's paradox:* see box in ch. 10 and lecture [13](https://www.youtube.com/watch?v=rSQ1XMwO_9A&index=13&list=PLDcUM9US4XdM9_N6XUUFrhghGJ4K25bFc) for a good example. Reversal of association is not necessarily good: could be due to confound, or collider! Think about your causal path diagram. You should worry about your Simpson paradox, lot of people make this mistake event in prestigious publications.
- *spurious effect:*
- *stability assumption (SUTVA):*
- *survey:* data collection mechanism whereby... Contrast with experiment, observational study and partial-data patterns. See also stratification and clustering, blocking and selections as well as truncation and censoring. 
- *survival function:* In duration models (aka event history analysis), it's the probability that the duration time will be at least *t*. See also: hazard function, cumulative hazard function. 
- *truncation:* See also censoring. BDA III 8.7 for technical treatment. truncated differs from censoring in sense that no count of observations beyond the truncation point is known. Censoring: the values of observations beyond the truncation point are lost but their number is observed. 
- *under-dispersion*: When the data has less dispersion than expected. This can arise when there is for instance *autocorrelation*. This means when an observation is dependent upon past or future values, the observed counts has often less variation. 
- *variance-covariance matrix:* 
- *zero-inflated outcomes:* When the zeros in a distribution come from different distributions, that is: there are different processes at play of why zero may arise (either nothing happened or the process in question failed to get started). Thus we need a mixture model to model the two or more processes at play. See section 11.2 of McElreath's book and his example of monks not producing manuscripts any given day either because they did not finish it or because they are drunk.
 -->

# Sources


# Code

The figure on statisitical vs. substantive significance can be replicated with the following Stata code:

```

kdensity x1, gen(x_1 h_1)
kdensity x2, gen(x_2 h_2)
kdensity x3, gen(x_3 h_3)

twoway scatteri 0 0 4 0, c(l) msym(none) lpat(vshortdash) lcol(gs10) legend(off) yscale(r(0 5) nofextend noline) ylabel(, nolabel nogrid tlength(0)) xscale(r(-.75 2.25) nofextend) xtitle("`=ustrunescape("\u03B2\u0302")' coefficients with 95% CI", height(6)) ///
|| line h_1 x_1, lcolor(red%50) lpat(dash) || area h_1 x_1 if x_1 > .2 - 1.96*.1 & x_1 < .2 + 1.96*.1, color(red%30) lcolor(red%5) xscale(r(-.75 2.25) nofextend) ///
|| line h_2 x_2, lcolor(orange%50) lpat(dash) || area h_2 x_2 if x_2 > 1.4 - 1.96*.1 & x_2 < 1.4 + 1.96*.1, color(orange%30) lcolor(orange%5) ///
|| line h_3 x_3 if x_3 <= 2.2 & x_3 >= -.7, lcolor(blue%50) lpat(dash) || area h_3 x_3 if x_3 > .8 - 1.96*.5 & x_3 < .8 + 1.96*.5, color(blue%30) lcolor(blue%5)  ///
	legend(off) plotregion(margin(b = 0.1)) ///
	text(4.5 -.8 "`=ustrunescape("\u03B2\u0302")' statistically significant?", color(gs10) placement(e)) ///
	text(4.75 -.8 "`=ustrunescape("\u03B2\u0302")' substantively significant?", color(gs10) placement(e)) ///
	text(4.5 .2 "Yes", color(red)) ///
	text(4.75 .2 "No", color(red)) ///
	text(1 .2 "Precision", color(red)) ///
	text(4.5 .8 "No", color(blue)) ///
	text(4.75 .8 "Yes", color(blue)) ///
	text(0.5 .8 "Ooomph", color(blue)) ///
	text(4.5 1.4 "Yes", color(orange)) ///
	text(4.75 1.4 "Yes", color(orange)) ///
	text(1 1.4 "Ooomph", color(orange)) ///
	text(0.8 1.4 "& Precision", color(orange)) ///
	graphregion(margin(small))
```