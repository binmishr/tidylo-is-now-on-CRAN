# tidylo-is-now-on-CRAN

The details of the codeset and plots are included in the attached Adobe Acrobat reader (.pdf) file in this repository. 
You need to download the same to view the contents. There are referrals to other contents in BLUE colour also to follow.

I am very pleased to announce that  tidylo, a package for weighted log odds using tidy data principles, is now on CRAN! 

You can now install the released version of tidylo from
CRAN with:

install.packages("tidylo")

A log odds ratio is a way of expressing probabilities, and we can weight a log odds ratio so that our implementation does a better job dealing with different features having different counts. In particular, we use the method outlined in Monroe, Colaresi, and Quinn (2008) for posterior log odds ratios, assuming a multinomial model with a Dirichlet prior. The default prior is estimated from the data itself, an empirical Bayesian approach, but an uninformative prior is also available.

Text analysis is a main motivator for this implementation of weighted log odds, because natural language exhibits an approximately power distribution for word counts with some words counted many times and others counted only a few times. 

Tidy Odd Logs: https://cran.r-project.org/web/packages/tidylo/vignettes/tidy_log_odds.html

Z-scores documentation : https://en.wikipedia.org/wiki/Standard_score

This is a good fit for the weighted log odds approach because some ingredients (like vodka) are much more common than others (like tabasco sauce). Which ingredients are more likely to be used with which type of cocktail glass, using a prior estimated from the data itself? By weighting using empirical Bayes estimation, we take into account the uncertainty in our measurements and acknowledge that we are more certain when we’ve counted something a lot of times and less certain when we’ve counted something only a few times. When weighting by the prior in this way, we focus on differences that are more likely to be real, given the evidence that we have.
