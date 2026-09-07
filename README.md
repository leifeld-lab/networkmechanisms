# NetworkMechanisms
Identification of Causal Mechanisms in Temporal Networks

## Observational data with complex dependence
This repository explores statistical and causal identification of competing mechanisms in networked systems. Networked systems are sets of observations that are not independent and identically sampled (i.i.d.) from an underlying population process; instead, modelling the observations requires taking into account some of the other observations. Simple dependence like multilevel or time series specifications are insufficient to capture this complex dependence. Network models, such as exponential random graph models, relational event models, stochastic actor-oriented models, latent space/factor models, latent order logistic models, network autocorrelation models, or their relatives are required.

## Types of temporal networks
The definition of a networked system may include adjacency or bipartite, weighted or unweighted, directed or undirected, multilayer, multilevel, multipartite, or hyper-networks.

Causal mechanisms likely require *time* for statistical or causal identification. This can include panel, time series, or event specifications for network data.

## Causal mechanisms in networks, including social influence/contagion
Network data are often available in the form of observational rather than experimental data. However, different processes may operate on temporal networks. To model a temporal network, these processes should ideally be disentangled. For example, social influence (also known as social contagion or peer effects) can be mistaken for social selection (sometimes called homophily) or prior similarity (sometimes called confounding). A recent paper by [Leifeld and Brandenberger (2026)](https://doi.org/10.1093/jrsssa/qnag069) suggested counterfactuals in the model specification of relational event models to separate contagion from prior similarity in bipartite network event sequences. However, the proposed solutions work under strictly defined assumptions (listed in the paper); they do not operate on one-mode networks; and they do not take into account other competing mechanisms that could be at work, such as social selection, common exogenous shocks, or other types of social influence sometimes discussed in the policy diffusion literature.

## Open questions in this repository
This repository seeks to explore what it takes to identify these mechanisms in network data. Open questions include:

1. What is the range of behavioural mechanisms that compete with social influence/contagion in bipartite event sequences of actors and behaviours/choices, like in Leifeld and Brandenberger paper?
2. What is the range of behavioural mechanisms competing with social influence/contagion in one-mode networks (e.g., actors sending information to other actors with observations of their node attribute(s))?
3. If atemporality can be factored into the null distribution to disentangle influence/contagion from prior similarity like in the paper by Leifeld and Brandenberger, then what counterfactuals do we need to embed in the models to test for other mechanisms?
4. How do these mechanisms and their identification extend to other types of networks and time structures, as defined above?
5. Leifeld and Brandenberger proposed causal identification via statistical modelling. Is it possible (and desirable) to use causal inference techniques to achieve the same---or identification of other causal mechanisms in networks that compete with influence/contagion?
6. What other data structures can we use to identify influence/contagion in networks? Should we model behaviour as attributes, second modes, or spatially embedded observations like in network autocorrelation models? How do different methods and specifications fare relative to each other in identifying social influence/contagion relative to other mechanisms?

## Research entry challenge
Interested students, academics, or statisticians are invited to contribute to this endeavour via the research entry challenge [#1](https://github.com/leifeld-lab/networkmechanisms/issues/1). Please have a look there for further instructions on how to collaborate on this.
