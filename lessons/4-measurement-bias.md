# Lesson 4

## Measurement Bias

* A and Y are the true measurements of variables A and Y 
* A* and Y* are the observed measurements of A and Y

***Measurement bias or information bias exists when the association between A
and Y is not the same as the association between A* and Y*.***

### Classification of Measurement Error

Four structures of measurement error due to independence and nondifferentiality:

1. Independent nondifferential
2. Dependent nondifferential
3. Independent differential
4. Dependent differential

Independence:

* *Independent errors* are when the measurement error in A is independent of
  the measurement errors in Y. For example, when two different people enter
  data into a database for A and Y at different times and randomly create input
  errors in the values entered for A and Y (i.e. A* and Y*).
* *Dependent errors* are associated when the errors in A and Y share a common
  cause. For example, an after the fact phone interview used to gather
  information on A and Y from a patient after the fact and the patient my
  provide an error in the value in both A and Y (i.e. A* and Y*).

Differntiality

* If the measurement value of a treatment is dependent on the true outcome,
  then the we say the measurement error of the treatment is differential with
  respect to the outcome.

* On the other hand, where the measurement error of the outcome is dependent on
  the true value of the treatment. In this case the outcome measurement error
  is differential with respect to treatment.

### Measurement Bias Control

Statistical Methods

* Usually require a validation sample or measurement of variables with little
  to no errors
* Mostly apply to independent nondifferential cases which are the easiest to
  handle because they have *no bias under the null*

Causal graphs are extremely useful to discover the sources and type of
measurement errors present. So that they can hopefully be corrected for in the
experimental design.

### Naming the Bias

* Confounding
* Selection Bias
* Measurement Bias

Simpson's Paradox is the idea that context is important to dictating the
relationship between variables in a study.

### Why Causal Inference is Hard

Causal graphs help identify issues and discuss strategies to remedy them. Key
issues include:

* Insufficient data
* Wrong population
* Measurement error
* Selection bias
* Confounding

## Additional Resources

### Causal Inference textbook

**Chapter 8**: Hernán MA, Robins JM.
[Causal Inference]().
Boca Raton: Chapman & Hall/CRC, 2018

* This chapter describes biases due to measurement error.

### Hepatitis B Vaccine and Multiple Sclerosis  

Zipp F, et al.  No increase in demyelinating diseases after hepatitis B
vaccination.  Nature Medicine 1999; 5(9): 964-965 

* This letter to the editor reports results from a study of hepatitis B
  vaccination and central nervous system demyelinating episodes. 

Hernán MA, Jick SS.
Hepatitis B vaccine and multiple sclerosis: the jury is still out.
Pharmacoepidemiology and Drug Safety 2006; 15(9):653-655 (Discussion and
Rejoinder Pharmacoepidemiology and Drug Safety 2007; 16(6):705-707)

* This commentary discusses the debated link between hepatitis B vaccination
  and multiple sclerosis.  

### To learn more

Hernán MA, Clayton D, Keiding N.
[The Simpson’s paradox unraveled](https://academic.oup.com/ije/article/40/3/780/746837/The-Simpson-s-paradox-unraveled).
International Journal of Epidemiology 2011; 40(3):780-785

* This paper uses causal diagrams to explain how Simpson’s paradox disappears
  when statistical analysis is appropriately guided by subject-matter knowledge
  of the causal context. 

Hernán MA.
[The hazards of hazard ratios](http://journals.lww.com/epidem/Fulltext/2010/01000/The_Hazards_of_Hazard_Ratios.4.aspx).
Epidemiology 2010; 21(1):13-15.

* This paper discusses the built-in selection bias of hazard ratios and the
  advantages of presenting survival curves in epidemiologic studies. 

