# Lesson 6

## Causal SWIGs

Single world individual graphs (SWIGs) model what would hapen if the
counterfactual existed. SWIGs are effective for causal mapping of time-variant
treatments.

### Counterfactuals

Counterfactuals are the hypothetical outcomes for individuals if they where in
the opposite group, treatment or no treatment, than the group that they are
actually in.

The counterfactual outcomes are often identified using *Y*<sup>a</sup> notation.

* Outcome Y under treatment: *Y*<sup>a=1</sup>
* Outcome Y under no treatment: *Y*<sup>a=0</sup>

There ***is causal effect*** for indvidual X if:

* Y under treatment is different than Y under no treatment for individual X.

There ***is NO causal effect*** for indvidual X if:

* Y under treatment is the same as Y under no treatment for individual X.
 
> ***In observational studies it's impossible to know the value of the
> counterfactual because treatment value and outcome have already 
> occured and cannot be maniputlated post hoc***

### Exchangeability

While you cannot go back in time and measure group level causal effects, you
can use group level causal effect or average causal effect as a proxy.

In the language of causal DAGs, exchangeability means that there are no common
causes of treatment and outcome—assuming no selection bias and no measurement
bias—which is the case under randomization.

In the language of counterfactuals, if the distribution of the average outcome
under treatment and not under treatment is the same for two groups, then
mathematically the counterfactual outcomes are independent of the actual
treatment. 

### Node Splitting

Split the node for treatment A into two parts `A|a=1`, wher `A` is the
treatment and `a=?` shows the the value that the treatment would take under the
intervention of interest.

There are typically two split nodes for SWIGs of a randomized experiment:

1. A|a=1 -> *Y*<sup>a=1</sup> - is the counterfactual outcome Y where everyone
   receives treatment
2. A|a=0 -> *Y*<sup>a=0</sup> - is the counterfactual outcome Y where noone
   receives treatment

In most cases this is collapsed and shown using A|a -> *Y*<sup>a</sup> to
represent both cases in a single SWIG.

The vertical line in the split node blocks the path between the treatment A and
the counterfactual outcome *Y*<sup>a</sup> and therefore creates exchangeability.

### Confounding Revisited

Both causal DAGs and SWIGs can be used to show there is confounding.

### Treatment Strategies

Sequential exchangebility - exists if, for time-variant treatments, there is
exchangeability at all times.

### Dynamic Strategies 

* **Static strategies** do not change based on feedback.
* **Dynamic strategies** change across time based on feedback from a previous
  treatment or a threshold in some signaling variable

For dynamic strategy split nodes in SWIGs, the noation uses g in lieu of a to
the right of the split to denote that the treatment value is not constant but
rather changes based on the strategy. Everyone receives the dynamic strategy g.

* *A*<sub>0</sub>|*g*<sub>0</sub>
   receives treatment
* *A*<sub>1</sub>|*g*<sub>1</sub>

SWIGs are much better for identifying relationships for dynamic strategies than
are causal DAGs.

