# Lesson 7

## Building Your Causal DAGs

### What DAGs don't need to show

DAGs are not meant to be built as an exact representation of the world with all
factors included.

* Do not need to add all causes of causes under study
* Ddo not need need to all mediators between the cause and effect under study

### Elements of DAGs

* Start with treatment and outcome nodes without any mediators
* Add nodes for all common causes of the treatment and outcome
* Make sure to identify whether common causes are measured or unmeasured
  * To avoid cluttering the graph, typically L is used for all measured common
    causes and U is used for unmeasured common causes
* Common way to draw dags are left to right or top to bottom
* Selection nodes are denoted by C if there is additonal selection criteria
* Nodes for mis-measured variables need to be added

***Any time a node is added to the graph, any common causes of multiple nodes
in the DAG must be added as well***

> A causal DAG can be a crude representation of reality as long as it includes
> all factors of confounding, selection bias, and measurement bias

### Mediators in DAGs

* If you are interested on the effect of a mediator, you can add the mediator to
  the causal DAG.
* If there is a mediator that can be placed between nodes on a graph and
  conditioned on to block a path on the DAG, then it should be added 
* A mediator can be used to create a front door path A -> M -> Y via the front 
  door method to establish the cause A on Y, but is not very useful in practice
  becasuse the mediator must have not common causes of A and Y and this has not
  been the case in practice

### Discovery in DAGs

Subject matter knowledge is relied upon to now which common causes to add to
DAGs and is usually sufficient.  However, sometimes subject matter expertised
is not sufficient in the area of study and in these these cases causal learning
from data might be able to help.

**Causal Disovery or Causal Search** - is when data is used to try to find the
structure of a causal DAG in cases where subject matter expertise is limited.
Causal discovery associations can often be explained by multiple DAG
structures, so additional analysis is required to use them responsibly.

