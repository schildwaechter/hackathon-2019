

# CodeRefinery Hackathon 2019

Stockholm Nov 6-7, 2019

Event website: https://coderefinery.org/events/2019-11-06-stockholm/


## Projects

### 1. Improve training material for inter-service-communication on Kubernetes (Carsten Thiel and colleagues)

This project is about improving [CESSDA](https://www.cessda.eu) training material for 
[an internal training in December](https://www.cessda.eu/News-Events/Events/CESSDA-Technical-Infrastructure-Training-Day). This is mostly focussed on microservice architecture and inter-service-communication as well as 
on automated testing with quality gates & linting.
The services will be dockerised and running on Kubernetes.

The plan is to do this based on a virtual [CESSDA](https://www.cessda.eu) Café 
consisting of a cashier, coffee machine(s), and a waiter, for which we have example components ready.
At the December training, participants will bring along their own dockerised coffee machines,
run them through our continuous integration service and deploy them to the full Café.

The goal is to make this material as re-usable as possible also outside of CESSDA.
We would therefore welcome collaboration, in particular on the generic parts.


### 2. Efficient implementation of the bootstrap particle filter in Julia using StaticArrays (Samuel Wiqvist)

To run the pseudo-marginal Metropolis-Hastings algorithm [1] fast for
state-space models is it of importance to efficiently estimate the likelihood
numerically with a bootstrap filter [3] (or some other sequential Monte Carlo
algorithm). Therefore, this project aims to implement a bootstrap particle
filter using the static array support in Julia
(https://github.com/JuliaArrays/StaticArrays.jl). Using the StaticArray
support in Julia could potentially improve the performance of the particle
filter quite a bit (we could perhaps achieve a 10x speed-up). A starting point
could be to implement the static bootstrap filter for the simple example
"example 1" in [2]. However, an extension could be to implement a generic
filter, for instance using functional programming and/or metaprogramming.

[1] Andrieu, Christophe, Arnaud Doucet, and Roman Holenstein. "Particle markov chain monte carlo methods."
Journal of the Royal Statistical Society: Series B (Statistical Methodology) 72.3 (2010): 269-342.

[2] Cappé, Olivier, Simon J. Godsill, and Eric Moulines. "An overview of existing methods and recent advances in sequential Monte Carlo."
Proceedings of the IEEE 95.5 (2007): 899-924.

[3] Gordon, Neil J., David J. Salmond, and Adrian FM Smith. "Novel approach to nonlinear/non-Gaussian Bayesian state estimation."
IEE proceedings F (radar and signal processing). Vol. 140. No. 2. IET Digital Library, 1993.


### 3. Create something interesting with our anonymized pre- and post-workshop survey results (Thor Wikfeldt)

Description coming up ...


### 4. Update the style of CodeRefinery lessons to match https://github.com/carpentries/styles/ (Radovan Bast)

At some point CodeRefinery lessons had the same styling as Carpentries lessons
but both evolved a bit since and I think CodeRefinery lessons could benefit
from a face-lift. Not only to make the material look better, but also to make
it look more familiar to the Carpentries community and simplify uptake there.


### 5. Create a web app which can update forked branches (Radovan Bast)

Creating forks on GitHub is simple but updating forks is not easy for persons
who are not familiar or comfortable with the command line. Here we would
create an app to which one could log in using GitHub and refresh forks with a
button click. For simplicity we would allow updating forked branches only if a
fast-forward is possible.

Tech stack to be discussed but would probably involve https://vuejs.org
and https://graphql.org/learn/.
