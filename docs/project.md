
# Project: Ethical Automated SE

Computers are stupid, they only give you answers.   
-- Pablo Picasso

So your goal:
- using data mining and/or optimizers and/or theorem drovers
- generate more choices
- select the ones that satisfy local, and competing, biases

## Why this project?

Software 2.0

<img src="/docs/img/software2.png">

I want software 4.0 
- people * (Software 2.0)

Ethics = power + choice
- how we divide resources
- how we should decide who does not get stuff. 
  - problem, those decisions are usually secret
  - and  in an ethical world, those decisions are debated before being applied

Problems with debating choices:
- How to represent them?
- How to excise those choices:
- How to summarize what you Information overload


| Modeling method         | Exercise it                          | Summarize it                                    |
|-------------------------|--------------------------------------|-------------------------------------------------|
| Build a model           | Simulate (controlled by an optimizer | Data mining                                     |
| Look at historical data | Data mining                          | Cluster and find contrasts between the clusters |
| Sketch human intuitions | Theorem proving (find maximal consistent subsets that satisfy most constraints) | [thorem proving](#abduction)) |  
| Assert properties contrasts or legal requirements | theorem proving  | data mining

e.g. the COMPASS model (who is most like to commit crimes):

<p align=center>
<img src="/docs/img/compass.png" width=600>
</p>

e.g 

<img align=right width=600 src="/docs/img/choice.png">
<small>
<pre>
local my= {
sames=      512, 
bins=      .5,
best=      .5,
cohen=     .35,
combine=   "mode",
far=       .9,
conf=      .05,
k=         2,  
cliffs=    .25,
loud=      false,
bootstraps=512,
p=         2, 
seed=      10011,
some=      256,
wait=      10
}
</pre></small>

e.g. 
- The SCRUM model offered by Mendonca et al. [^mend]
  - 128 project management options and nearly 300 constraints
  - (e.g., if sprints last two weeks, then each individual task must take less than 10 days of programming). 
  - Complex mode;
    - less than 2% of the 2<sup>128</sup> choices are acceptable to that model. 
- The  PicoSAT [^pico] SAT solver can find tens of millions of satisfying solutions to the SCRUM model.
- Now we have a new problem
  - Too many solutions
  - Cognitive overload


[^mend]: M. Mendonca, M. Branco, and D. Cowan, "Splot: software
product lines online tools," in Proceedings of the 24th ACM
SIGPLAN conference companion on Object oriented programming
systems languages and applications, 2009, pp. 761–762.

[^pico]: A. Biere, "Picosat essentials," Journal on Satisfiability, Boolean
Modeling and Computation, vol. 4, no. 2-4, pp. 75–97, 2008.

Ethical decision making
- explore more choices, for more people, explores more bias
- make decision satisfying local biases
  - bias is how we decide what to ignore, what to focus on
    - I am biased towards breathing and eating, every day
    - I like making money, to pay the mortgage, so everyone at my place sleeps
      safe and secure in a warm bed each night.
- All  decisions are bias (otherwise, how do we decide?)
  - no bias, no ignoring stuff
  - no ignoring stuff, no summarization
  - no summarization, no model building
  - no models, no way to predict the future
  - so bias makes us blind (to what what have ignored)
    - and bias lets us see (the future)
- Biases need to be explict, debated, traded-off
  - you scratch my back, I'll scratch yours

How do you know if you are ethical?
- can you recognize who might be harmed by this design?
  - are you talking to those people?
- are you changing your designs to empower more people?

# Abduction

| A logic to guide guessing about what question to ask next.

(Historical note: this was my Ph.D. thesis, waaaaaaay back in time. None of the following ever really scaled. But lately I've realized that if we 
use data miners and theorem provers as the engine under the hood, then all these could become practical and reasonable.)

Abduction: inference to the best guess

Given rules of the form _cause_ &rarr; _effect_ then

| What      | Given                                                            | Generate     | Comment                     |
|-----------|------------------------------------------------------------------|--------------|-----------------------------|
| deduction | _cause_ + _rule_                                                 | _n_ | certain                     |
| induction | Lots of experience  that _cause_  and _effect_ are seen together | _rule_       | possible                    |
| abduction | _rule_ + _effect_                                                | _cause_      | not a certain inference (*) |

<img src=/docs/img/logic.png>

How to make a mistake, with abduction:
- Rule1: The sprinkler wets the grass
- Rule2: The rain wets the grass
- Effect: The grass is wet
- Cause: it rained
  - Not certain. What about the sprinkler?

Abductive inference requires validation
- It is the logic of guessing what question to ask next.

Given:
- a theory _T_
- with goals _G_
- and some _nogood_ constraint predictors,

Find:
- assumptions _A_ 
- that achieve the most goals you can
- fewest mistables. 

In practice only subset of _T_ is usable and only some subset of _G_ is achievable:

- T’ &sube; T
- G’  &sube; G   
   
So:

- _T’ &cup; A’ &rarr; G'_
- _&not; (T’ &cup; A’ &rarr; nogood)_  

Notes:
- Slow (all those subsets). In fact, formally this is [NP-hard](https://doi.org/10.1016/0004-3702(91)90005-5)
- Many solutions (all those subsets)
- Some solutions contradict other solutions
  - So usually group solutions into consistent "worlds of belief"
- Some worlds contain other worlds 
  - So we usually only talk "maximal" worlds (i.e. are not contained in other worlds)
- Which world you want depends on your biases
  - Different biases select different world, suitable for different tasks
  - Planning: favor worlds with least cost of assumptions
  - Classification: favor worlds with largest overlap to known facts
  - Explanation: favor the world that most overlaps with beliefs of audience
  - Tutoring: Expiation + planing (where we "plan" to go somewhere the student has not seen before)
- There is no _best_ bias
  - Just biases that are most useful in different contexts.


