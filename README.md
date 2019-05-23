# videosurvey
Analysis of bicycling comfort from a video survey

### Jane's Notes

- Modeling notes 
  - Preliminary linear model (lm.prelim) seems reasonable now, though I think there's still some conflation with divided road and other street features to explain its large positive coef. (Note the divided road coef. fades away in a penalized model.)
  - Preliminary ordered model (ord.prelim) and penalized ordered model (glmcr.prelim) also seem reasonable.
  - Street features basically provide as much information as street id. (This may be because the features essentially reconstruct the names, though the signs of the coefficients make sense so probably not.) 
  - There is a lot of variation in street ratings in general. 
    - Rating distributions are more bimodal (bumps for high and low) than normal, and certain qualities (e.g. don't like biking) seem to flatten out the distribution rather than just moving the mean
    - What explains the tails in the ratings i.e. people who deviate from the general trend? Do people have low-rating and high-rating tendencies (random effects?), and/or are they explained by covariates?
    - Strategy for responders who rated all videos the same, even when shown "between" blocks. (Consider as outliers? Add random effects? Seperate random effects for between and within blocks?)
  

- Data questions
  - Why so many blank entries in the child fields? Why a few "Nones" in addition to zeros? (free-entry fields?)
  - Coding of hh_composition? Conflicting levels selected. (Used rent_share as a hh composition type variable because it has least missing data nad is still somewhat discriptive of household type.)
  - Are blocked bike lanes really blocked? (https://youtu.be/LI0m8h3jVJ4, https://youtu.be/XAKiJ78Z8uE)
  - Exact difference between bike lane, width, shoulder, etc.
  

  
  
