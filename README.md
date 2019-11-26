# SemEval-2020-Task5
SemEval-2020-Task5

### 说明
#### Subtask1: Detecting counterfactual statements
In this task, you are asked to determine whether a given statement is counterfactual or not. Counterfactual statements describe events that did not actually happen or cannot happen, as well as the possible consequence if the events have had happened. More specifically, counterfactuals describe events counter to facts and hence naturally involve common sense, knowledge, and reasoning. Tackling this problem is the basis for all down-stream counterfactual related causal inference analysis in natural language. For example, the following statements are counterfactuals that need to be detected: one from healthcare and one from the finance domain:

Her post-traumatic stress could have been avoided if a combination of paroxetine and exposure therapy had been prescribed two months earlier.
Finance Minister Jose Antonio Meade noted that if a jump in tomato prices had been factored out, inflation would have begun to drop.
While the above examples are chosen for clarity for demonstration, real statements are harder for computers to judge.
 
#### Subtask2: Detecting antecedent and consequence
Indicating causal insight is an inherent characteristic of counterfactual. To further detect the causal knowledge conveyed in counterfactual statements, subtask 2 aims to locate antecedent and consequent in counterfactuals.
 
According to (Nelson Goodman, 1947. The problem of counterfactual conditionals), a counterfactual statement can be converted to a contrapositive with a true antecedent and consequent. Consider the “post-traumatic stress” example discussed above; it can be transposed into “because her post-traumatic stress was not avoided, (we know) a combination of paroxetine and exposure therapy was not prescribed”. Such knowledge can be not only used for analyzing the specific statement but also be accumulated across corpora to develop domain causal knowledge (e.g., a combination of paroxetine and exposure may help cure post-traumatic stress).
 
Please note that in some cases there is only an antecedent part while without a consequent part in a counterfactual statement. For example, "Frankly, I wish he had issued this order two years ago instead of this year", in this sentence we could only get the antecedent part. In our subtask2, when locating the antecedent and consequent part, please set '-1' as consequent starting index (character index) and ending index (character index) to refer that there is no consequent part in this sentence. For details, please refer to the 'Evaluation' on this website.

