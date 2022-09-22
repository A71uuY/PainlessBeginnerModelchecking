# Transition system

## Why model checking

Suppose we have a system, the usual way to check the correctness is software or hardware testing performed by human. The first problem is it usually cannot cover all possibilities so potential but fatal errors may occur, which is unacceptable in some domains. The second problem is human can make mistakes (also happen in other checking methods).
Model checking in this book means we use a model to represent a system then check if it have or vaiolate some properties. The advantage is it ensures correctness as long as we have correct model and specifications towards it.

## Transition system

**Transition system** is frequently used to model a system. We define Transition System as a tuple $(S,Act,I,\rightarrow,AP,L)$ in which $S$ is the set of states, $Act$ is the set of possible actions of the system, $\rightarrow:S \times Act \times S$ is the transition from a state to another state by an action, $I$ is the initial states, $AP$ is the set of atomic propositions that uses logic propositions to describe some facts, $L:S \rightarrow 2^{AP}$ is labelling function that uses the combination to describe 'what is true' in a state.

For instance, if we have a Beverage Machine, we can insert coins, select 'soda' or 'beer', and we can take drinks away, then we can model $S=\{pay, select, soda, beer\}$, $Act=\{insert/_coin, get/_soda, get/_beer, \tau\}$, $I=\{pay\}$, $AP=\{drink, paid\}$.
