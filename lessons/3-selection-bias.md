# Lesson 3

## Selection Bias

* Randomization prevents selection bias at baseline but is powerless to prevent
  it due to post baseline factors like differential loss to follow-up (i.e.
  censoring) or other missing data issues
* Randomization prevents selection bias under the null at baseline as long as
  randomization if the first step performed. However, selection bias can still
  occur due to factors that happen after baseline. In theory, the only way to
  eliminate the possibility of selection bias after the fact, would be to
  randomize selection itself and this is not practical.
 
**Methods of controlling for selection bias**

* Avoid selection
* Smart selection
* Adjust for selection bias
  - Stratification (pooling stratum), but it doesn't always work 
  - Inverse probability weighting (IP weighting) - probability of follow-up.
    This can correct for selection bias in all cases, but requires knowledge on
    true causal DAG and information on all the variables

**Selection bias for smoking on dementia**

* Depletion of susceptibles caused by competing event

## Additional Resources

### Causal Inference textbook

**Chapter 8**: Hernán MA, Robins JM.
[Causal Inference]().
Boca Raton: Chapman & Hall/CRC, 2018

* This chapter defines selection bias and reviews methods to adjust for it.

### Smoking and Dementia

Hernán MA, Alonso A, Logroscino G.
[Cigarette smoking and dementia: potential selection bias in the elderly](http://journals.lww.com/epidem/Fulltext/2008/05000/Cigarette_Smoking_and_Dementia__Potential.17.aspx).
Epidemiology 2008; 19(3):448-450

* This paper reports results from a systematic review of prospective studies on
  smoking and the incidence of Alzheimer’s disease and dementia and discusses
  the potential role of selection bias in explaining their findings. 

### To learn more

Snoep JD, Morabia A, Hernández-Díaz S, Hernán MA, Vandenbroucke JP.
[A structural approach to Berkson’s fallacy and a guide to a history of opinions about it](https://academic.oup.com/ije/article/43/2/515/680398/Commentary-A-structural-approach-to-Berkson-s).
International Journal of Epidemiology 2014; 43(2): 515-521

* This commentary uses causal diagrams to describe the structure of Berkson’s
  fallacy, explains how to avoid it, and reviews a history of opinions about
  it.

Appendix of Hernán MA, Hernández-Díaz S, Robins JM.
[A structural approach to selection bias](http://journals.lww.com/epidem/Fulltext/2004/09000/A_Structural_Approach_to_Selection_Bias.20.aspx).
Epidemiology 2004; 15(5):615–625.

* This paper provides examples of selection bias in epidemiologic studies and
  discusses the importance of a structural classification of bias to
  distinguish confounding and selection bias. The Appendix further explores
  causal and associational risk ratios, hazard ratios as effect measures, and
  effect modification and common effects in causal diagrams.
