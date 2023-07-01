# Lesson 2

## Confounding

* Causal diagrams support structural identification of confounding
* Traditionally, non-structural definitions of confounding were used to
  identify confounders

  * L is associated with the treatment
  * L is associated with the outcome conditional on the treatment
  * L is not on a causal pathway from A to Y

We care only about the concept of 'confounding' not the 'confounders'. The goal
is simply to eliminate 'confounding' by any means necessary. If we focus to
closely on identifying 'confounders' we miss the opportunity to eliminate
'confounding'.

* **Confounding is an absolute concept
* **confounder is a relative concept tied to the variables being considered

Surrogate or proxy confounding variables can be used to partially remove
confounding when a variable associated with a common cause is measured, but the
common cause itself is unmeasured and could not be conditioned on.

### Confounding Control

**Methods of controlling for confounding**

>Randomization is gold standard

When only observational data is available:

* Measure enough variables to block all backdoor paths between A and Y
    - Stratification - restrict analysis to certain subsets 
    - Matching - match on the potential confounders in the backdoor path
        - Propensity score based on the potential confounders
    - G-methods - can be used in settings where treatment is time variant
        - Inverse probability weighting
        - Standardization (G-formula) - mathematically equivalent to inverse
          probability weighting
        - G-estimation
* Instrumental variable estimation - only applicable in certain settings (i.e.
  treatment being studied changes over time)

## Additional Resources

### Suggested Readings

#### Causal Inference textbook

**Chapter 7**: Hernán MA, Robins JM.
[Causal Inference]().
Boca Raton: Chapman & Hall/CRC, 2018

* This chapter defines confounding and reviews methods to adjust for it. 

#### Folic Acid and Birth Defects

Hernán MA, Hernández-Díaz S, Werler MM, Mitchell AA.
[Causal knowledge as a prerequisite for confounding evaluation: an application to birth defects epidemiology](https://cdn1.sph.harvard.edu/wp-content/uploads/sites/1268/2014/11/Am.-J.-Epidemiol.-2002-Hernán-176-84.pdf).
American Journal of Epidemiology 2002; 155(2):176–184.

* This paper presents findings from the Slone Epidemiology Unit Birth Defects
  Study, a case-control study on folic acid supplementation and risk of neural
  tube defects.

#### To learn more

Greenland S (2003).
[Quantifying biases in causal models: classical confounding versus collider-stratification bias](http://journals.lww.com/epidem/Fulltext/2004/09000/A_Structural_Approach_to_Selection_Bias.20.aspx). 
Epidemiology 14:300-306

* This paper examines the relative magnitudes of bias from confounding and
  collider-stratification.

Ogburn EL, VanderWeele TJ.
[Analytic results on the bias due to nondifferential misclassification of a binary mediator](https://jhu.pure.elsevier.com/en/publications/analytic-results-on-the-bias-due-to-nondifferential-misclassifica-3).
American Journal of Epidemiology 2012; 176 ( 6): 555-561.

* This paper describes rare mathematical conditions under which adjusting for a
  surrogate confounder may increase bias compared with not adjusting.
