---
title: Statistical dictionary
author: Zbigniew Truchlewski
date: 2020-09-08 19:34:00 +0000
categories: [Stats]
tags: [learning,stats]
toc: true
math: true
pin: true
has-code: true
---

Many statistical terms are daunting. They can quickly become confusing. Even scholars themselves do not agree on what some mean. Try asking what a [p-value is at a conference](https://fivethirtyeight.com/features/not-even-scientists-can-easily-explain-p-values/) or, if you want to see academics practice kung-fu, ask them whether one should use fixed or random effects (safety not guaranteed). Many concepts sound alike and statistical learners end up feeling like reading a Russian novel: who is Alexandra Petrovna again? And what is her relation to Peter Alexandrovitch? Sometimes, it is even hard to distinguish statistical concepts from expletives used by [Captain Haddock](https://en.wikipedia.org/wiki/Captain_Haddock#Expletives). Being a non-native speaker compounds these difficulties. For instance, what does "significant" mean? 

I have not yet come across a statistical book with an accessible glossary. So I hope this simple dictionary (work-in-progress!) will help you (and me) to survive the life statistical. Let me know where I can improve it! Use this dictionary at your own peril.

<!-- "“Unfortunately, I have yet to find a single person who can explain what ignorability means in a language spoken by those who need to make this assumption or assess its plausibility in a given problem.” (The book of Why, p. 281)."

Imai 2010 (focus on NDE - fn 3) vs. Balckwell (focus on CDE)

For controlled direct effect, you can freedom to put values in T and Mediator. Also easier to estimate. See Blackwell. For Natural Direct Effect: need to find a particular value of the mediator.  

total effectc an be nul but mechanism can have effect. Gelato example of Aki. 

“ The applied econometrician is like a farmer who notices that the yield is somewhat higher under trees where birds roost, and he uses this as evidence that bird droppings increase yields. However, when he presents this finding at the annual meeting of the American Ecological Association, another farmer in the audience objects that he used the same data but came up with the conclusion that moderate amounts of shade increase yields. A bright chap in the back of the room then observes that these two hypotheses are indistinguishable, given the available data. He mentions the phrase ”identification problem,” which, though no one knows quite what he means, is said with such authority that it is totally convincing.” ([Leamer, 1983], p. 31). -->

<!-- https://catalogofbias.org/biases/collider-bias/ -->

<!-- https://sgfin.github.io/2019/06/19/Causal-Inference-Book-Glossary-and-Notes/ -->

# Alphabetically

DISTRIBUTIONS FROM BEN LAMBERT, CH. 8. 

* ***Berkson's paradox:***

* ***Bias:*** See [here](https://catalogofbias.org/biases/)

* ***Bias-variance trade-off:***

* ***Collider:*** common effect of two causes. In DAGs where two arrows collide. Thus if you condition on this collider, there can be an association between these two causes even though there is no causal relation between them. This is due to the fact that information circulates from one cause to the effect to the second cause. 
	- This leads to *selection bias*: association between A and Y even if A does not cause Y. NB: a common effect is not necessarily a collider: a common effect can be the effect of a collider. Selection bias also arises in this case if we condition on the effect of a collider.
	- [Example](https://www.youtube.com/watch?v=l_7yIUqWBmE&feature=youtu.be): light switch, electricity and light. If you see light is on, and switch is on, then you automatically learn that there is electricitiy. If there is electricity, and there is no light, you automatically deduce that the switch if off (draw DAG below, link to McElreath).[DAG](#DAG) 


* ***DAG (directed acyclic graph):***

* ***Dendogram:*** a dendrogram is a hierarchical tree that predicts the possible community partitions. Used mostly in cluster analysis. In network analysis can be used to identify communities (Barabasi 2016). <!-- "We can use a dendrogram to extract the underlying community organization. The dendrogram visualizes the order in which the nodes are assigned to specific communities. To identify the communities we must cut the dendrogram. Hierarchical clustering does not tell us where that cut should be. Using for example the cut indicated as a dashed line in Figure 9.9b, we recover the three obvious communities (ABC, EFG, and HIJK)." -->

* ***Fitting:*** REWRITE, from Sololon Kurz: 	Two contrasting kinds of statistical error:
    - overfitting, “which leads to poor prediction by learning too much from the data”
    - underfitting, “which leads to poor prediction by learning too little from the data” (p. 166, emphasis added)

* ***Hierarchical model:*** also called "multilevel models". 

* ***Likelihood:*** In Bayesian statistics, the probability model. In Bayes' formula, $p(data|theta)$. More simply, likelihood is a probability distribution. Difference between likelihood and probability: in Bayes we used the word likelihood because the data is fixed (Lambert 4.4). Likelihood does not necessarily sum up to one, while probability does.

* ***Moments of sample:*** to fit the first two moments (the mean and the standard deviation, respectively) of the sample.
	- See also: mean, standard deviation, skewness, kurtosis. 

* ***Probability:*** Does probability exist? If yes, what is it? It's surprising to learn that there is no agreement on this. Some people like Bruno de Finetti claimed that probability does not exist - at least not objectively. It's in the eye of the beholder: many people have different probabilities of an event depending on their state of knowledge. Others defined probability base on notions such as a set of events (Kolmogorov), a long run frequency (Venn), or based on all possible outcomes of an experiment (Gosset). 
	- Seel also: The Lady Tasting Tea, Ch. 29. 

* ***p-value:*** See [here](https://statsepi.substack.com/p/no-you-cant-explain-what-a-p-value)

* ***random sample:*** “Combining these two assumptions, we say in statistical language that our data sample is composed of independent and identically distributed observations, or alternatively we say that we have a random sample.” Excerpt From: Ben Lambert. “A Student’s Guide to Bayesian Statistics”. Apple Books. 

* ***Sensitivity analysis:*** Usual done in several ways: 1/ Show how estimates change as we add controsl. Why this is bad? 2/ Fom Imai et al 2011 p. 774 L: Sensitivity analysis provides one way to do this. The goal of a sensitivity analysis is to quantify the exact de- gree to which the key identification assumption must be violated for a researcher’s original conclusion to be re- versed. If inference is sensitive, a slight violation of the assumption may lead to substantively different conclu- sions. Although sensitivity analyses are not currently a routine part of statistical practice in political science (but see Blattman 2009, and Imai and Yamamoto 2010), we would argue that they should form an indispensable part of empirical research (Rosenbaum, 2002b).

Several schools: Stability of Coefficinet visual or table-based (classic, Traunmeuller? Adolph), Bounds (Leamer, Young, Sala-i-Martin), and unobservable confounders (Blackwell, Oster). 

* ***Significance:*** distinction between statistical and substantive
	- See also: p-value. [####Significance]

<img src="https://zgtruchlewski.github.io/assets/img/sample/Stargazing_BW_Negative.png" width="426" height="281" />

* ***Sequential ignorability:*** 

* ***Sharp bound:*** partially identification of MAnski, mathematically guaranteed bound of ATE vs. Confidence Interval due to uncertainty of sample. 

* ***Skewness:*** The skewness and kurtosis (skewness measures how symmetric a distribution is, and kurtosis quantifies how fat its tails are; these relate to the third and fourth moments of a distribution, respectively).”


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

Link for the DAG code

```R
library(dagitty)
```

The figure on statisitical vs. substantive significance can be replicated with the following `R` code:

```R
### Data 
x1 <- seq(-.2,.6,length=1000)
y1 <- dnorm(x1,mean=.2, sd=.1)
x2 <- seq(1,1.8,length=1000)
y2 <- dnorm(x2,mean=1.4, sd=.1)
x3 <- seq(-1,2,length=1000)
y3 <- dnorm(x3,mean=0.8, sd=.5)

### Plot 

# Zero line
segments(0,-.2,0,4, lwd=2, col="gray60", lty=2)

# Densities
plot(x2,y2, type="l", xlim=c(-1, 2), ylim=c(0, 5), lwd=1, axes=FALSE, 
	xlab="",ylab="", xaxs="i", yaxs="i")
	# # 95% CI shaded
	x2p <- seq(1.2,1.6,length=1000)
	y2p <- dnorm(x2p,mean=1.4, sd=.1)
	polygon(c(1.2,x2p,1.6),c(0,y2p,0),col=col.alpha("gray",0.3), border=NA)

lines(x1,y1, type="l", xlim=c(-1, 2), yaxt='n', lwd=1)
	# # 95% CI shaded
	x1p <- seq(0,.4,length=1000)
	y1p <- dnorm(x1p,mean=0.2, sd=.1)
	polygon(c(0,x1p,.4),c(0,y1p,0),col=col.alpha("gray",0.3), border=NA)

lines(x3,y3, type="l", xlim=c(-1, 2), yaxt='n', lwd=1)
	# # 95% CI shaded
	x3p <- seq(-.2,1.8,length=1000)
	y3p <- dnorm(x3p,mean=0.8, sd=.5)
	polygon(c(-.2,x3p,1.8),c(0,y3p,0),col=col.alpha("gray",0.3), border=NA)

axis(1, xlim=c(-1, 2), at= cbind(-1, -0.5, 0, .5, 1, 1.5, 2), 
	labels=c("-2", "-1", "0", "1", "2", "3", "4"))

# Add text
text(-.775, 4.25, "Statistically significant?")
text(-.775, 4.5, "Substantively significant?")

text(.15, 4.25, "Yes") 
text(.15, 4.5, "No")
text(.2, 1, "Precision")

text(1.35, 4.25, "Yes") 
text(1.35, 4.5, "Yes")
text(1.4, 1, "Ooomph &\nprecision")

text(0.75, 4.25, "No") 
text(0.75, 4.5, "Yes")
text(0.8, .5, "Ooomph")
```