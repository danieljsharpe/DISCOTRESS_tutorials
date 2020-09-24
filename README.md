# DISCOTRESS tutorials

Learn to get started using DISCOTRESS with these tutorials! Then apply the methods to your own Markov chains 🦜🌴💸📈🧬🦠

.center[

![Example first passage time distribution](https://github.com/danieljsharpe/DISCOTRESS_tutorials/blob/master/fpt_distribn_example.pdf?raw=true)

.caption[
**Numerical estimate of the first passage time (FPT) distribution from dynamical simulations; one of many quantities that can be computed using DISCOTRESS.**
]

]

## Overview of tutorials

The following tutorials use simple example Markov chains to demonstrate various key features of the algorithms available in DISCOTRESS, allowing you to familiarise yourself with the capabilities and flexibility of the software.

- **mfpt\_ctmc**: you will learn to exactly compute key dynamical properties characterising an A<-B transition in a continuous-time Markov chain (CTMC), using numerically stable state reduction state reduction algorithms. Namely: mean first passage times (MFPTs), committor and absorption probabilities, and the stationary distribution.
- **mfpt\_dtmc**: repeats the same exercise for a discrete-time Markov chain (DTMC).
- **kmc\_ab**: you will learn to use the standard kinetic Monte Carlo (kMC) (aka Bortz-Kalos-Lebowitz, BKL) algorithm to simulate A<-B paths.
- **kps\_ab**: you will learn to use the kinetic path sampling (kPS) algorithm to simulate A<-B paths.
- **dimredn**: you will learn to use kinetic path sampling (kPS) to simulate many short nonequilibrium trajectories initialised from each community, from which a coarse-grained Markov chain can be estimated and validated.
