t's about "universal truth". 
Eg: "all human are mortal", in horn logic becomes:
```
¬ human(X) ∨ mortal(X)
```
which is equivalent to `∀X (¬ human(X) ∨ mortal(X)) `, or `∀X (human(X) => mortal(X)) `. 
*Why this means "if-then"? I read it as: any X should be either (non-human) or mortal, thus human must be a subset of mortal, thus human is sufficient for mortal.*

Besides "universal", Horn logic can contain only **1 positive argument (/"literal")**, like mortal in the case above -- this is said to be its [definition](https://cs.nyu.edu/courses/spring02/G22.2560-001/horn.html).

## Why do I care about it? 
Because probabilistic Horn logic can be used to infer knowledge-base contents. *(Toward an Architecture for Never-Ending Language Learning)*
>"Rule Learner (RL): A first-order relational learning al- gorithm similar to FOIL (Quinlan and Cameron-Jones 1993), which learns probabilistic Horn clauses. These learned rules are used to infer new relation instances from other relation instances that are already in the KB." 

Example of rules learnt by the RL mentioned above.
+ X playsin NBA => X is a basketball player: 
``` 
¬ AthletePlaysInNBA (X) ∨ AthletePlaysBasketball (X)
```

**However**, don't see what's the **convenience** of using this specific language rather than saying X=>Y. Is there other properties of Horn logic?

## General field related
+ Logic
+ logic programming -- it's used in programming language Prolog. Wikipedia said...
>Horn clause logic is equivalent in computational power to a universal Turing machine.
(okay, what's universal Turing machine, first?)
+ model theory (don't understand what is it)
+ machine theorem proving -- sounds so cool![https://en.wikipedia.org/wiki/Automated_theorem_proving]



