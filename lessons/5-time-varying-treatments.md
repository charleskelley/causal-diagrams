## Lesson 5

### Time-varying Treatments

Time-varying treatements can take a different values for given indvividual
across time.

#### Time-varying Confounding

There may be time-varying confounder when, one L is time-variant and can have
different values at multiple time points, L is present at multiple time points
and can influence treatment and outcome at multiple time points.

#### Treatment-confounder Feedback

Treatment-confounder feedback is when an earlier treatment at a previous time
point effects the cofounder at a subsequent time point.

When there is treatment-confounder feedback, conventional methods for
confounder  adjustment don't work.

#### Bias of Conventional Methods

Conditioning on the time-variant confounder will not work when there is
treatment-confounder feedback because backdoor paths are opened (i.e. selection
bias). As a result, conventional bias adjustment methods cannot be used to
adjust for confounding.

However, G-methods can potentailly be used to adjust for confounding in cases
where there is treatment-confounder feedback. G-methods include:

- Inverse probability weighting
- Standardization (G-formula)
- mathematically equivalent to inverse probability weighting
- G-estimation

## Additional Resources

### Causal Inference textbook

**Chapter 19 & 20**: Hernán MA, Robins JM.
[Causal Inference]().
Boca Raton: Chapman & Hall/CRC, 2018

* Chapter 19 describes key terminology and concepts for causal inference with
  time-varying treatments
* Chapter 20 describes the structure of treatment-confounder feedback and the
  reasons why traditional adjustment methods fail

### Antiretroviral Therapy and Human Immunodeficiency Virus

Ray M, Logan R, Sterne JA, Hernández-Díaz S, Robins JM, Sabin C, Bansi L, van
Sighem A, de Wolf F, Costagliola D, Lanoy E, Bucher HC, von Wyl V, Esteve A,
Casbona J, del Amo J, Moreno S, Justice A, Goulet J, Lodi S, Phillips A, Seng
R, Meyer L, Pérez-Hoyos S, García de Olalla P, Hernán MA on behalf of the
HIV-CAUSAL Collaboration.
[The effect of combined antiretroviral therapy on the overall mortality of HIV-infected individuals](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC2920287/).
AIDS 2010; 24(1):123-137

* This study estimates the effect of combined antiretroviral therapy (cART) on
  mortality among HIV-infected individuals after appropriate adjustment for
  time-varying confounding by indication. 

### To learn more

Robins JM.
[A new approach to causal inference in mortality studies with a sustained exposure period — Application to the healthy worker survivor effect](http://www.sciencedirect.com/science/article/pii/0270025586900886)
[published errata appear in Mathl Modelling 1987;14:917-21].
Mathematical Modelling 1986; 7: 1393-1512.

* In this landmark paper, James Robins introduces a new framework for drawing
  causal inference from complex longitudinal data with time-varying treatments. 

