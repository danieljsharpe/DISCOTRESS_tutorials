# DISCOTRESS tutorials

Learn to get started using [DISCOTRESS](https://github.com/danieljsharpe/DISCOTRESS) with these tutorials, then apply the methods to your own Markov chains!

<p align="center">
  <img src="https://github.com/danieljsharpe/DISCOTRESS_tutorials/blob/master/fpt_distribn_example.svg">
  <i>Numerical estimate of the &#120068; &#8592; &#120069; first passage time (FPT) distribution from dynamical simulations; one of many quantities that can be computed using DISCOTRESS.</i><br>
</p>

Finite Markov chains are network models that can be used to model phenomena as varied and exciting as:
- animal movement within an ecosystem, such as migration :bird: :parrot: or foraging :elephant: :palm_tree:
- the variation in populations of species within an ecosystem, for example arising from predator-prey interactions :wolf: :deer:, competition for limited resources :bear: :fish:, or the introduction of a parasite :mosquito: or invasive species :snake:
- the evolution of organisms or genes characterised by the fitness for their environment :giraffe: :turtle:
- epidemic spread of a disease in a population :microbe: :syringe:
- climate dynamics :sun_behind_rain_cloud: :tornado:
- the fluctuating status of financial markets :money_with_wings: :chart_with_upwards_trend:
- structural changes in molecular and condensed matter systems, for example a protein or DNA molecule folding to its functional shape :dna: :atom_symbol:
- the distribution of molecule copy numbers in biochemical or chemical reaction cycles or gene regulatory networks :test_tube: :petri_dish:

We are typically interested in a particular &#120068; &#8592; &#120069; first passage process on the Markov chain. That is, we wish to understand the dynamical process of first hitting an absorbing (target) set of nodes &#120068; for paths beginning within the initial set of nodes &#120069;. We may want to know: what is the average time to reach the &#120068; state? Which nodes are most likely to be visited along an &#120068; &#8592; &#120069; path?  How many times is each node visited along an &#120068; &#8592; &#120069; path on average? If the &#120068; &#8592; &#120069; transition is slow (i.e. low probability) compared to random fluctuations, then linear algebra methods to solve for exact dynamical properties are numerically unstable and the standard kinetic Monte Carlo method to simulate paths is inefficient and therefore unfeasible. DISCOTRESS includes implementations of advanced algorithms that negate these problems. The software is highly flexible, and can also be used to efficiently simulate long-timescale trajectories that are not conditioned on initial and target states.

## Overview of tutorials

The following tutorials use simple example Markov chains to demonstrate various key features of the algorithms available in DISCOTRESS, allowing you to familiarise yourself with the capabilities and flexibility of the software:

- **mfpt\_ctmc**: you will learn to exactly compute key dynamical properties characterising an &#120068; &#8592; &#120069; transition in a continuous-time Markov chain (CTMC), using numerically stable state reduction algorithms. Namely: mean first passage times (MFPTs), committor and absorption probabilities, and the stationary distribution.
- **mfpt\_dtmc**: repeats the same exercise for a discrete-time Markov chain (DTMC).
- **kmc\_ab**: you will learn to use the standard kinetic Monte Carlo (kMC) (aka Bortz-Kalos-Lebowitz, BKL) algorithm to simulate &#120068; &#8592; &#120069; paths.
- **kps\_ab**: you will learn to use the kinetic path sampling (kPS) algorithm to simulate &#120068; &#8592; &#120069; paths.
- **dimredn**: you will learn to use kinetic path sampling (kPS) to simulate many short nonequilibrium trajectories initialised from each community, from which a coarse-grained Markov chain can be estimated and validated.

Scripts to help you process the output of DISCOTRESS simulations are available [here](https://github.com/danieljsharpe/DISCOTRESS_tools).
