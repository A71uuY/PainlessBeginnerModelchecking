# Some properties

Here let's see some real properties.

## Safety

Safety requirements say 'nothing bad should happen', or 'bad thing can never happen'. 

### Invariant

Invariant is a special kind of safety property. It says 'something always holds', $P_{inv} = \lbrace A_0A_1... \in (2^{AP})^\omega | \forall i \geq 0 ~ A_i \vDash \Phi \rbrace$ in which $\Phi$ is an invariant condition.
So we say a transition system $TS \vDash \Phi$ iff all reachable states $s \vDash \Phi, \forall s \in Reach(TS)$ in which $Reach(TS)$ is the set of all reachable states in transition system $TS$.
