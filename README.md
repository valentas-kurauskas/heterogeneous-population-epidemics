# Short description

A quick script to try to understand the effect of quarantine using random graphs with a toy degree distribution. 

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/valentas-kurauskas/heterogeneous-population-epidemics/master)

A fraction *1-p_a-ε* of the population infects *0* new individuals.
A fraction *p_a* of them infects *a* new individuals. Finally, a fraction ε of the population infects a large number *b* of new individuals (they are "superspreaders"). We assume that the [basic reproduction number](https://en.wikipedia.org/wiki/Basic_reproduction_number) R0 is known and fixed, and adjust ε accordingly.

When R0 fixed, if most individuals observe quarantine, the same growth can only be sustained by those that don't or can't, let us call them "superspreaders". If this is the case (most individuals do not pass the infection on, but the initial growth is still fast), the final size of an epidemics (the largest component) may be smaller than the one predicted by the simple G(n,p) model corresponding to a completely homogeneous population (initial growth is the same but everyone equally ignores the quarantine, the green line in the plot).

![Example chart](example.png "30% infect 1, 100ε% (the superspreaders) infect b, others infect 0")

For $G(n,p)$ the blue line is the ["herd immunity threshold"](https://en.wikipedia.org/wiki/Herd_immunity#Mechanics) $1 - \frac 1 {R_0}$. If herd immunity is attained via "natural infection" as opposed to vaccination, the epidemics only begins to die out once this point is reached. The total infected fraction (the green line) is quite a bit larger, it is the unique solution $\rho=\rho(R_0)$ of $1-\rho = e^{-R_0 \rho}$
in the interval $0 < \rho < 1$.

# Literature

Svante Janson and Malwina J. Luczak, *A new approach to the giant component problem*, Random Structures & Algorithms **34** (2009), 197-216.
