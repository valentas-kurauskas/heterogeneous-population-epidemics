# Short description

A quick script to try to understand the effect of quarantine using random graphs with a toy degree distribution. 

A fraction *1-p_a-ε* of the population infects *0* new individuals.
A fraction *p_a* of them infects *a* new individuals. Finally, a fraction ε of the population infects *b* new individuals (the "superspreaders"). We assume that the [basic reproduction number](https://en.wikipedia.org/wiki/Basic_reproduction_number) R0 is known and adjust ε accordingly.

Keeping R0 fixed, if a large fraction of individuals observe quarantine even with the presence of superspreaders the epidemics (largest component size) can be smaller than predicted by the simple G(n,p) model.

![Example chart](example.png "30% infect 1, 100ε% (the superspreaders) infect b, others infect 0")

# Literature

S. Janson and M. J. Luczak, *A new approach to the giant component problem*, Random Structures & Algorithms **34** (2009): 197-216.
