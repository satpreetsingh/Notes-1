<a name='1'></a>

Physics 112: Statistical Mechanics
==================================
January 18, 2012
----------------

Organization
-----------
Goals

 * Deeper understanding of concepts: less mysterious.
   + Entropy
   + Free energy
   + Chemical potential
   + Statistical mechanics
	  - Fluctuations
	  - Kinetic theory background ← use of simulations
   + Recognition of physics in a "context-rich" situation, i.e. real life.
 * Acquire computational tools
   + Quantitative
   + Problem-solving skills
 * Linkages to
   + everyday life
	 - bridge between microscopic and macroscopic
	 - irreversibility
	 - engineering
   + modern physics
	 - frontier
	 - applications e.g. astronomy, cosmology
	   · condensed matter physics, low temperature
   + History

Participation

 * Focus: Conceptual Understandidng
   + We learn by construction/reconstruction of your mental models.
   + This process is both intensely personal and social (learn through
	 others)
   + focus on grades, formulae, short cuts
 * Before lecture
   + Read book and notes because our use of clickers which decreases
	 the in-class presentation time, there will be testing of this
	 reading.
   + Play with applet simulations → intuition. (You can suggest others
	 you can find)
* In class
  + Beginning of class: typically a conceptual question/applet
  + Peer instruction questions:
	- A conceptual question
	- Vote (with clickers)
	- Discussion in small groups
	- Vote again
  + Active participation during lecture: questions, clickers
  + "One minute" random quizzes (check attention to the material)
* Out of class
  + Homework
  + Working groups on problems if you like (but you write your own
	solution)
  + Discussion sections (but try homework first)
  + Office hours (come with questions)

Clickers:

* Systematic use in class begins Mon, Jan 23.

[ More boring administrative stuff; not particularly unique to this
  particular class. Largely duplicated from the syllabus. ]

[ note to self: 277 Cory ]

<a name='2'></a>

Physics 112: Statistical Mechanics
==================================
Kinetic Theory 1 / Probabilities. January 23, 2012
--------------------------------------------------
Details:

 * clickers
 * homework -- due in LeConte reading room
 * webcasts
 * Discussion sections

Ideal Gas

 * particle interaction leads to thermal equilibrium.
 * particle probability distributions are independent
 * particle systems where interaction time ≪ mean free time between
   collisions

Motivations: statistical mechanics and fluctuations
===================================================
The need for statistical mechanics
----------------------------------
How to describe large systems.
------------------------------
 * very large
 * at finite temperature – not at rest
   + velocity $v \approx 300$m/s @ 300K.
 * Constant collisions
   + mean free path $\lambda \approx 0.1$ μm.
 * Probabilistic description. 1 particle
   + Classically
	 - Have to track both position and velocity/momentum.
	 - We will introduce a phase space. The probability distribution
	   on phase space = position × momentum.
	 - Problem is that states are treated as continuous.
   + Quantum – states are actually discrete / countable.

N particles
-----------
In many cases it is a good approximation to treat particles as
independent. We will call this an ideal gas.

Temperature, pressure, entropy
------------------------------

Temperature as a measure of mean energy of excitations of the system. Two
reasons: 1) usually more degrees of freedom than spatial degrees of freedom
(spin (e.g. ferromagnetism), and 2) other effects: quantum gas: Fermi-Dirac
exclusion principle (i.e. we cannot put two particles in the same state)
means that we have to stack in energy. Their mean energy is very large,
even at 0K.

Pressure as a measure of energy density or "average" force per unit area on
walls of container.

Entropy as a measure of the state of disorder of a system. Modern
definition: $\sigma = -\sum p_i \log p_i$. 0 if in one state, max if flat
distribution.

<a name='3'></a>

Physics 112: Statistical Mechanics
==================================
Kinetic Theory 2 / Probabilities. January 25, 2012
--------------------------------------------------
# House keeping.
# Fast introduction to kinetic theory.
 * Equilibrium
 * Vibrations
# Probabilities.
 * Distributions
 * Moments

How a system reaches equilibrium
================================

Diffusion. True also in probability space. An isolated system tends to
evolve toward maximum flatness.

We won't speak classically of position + momentum, but rather of
states. Quantum states. The same thing happens in the case of probability.

It turns out that when all the properties are equal, we have maximum
entropy. Equilibrium occurs when "you are maximally flat".

Fluctuations
============

Fluctuations are the effect of life if you don't have an infinite number of
degrees of freedom. Which never happens. One of the fundamental properties
is noise. Noise is intrinsic to the finity of degrees of freedom.

Central limit theorem. Fluctuations decrease as samples increase.

Probabilities
=============

Probabilistic event: occurs in an uncontrolled manner, described by random
variables. parameters are fixed (even if unknown).

# Discrete case
 * consider bins.

An example of discrete probabilities is a histogram. Raw counts.

Cannot determine probabilities via experiments. Probability distributions
add up to 1. Probabilities cannot be negative.

# Continuous case
 * Actually a lie.

Moments. Stuff.

<a name='4'></a>

Physics 112: Statistical Mechanics
==================================
Kinetic Theory 3 / Probabilities. January 27, 2012
--------------------------------------------------

Various probability stuffs. Continuous distirbutions. Sum/average of
independent events. Central limit theorem.

$$
  P(s) \ge 0, \sum P(s) = 1
  \\ \avg{y} = \sum y(s)P(s) \text{ [ this is the first moment. ]}
  \\ y(s) = 35 \delta_{ik}. \avg{y} = \sum 35\delta_{ik} = 35/38.
$$

Variance:

  $\sigma^2 = \avg{(y(s) - 〈y})^2 = \avg{y^2} - 2\avg{y\avg{y}} + \avg{y}^2
  = \avg{y^2} - \avg{y}^2$

root mean square (rms) $\equiv$ standard deviation

Independence. Usually, if I have two random variables, x and y, the
probability of $P(x,y) = P(x|y)P(y) \neq P(x) \times P(y)$. We say we have
independence iff $P(x,y) = P(x)P(y)$. In other words, $P(x|y) = P(x)$.

You can define a correlation coefficient to be
  $\frac{(x - \avg{x})(y - \avg{y})}{\sigma_x\sigma_y}$.

Independence $ ⇒ \rho = 0$. Converse not necessarily true.

Continuous distributions. Histograms. The case where a variable is
continuous. We now have probability _densities_.

$$
  f(x)dx = g(y)dy = f(x,y)\deriv{x}{y}dy.
  f(x) \ge 0, \sum f(x)dx = 1.
$$

Moments: we can define moments in exactly the same way as before.
The moment of a variable $y(x)$

$$
\avg{y(x)} = \int y(x)f(x)dx.
\\ \mu = \avg{x} = \int xf(x)dx.
\\ \sigma^2 = \avg{x²} - \avg{x}² = \int x^2 f(x)dx - \parens{\int xf(x)dx}^2.
$$

$f(x,y)dxdy = g(x)dx h(y)dy$. Factoring works the same way, if our
variables are independent.

Normal distributions: Gaussian.

It is very important to put the differential element ($dx$ or $dy$) because
the function changes depending on what the differential element is. The
histogram depends on what variable you choose to plot. If I choose $x$ or
$x^2$, my histogram will be different. Usually.

The mean is in the middle of a normal distribution because the third
moment is 0.

Full-width half maximum (FWHM) $\approx 2.3\sigma$

A is called the mode, i.e. the maximum. In a distribution with nonzero skew
(like the Maxwell-Boltzmann), the mode is different from the mean.

mean: location.

standard deviation: width.

skewness: symmetry.

kurtosis: peakedness.

Fourier transform is the characteristic function. The log of this is stuff
with cumulants.

Sum of random variables:

$$
x \equiv y + z
\\ \avg{x} = \avg{y} + \avg{z}.
\\ \sigma^2_x = \sigma^2_y + \sigma^2_z + 2\rho\sigma_y\sigma_z.
\\ \text{Independence} \implies \rho = 0; \sigma^2_x = \sigma^2_y + \sigma^2_z
\\ h(x)dx = (f*g)(x)dx \implies \text{the cumulants add!}
$$

Proof: Convolution in original space is equivalent to product in Fourier
space. Hence for a sum, the characteristic functions multiply and the logs
of characteristic functions add.

Central limit theorem: Cool if our variables actually are independent.

<a name='5'></a>

Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. January 30, 2012
-----------------------------------
Homework
========
First one is due today, second one is posted.

Central Limit Theorem
=====================

Taking N independent random variables $x_i$ of average $\mu_0$ and of
variance $\sigma_0^2$, the experimental average $A = \frac{1}{N}\sum
x_{i}$. $f(A)dA → \lim_{N\to\infty} \frac{1}{\sqrt{2\pi}σ}
\exp(-\frac{(A-\mu)^2}{2\sigma^2})dA; \mu = \mu_0, \sigma^2 =
\frac{\sigma_0^2}{N}.$

This is different from $\avg{A}$, which would just be an integral.

The other thing is that $\sigma^2 = \frac{\sigma_0^2}{N}$. The variance
decreases as $\frac{1}{N}$, or the standard deviation decreases as
$\frac{1}{\sqrt{N}}$. This is fairly typical of stochastic processes, where
the relative width decreases as $\frac{1}{\sqrt{N}}$. Overall width will
increase if you don't normalize, but relative width decreases.

The relative widths of kurtosis and skewness go to zero as we add more
terms.

Consequences for Thermodynamics
-------------------------------

Because of large number of particles, averages are very peaked around mean.

 * System well characterized by mean = "macroscopic quantity".
 * Fluctuations are very small.
 * Not a lot of difference between most probable value, mean value,
   and experimental value.

Dealing with systems with large degrees of freedom. Temperature, for
instance, is related largely to the kinetic energy of the particles. It
will be very well-defined and have very few fluctuations if we are just
measuring the mean of said particles, and it will be very peaked around the
mean.

The central limit theorem makes thermodynamics meaningful.

Quantum States of a System
==========================
States of a System
------------------
Not covering spins. ALso, marginal definition of entropy.

(mostly chapters 1 and 2 of Kittel and Kroemer)

 * States / COnfigurations
 * Probabilities fo States
   + Fundamental assumptions
   + Entropy
 * Counting States
 * Entropy of an ideal gas.

State = Quantum State.
 * Well-defined, unique.
 * Discrete ≠ "classical thermodynamcs" where entropy was depending on
   resolution ΔE.

Boltzmann for reasons that he did not fully understand arrived at the
conclusion that he had to have discrete states. This was before Planck and
quantum mechanics. Boltzmann was always doubting himself to the point that
he took his own life. So when you are a little bit despaired, think about
Boltzmann.

It's amazing that a guy like that who contributed so much to modern physics
was unsure of himself.

Configuration = Macroscopic specification of system

 * Macroscopic Variables
   + Extensive: U, S, F, H, V, N (not normalized)
   + Intensive: T, P, μ (chemical potential)
 * Not unique: depends on level of details needed.
 * Variables + constraints ⇒ not independent.

Many microstates (states) correspond to a single macrostate
(configuration).

Quantum Mechanics in 1 transparency
-----------------------------------
Fundamental postulates

 * State of one particle is characterized by a wave function.
 * Probability distribution = |Ψ(x,t)|^2 with 〈Ψ|Ψ〉 = ∫{Ψ(x)*}Ψ(x)dx = 1.
 * Physical quantity → Hermitian operator.
 * In general, not fixed outcome. Expected value of Ô = 〈Ψ|Ô|Ψ〉.
 * Eigenstate ≡ state with a fixed outcome e.g. Ô|Ψ〉 = o|Ψ〉, where o
   is a number.
 * A finite system has discrete eigenvalues.

1-dimensional case, infinitely deep square well. Solve via separation
of variables, construct Fourier series.

If you solve this equation, you can show that in that case, the wave
function has to go to 0 at the wall.

That's just a particle in a box. If you ask yourself what is the momentum
of this particle, this particle is actually a series of two momenta. It
does not have a well-defined momentum, since it is going back and forth.

<a name='6'></a>

Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 1, 2012
------------------------------

REMINDER: states ⇒ microstates; configurations ⇒ macrostates.

Overview:

 * Discrete states
 * Isolated system in equilibrium

Postulate; H theorem. One of the finest works in physics by
Boltzmann. Shows that entropy is increasing. The probability distributions
of the states tend to equalize. Whatever initial probabilities tend to
evolve toward equilibrium.

 * Counting states

Quantum Mechanics (again)
=========================

Particle in a box (or, if you like, an infinite square well). By the axioms
of quantum mechanics, these solutions are identical to the modes of a
vibrating string.

[ clicker question regarding distance between momentum states. Talk
  about Uncertainty principle. ]

ℏ/2L: distance between momentum states.

quantization comes from the combination of both the eigenvalue equation as
well as the specific boundary conditions.

Same thing happens with a hydrogen atom. We have an electron orbiting
around the photon, and Bohr said that if you turn the nucleus by 2π, your
function should come back on itself. And then if you solve the radial
Schrödinger equation, it is the solution where you have something finite at
the origin and 0 at infinity which gives the quantization of energy.

Basically resonance conditions, like a vibrating string, will give us
discrete energy levels.

SPIN
====

Particles can carry a spin – a unit of angular momentum. Actually, they can
carry an angular momentum. Carrying integers and half-integers of angular
momentum – former are known as fermions, and latter are known as
bosons. Very different.

If I have a spin of 1, it can point up, nowhere, or down. The photon, which
is massless, is spin 1 with 2 spin states. (exception: usu. spin s ⇒ 2s+1
states.)

$\epsilon = mB$, where m = magnetic moment, B = magnetic field. emission of
photons, directions of spin.

Important implication in medicine: MRI is the magnetic resonance
imaging. Uses this property to see where the spins of the hydrogen
are. Just looking at hydrogen, basically.

Energy now is is proportional to r².

Fundamental postulate
=====================

Probabilistic description of state of a system.

Systems in equilibrium. An isolated system in equilibrium is equally likely
to be in any of its accessible states. Kittel does not specify in
"equilibrium". It does not matter if we are close to equilibrium.

Consequences
------------

Probability of a configuration:

 * Probability of configuration: simple counting problem, normalized.

This allows us to compute probabilities of configurations. This method is
conventionally called a microcanonical computation. Characterized by being
very awkward, cumbersome, difficult to implement, and so on.

Entropy
=======

$\sigma = -\sum p log p = -H$. H = Negentropy = Information (Shannon).

For an isolated system in equilibrium: identical to Kittel. In classical
thermodynamics, definition usually used is $dQ = TdS$.

Basically, we have a nondeterministic finite-state machine (weighted
probabilities and all) being run many times simultaneously. H theorem tells
us it will reach equilibrium i.e. all currents will cancel.

$\Gamma_{rs} = \Gamma{sr} ⇒ \text{ H theorem}$. Symmetry of the transition
rate will cause the evolution of the probabilities to converge eventually
to a flat distribution (_of microstates_). Else you have a nonzero
divergence in more than one state.

Stirling approximation: number of states goes to a Gaussian.

<a name='7'></a>

Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 3, 2012
------------------------------

homework problem #2:
$\exp(u² - 2ρuv + v²) ⇒ exp(u² + (v-ρu)² - ρ²u²)$

Counting States: Discrete States
================================

With just counting states and some assumptions as to what pressure and
temperature are, we have PV = NkT and U = 3NkT/2.

Density of spatial states per unit phase space
----------------------------------------------

Phase space: Position space (x) $\otimes$ (p) Momentum space.

Density of quantum states (orbital states) is $\frac{1}{h^n}$ per particle
(n ≡ dimensions). That is, if I have a volume in the phase space, I can
count the number of orbital states for one particle by dividing this volume
by $h^3$ (in three dimensions).

The volume of the phase space is just the integral of $\frac{d^3 x d^3 p}{h³}$.

Ideal Gas
---------

Now consider N particles in weak interactions. Total energy U is
constant. $g = \Pi \int \frac{d^3 xd^3 p}{h^{3N}}$. Insert a $\delta(\sum
\frac{p_{i}^2}{2M} - U)$. Basically imposing that the total energy of my
system is U. The product of $dx_i$ will give $V^N$. So there is no problem
there. But what about the $d^3 p_i \delta(\sum...)$? Imposing some of the
$\frac{p_i^2}{2N}$ to be equal to $U$. I'm looking now at the surface of a
sphere with a certain radius.

If we have one particle in one dimension, we have only one momentum
space. In large dimensions, $g \propto \frac{V^NU^{3(N-1)/2}}{h^{3N}}$.

[ Reasoning: for momentum integral: we need to conserve energy. ]

[ We are basically speaking of the surface of a volume in 3N-space. ]

$\sigma = \frac{S}{k} = \log(g) = \log(V^N U^{3N/2}) + \text{const}
  = N\log(V) + \frac{3N}{2}\log(U) + \text{const}.$

In that case, can write $dU = TdS - pdV$. Or, if you prefer, $\tau d\sigma
- pdV$.

Solve for U: $U = A\exp(2\sigma/3N)V^{-2/3}$.

$\tau = \pderiv{U}{\sigma(V, \sigma, N)} = \frac{2U}{3N} \iff U =
\frac{3NkT}{2}$.

$p = -\pderiv{U(V, \sigma, N)}{V} = \frac{2U}{3V} \iff pV = N\tau ≡ NkT$.

<a name='8'></a>

Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 6, 2012
------------------------------

[[ Talk about clickers. ]]

So far:
-------

$\sigma = -\sum p \log p$ ✓

H theorem: with an isolated system, probabilities of states evolve to being
equal.

Consequence of the H theorem: If I am looking at the probability of a
configuration, the probability is equal to (states in configuration) /
(total states)

$\sigma = \log (g_t)$ (mathematically equivalent to the first statement)

Counting of states to get the entropy.

Density of orbitals (quantum spatial wave functions) in phase space is
$\frac{1}{h^d}$ (dimension of space)

Once again: phase space $\equiv$ position space (x) $\otimes$ (p) momentum
space. Good way to compute the number of spatial states. degrees of freedom
(spin, rotation, vibration).

Number of states g(spatial states) of a system of energy U in a volume

V is $g ∼ U^{3N/2}V^N = \exp(\sigma). \tau \equiv kT, \sigma \equiv \frac{S}{k}$

$\tau = \pderiv{U}{\sigma}|_V \implies U = \frac{3}{2}N\tau$

$P = -\pderiv{U}{V}|_\sigma \implies PV = N\tau$

Just as natural, if not more so, to work with $\sigma(U,V) \equiv
\log(V^N U^(3N/2))$.

**We must be careful to note, when working with partial derivatives,
  which variables we are keeping constant.**

This is a very useful way of defining pressure and temperature once we have
counted states.

$\tau = \frac{1}{\pderiv{\sigma}{U}|_{V,N}}, p = \tau \pderiv{\sigma}{V}|_{U,N}$

We were starting with the phase space for our $N$ particles: $\frac{d^{3N}x
d^{3N}p}{h^{3N}}$: density of our states. We want to then integrate over
the volume, but we choose the states such that U fixed. Represents in our
3N-dimensional momentum space a sphere.

$\delta[\sqrt{\sum\sum p^2_{ik} - \sqrt{2MU}}]$. Take advantage of sifting
property of $\delta$.

radius of sphere in 3N momentum space. r has dimension $r^{d-1}$. In the
general case, we'll have $\Omega^{3N}r^{3N-1}$.

Thus we have $\frac{\Omega^{3N}\sqrt{(2MU)^{3N-1}}}{h^{3N}}$.

$\delta$ has dimension of $\frac{1}{p}$. $\int \delta(x)dp = 1$

Sackur Tetrode formula: entropy of an ideal gas. $\frac{S}{k} =
N(\log(\frac{n_Q}{n}) + 5/2)$

<a name='9'></a>

Physics 112: Statistical Mechanics
==================================
Entropy and Stuff. Feb 8, 2012
------------------------------

Divide $g_{t}$ by a missing $N!$, which is from indistinguishability of
particles / quantum states. Also, experiments were off by a very large
factor.

$g_t = \Omega_{3N}\sqrt{2M\Delta U}V^N U^{3(N-1)/2}/(N!h^{3N})$

Quantum density. What remains of our counting states.

$\sigma = N(\log(n_Q/n) + 5/2)$.

$n = N/V$, $n{Q} = \parens{\frac{2\pi M}{h²} \frac{2U}{3N}}^{3/2}$

Free expansion of gas (isolated system ⇒ no particle/heat exchange): final
temperature = initial temperature.

Entropy is increasing, however, since volume is increasing.

Chapter Three:

Equilibrium, Thermodynamics, Potential
======================================

RECALL:

$\frac{1}{\tau} = \pderiv{\sigma}{U}|_{V,N}$

$\frac{p}{\tau} = \pderiv{\sigma}{V}|_{U,N}$

$\frac{\mu}{\tau} = -\pderiv{\sigma}{N}|_{U,V}$

For an ideal gas in 3-space:

$$
U = \frac{3}{2}N\tau
\\ \tau \equiv kT
\\ pV = N\tau
$$

States of a combination of two systems
--------------------------------------

Take 2 systems and put them in contact.

Put them in weak interactions $U = U_1 + U_2, V = V_1 + V_2, N = N_1 + N_2$

Number of states $g_1(U_1,V_1,N_1)$, $g_2(U_2,V_2,N_2)$. Weak interaction ⇒
quantum states are not modified.

How many states do we have in the combined system?
$g_1g_2$

What is the configuration of maximum probability? The number of states in
$g(U_1,V_1,N_1)/g_t$. Take a derivative with respect to $U_1$ to see where
the extremum of this function is.

$$
\pderiv{g_1}{U_1} g_2 + g_1 \pderiv{g_2}{U_1} ≡ 0.
\\ \pderiv{g_1}{U_1} g_2 - g_1 \pderiv{g_2}{U_2} = 0.
\\ \frac{1}{g_1}\pderiv{g_1}{U_1} = \frac{1}{g_2}\pderiv{g_2}{U_2}.
\\ \pderiv{\log(g_1)}{U_1} = \pderiv{\log(g_2)}{U_2}.
\\ \pderiv{\sigma_1}{U_1} = \pderiv{\sigma_2}{U_2}.
\frac{1}{\tau_1} = \frac{1}{\tau_2}.
$$

<a name='10'></a>

Physics 112: Statistical Mechanics
==================================
Equilibrium, Thermodynamics, Potential. Feb 10, 2012
----------------------------------------------------

# Midterm
# Equilibrium between two two systems
# Laws of Thermodynamics

At the end of last lecture, we were considering two systems which can
exchange energy, volume, particles. We were asking ourselves what was the
most probable configuration $U_1,V_1,N_1$. $\pderiv{\sigma_1}{U_1} =
\pderiv{\sigma_2}{U_2} \equiv \frac{1}{\tau}$. Similarly,
$\pderiv{\sigma_1}{V_1} = \pderiv{\sigma_2}{V_2} = \frac{p}{\tau},
\pderiv{\sigma_1}{N_1} = \pderiv{\sigma_2}{N_2} = -\frac{\mu}{\tau}$ ($\mu$
for one species) – definitions.

The configuration of maximum probability share the same pressure,
temperature, potential.

The important thing is that the distribution of the system around this most
probable configuration is very peaked and becomes more peaked as we get
more particles (see central limit theorem).

Did not put volume because it is difficult to define walls.

The last point I wanted to make: by putting the system in contact, we have
increased the entropy of the system. That we know from the H theorem.

What Kittel and Kroemer say is approximately correct. "Entropy increases
because most probable configuration by default is greater than what you
started with before". This is approximate because they are speaking about
the most probable configuration.

$\sigma_{\max} < \sigma; \sigma_{\max} \approx \sigma$ (very very close,
though, because our probability distribution is very peaked. This is why
Kittel and Kroemer is merely an approximation)

In practice, it does not really matter, since this is a good enough
approximation for the systems that we work with: $\sigma-\sigma{max} \ll
\sigma = N(\log\frac{n_{Q}}{n}+5/2)$ [Sackur tetrode formula].

Kittel & Kroemer does recognize that, but it is presented in a slightly
confusing manner.

We have shown that indeed the temperature behaves as the temperature we
know. We have not yet shown that this is the same pressure.

Chemical potential affects various things such as rates of
diffusion. Determined by species of particles. However, at equilibrium, by
the H theorem, the chemical potential is equal in all accessible states.

What is chemical potential? It is a measure of the concentration! (verify
by working out $-\tau \pderiv{\sigma}{N}$). A lot of work for a very simple
result. But this is much more powerful. We will use this to look at
batteries, equilibrium in various systems. 

MIDTERM: Friday the 24th. 8:10-9:00. Why Friday and not Monday? Turns out
there is an important workshop on dark matter in UCLA. There is a potential
problem: Monday the 20th is President's day, so no class, no office
hours. Proposition: Tuesday the 21st, we have extended office hours from
4:00-6:00.

Alex's review sessions: Wednesday 15th (5-6), Wednesday 22nd (6-8).

You should take this midterm seriously but not panic too much about it. I
will also give you, next week, maybe before Wednesday, a small diagnostic
quiz that allows you to see where you are.

BACK TO THERMO.

Thermodynamics were developed over a century and a half from the late 1700s
to the early 1900s. Basically, by the beginning of the twentieth century,
there was this concept of three laws of thermodynamics (actually 4: the 0th
law says that at equilibrium, pressure, temperature, chem. potential are
equal).

The first law comes directly from our definition

$d\sigma = \frac{1}{\tau} dU + \frac{p}{\tau} dV -\sum \frac{\mu}{\tau}
dN$. Now, I can multiply by $\tau$ and we get $dU = \tau d\sigma - pdV +
\sum \mu dN$: change in energy = heat - work + chemical work

You can have many different expressions, but basically, this is a
consequence of our definition.

Second law of thermodynamics: when an isolated system evolves from a
non-equilibrium configuration to equilibrium, its entropy will increase.

Third law: entropy is zero at zero temperature (or log of number of states
occupied) ⇒ method to compute entropy.

If there is only one ground state, at zero temperature, all of the
particles will be in this ground state (not fermions) and there is only
one state. $p_0 = 1; p_i = 0 \implies \sigma = 0$. If there are several
ground states, this is degenerate; you will have a $\log g$, where $g$ is
the number of ground states.

Fermions: all of particles cannot be in the ground state. What you should
remember is that at zero temperature, there is one (or several) ways to put
all of the particles.

Thermodynamic identities. Rewrite slides in different ways depending on
what are your independent variables.

How do we measure entropy experimentally? There is a problem with assuming
ideal gas: not valid close to absolute zero. For that matter, Sackur
Tetrode is not valid at absolute zero. The classical approximation breaks
down when $n > n_Q$.

<a name='11'></a>

Physics 112: Statistical Mechanics
==================================
Macroscopic Thermodynamics. Feb 13, 2012
----------------------------------------------------

Nader Mirabolfuthi. 343 Old LeConte. 12-1p.

Review of some thermodynamics concepts, laws and applications.
Thermodynamic functions: Maxwell relations
Heat engines, refrigerators: Carnot cycle.

dQ = dE + dW.

The laws of thermodynamics were developed by people who didn't use
statistics.

equilibrium: A↔B.

0th law: equilibrium. 1st law: energy (heat in the form of energy). 2nd
law: entropy of isolated system increasing.

An exact differential is a well-defined function in terms of multiple
variables x and y. Very important feature: conservative vector
field. Internal energy is actually a state function of the system, whereas
heat and work can be added arbitrarily. Place bars to denote non-exact
differentials.

PV = nτ: equation of state: relates observables with the system (pressure,
volume, temperature).

pV = νRT, TdS = pdV + dE. Therefore dS = P/T dV + dE/T. Since E = E(T,V),
dE = ∂E/∂T dT + ∂E/∂V dV. So dS = nR/V dV + 1/T (∂E/∂T dT + ∂E/∂V dV).

So dS = (νR/V + 1/T ∂E/∂V)dV + 1/T ∂E/∂T.

S = S(T,V). Also a state function. So we can write dS, therefore, as:

∂S/∂T dT + ∂S/∂V dV = ... ⇒ ∂S/∂T = νR/V ∂E/∂V + 1/T; ∂S/∂V = 1/T ∂E/∂T.

Working through the math,

∂²S/∂V∂T = 1/T² ∂E/∂T + 1/T ∂E/∂V∂T = 1/T ∂E/∂V∂T.

Specific heats: ∂Q/∂T while holding various parameters constant.

Adiabatic vs. isothermal expansion. γ ≡ C{p}/C{v}.

<a name='12'></a>

Physics 112: Statistical Mechanics
==================================
Macroscopic Thermodynamics. Feb 15, 2012
----------------------------------------

Recap of last time: we proved that the internal energy of an ideal gas was
a state variable.

Maxwell relations and their proof: from τdσ = dU + pdV,
	* U = U(σ,V) ⇒ dU = τdσ - pdV
	  + Internal energy
	* H = H(σ,P) ⇒ dH = τdσ + Vdp
	  + Enthalpy
	  + H = U + PV
	* F = F(τ,V) ⇒ dF = -σdτ - pdV
	  + Helmholtz free energy
	  + F = U - τσ
	* G = G(τ,P) ⇒ dG = -σdτ + Vdp
	  + Gibbs free energy
	  + G = U - PV + τσ

exact differential: f = f(x,y) ⇒ df = (∂f/∂x)dx + (∂f/∂y)dy.

For an ideal gas, we found C{p} - C{v} = k{B}N{A}. But C ≡ dQ/dt. If Q or T
were exact differentials, regardless with which path they took, we should
have had the same dQ/dT. The same for work because the first thermodynamic
law combines heat and work, and energy is an exact differential.

∂τ/∂V = -∂p/∂σ
dU = τdσ - pdV. U ⇒ dU = (∂U/∂σ)∂σ (∂U/∂V)∂V.

A necessary condition for an exact differential is that the derivatives
commute. In other words, _take the curl_.

More relations:

∂τ/∂V = –∂p/∂σ
∂τ/∂p =  ∂V/∂σ
∂σ/∂V = –∂p/∂τ
∂σ/∂p = –∂V/∂τ

We just get these from various formulations of first law of thermo (U, H,
F, G): by virtue of being exact differentials, their derivatives commute.

General relations for the specific heat:

C{V} = (∂Q/∂τ){V} = T(∂σ/∂τ){V}
C{p} = (∂Q/∂τ){p} = T(∂σ/∂τ){p}

Thus C{v} = C{p} + τ(∂σ/∂P·∂P/∂τ)

\alpha ≡ 1/V ∂V/∂τ. "volume coefficient of expansion"

κ ≡ -1/V ∂V/∂p "isothermal compressibility"

Therefore C{p} - C{v} = Vτ(\alpha²/κ)

What's needed to calculate entropy

Use the relations shown in the previous part. All we need are C{v} and
equation of state. But C{v} is also computable using equation of state at a
given V₀.

σ(τ,V) = σ(τ₀,V₀) + ∫C{v}(τ′,V)dτ′/τ′ + ∫dV′(∂P{v}(τ₀,V′)/∂τ)

Same for internal energy.

dU = C{v}dτ + (τ∂P/∂τ - P)dV
∂U/∂τ = C{v}
∂U/∂V = τ∂P/∂τ - P.

Example van der Waals gas (particle interactions):
(P + a/v²)(v-b) = k{B}N{A}τ (v ≡ V/ν

<a name='13'></a>

Physics 112: Statistical Mechanics
==================================
Applications of Classical Thermodynamics. Feb 17, 2012
------------------------------------------------------

Heat engines, refrigerators, and Carnot cycle
---------------------------------------------
Historically very important: industrial revolution. Easy to do mechanical
work and transform to heat: mechanical, electrical. What about the
opposite? Not at the expense of machine itself: otherwise no cyclic.

Also has interesting physical importance: this was a new thing: how to
study energy? Joule showed there was an equivalence between work done and
heat released.

η = w/q₁ ≤ 1 - τ₂/τ₁. Equality holds only for quasi-static.

Carnot cycle: alternating adiabatic / isothermal expansion /
contraction. Maximum attainable efficiency for given τ₁, τ₂.

Reversibility
-------------

Entropy constant / always in equilibrium. Relaxation of constraints: if you
enforce the original constraints, and the system returns to its initial
state, it is reversible.

t{operation}, t{equilibrium}. t{o} » t{e}. Other possibility: t{e} ≫
t{o}. Also reversible. Becomes bad when these two are of the same order of
magnitude.

Clausius statement for 2nd law of thermodynamics: effectively, Carnot
engine is maximally efficient, given τ₁, τ₂. (q₂/q₁ ≤ τ₂/τ₁)

Joule-Thomson process: H = U + PV ⇒ H₁ = H₂ if dQ = 0.
μ ≡ V/C{p} (τ\alpha - 1)

<a name='14'></a>

Physics 112: Statistical Mechanics
==================================
Chemical Potential. Feb 22, 2012
--------------------------------

# Midterm
  * One page of notes. Clarification: One side of one sheet. No explicit
	ruling against oversized paper. Reasoning: it is always good to
	reconstruct what you have learned.
	+ Put things in your own terms and understand what you don't understand
	  and why you don't understand.
	  $\cdot$ There are some formulae that are useless to understand. (n_{Q}, n,
		etc.) This is not a memorizing test. I would like you to understand
		the concepts.
  * Will take about a week for grading.
  * No need for blue book. May want scratch paper if you like, but no blue
	book necessary.
# Exact differentials
  * Evolving system.
	+ Energy can be defined. Not necessarily useful.
	+ Entropy can also be defined.
	  $\cdot$ $\sigma = \log g_{t}$ only holds in equilibrium for an isolated system.
	  $\cdot$ In this case, it is well-defined by $\sigma \equiv -\sum p(t) \log p(t)$.
  * Heat transfer is not an exact differential.
# Chemical potential
  * Why is it called a potential?
  * Action mass law

Most common state is such that the sum of chemical potentials is equal to
zero. $\mu_{i} = \tau \log (n/n_{Q_i})$.

<a name='15'></a>

Physics 112: Statistical Mechanics
==================================
Chemical Potential. Feb 27, 2012
--------------------------------

Conference result (dark matter): unfortunately a negative result. A number
of groups (two in particular) claimed that they saw signals that could be
the result of WIMPs which are responsible for dark matter. MACHOs were
bad.

What we have done so far is referred to the microcanonical method (the name
does not matter). Basically, we have been counting states. With the
postulate of the H theorem, this allowed us to define entropy as $-\sum_i
p_i \log p_i$. ( Various reminders of definitions of temperature, pressure,
chemical potential. )

The system $S$ is in one state of energy $\epsilon$. How does the number of
the states in the reservoir evolve as $\epsilon$ increases? Since the two
systems are isolated, the total energy of the system is constant. As one
increases, the other decreases. Energy is directly proportional to the
number of states and inversely proportional to the probability of being in
a state.

Now we are equipped to derive the Boltzmann distribution.

We know that the number of states is $g_{R}(U_0 - \epsilon)$, where $g_R
\equiv (U_0 - \epsilon)^{3N/2}$.

$$
= A(U_0 - \epsilon)^{3N/2}
\\ = AU_0^{3N/2}(1-\frac{\epsilon}{3N\tau_R/2})^{3N/2}
\\ \Rightarrow AU_0^{3N/2}e^{-\epsilon/\tau_R}
$$

Configuration that we are looking at: state of the system
$S$.

$$Pr[S \in \epsilon ] \propto g_R(U_0 - \epsilon)$$

\begin{align}
\frac{Pr[S \in \epsilon_1]}{Pr[S \in \epsilon_2]}
= \frac{g_R(U_0 - \epsilon_1)}{g_R(U_0 - \epsilon_2)}
\\ = \frac{\exp(-\sigma_R(U_0-\epsilon_1))}
{\exp(-\sigma_R(U_0-\epsilon_2))}
\\ = \frac{\exp(-\frac{\epsilon_1}{\tau})}
{\exp(-\frac{\epsilon_2}{\tau})}
\end{align}

$$
Pr[S \in \epsilon] = \frac{e^{-\epsilon/\tau}}{\sum_s e^{-\epsilon
s/\tau}}
\\ (z \equiv \sum_s e^{-\epsilon s/\tau})$$

$z$ is known as the partition function.

So let me take a two-level system, where state 1 has $\epsilon = 0$, and
state 2 has energy $\epsilon$.

So the probability of being in state 1 is $\frac{\exp(-0/\tau)}{1 +
\exp(-\epsilon/\tau)} = \frac{1}{1 + \exp(-\epsilon/\tau)}$.

Likewise, the probability of being in state 2 is $\frac{\exp(-\epsilon/\tau)}{1 +
\exp(-\epsilon/\tau)} = \frac{1}{\exp(\epsilon/\tau) + 1}$.

As I increase the temperature, I can excite the system, and at some
temperature, the two states are equiprobable with 50%. 

The second example we will take is the Maxwell distribution, where a
particle in a gas in contact with a reservoir (which can be the rest of the
gas). To be continued on Wednesday.

<a name='16'></a>

Physics 112: Statistical Mechanics
==================================
Boltzmann Distribution. Feb 29, 2012
------------------------------------
5.1 Constant number of particles
================================
Boltzmann factor
----------------
Recall: two-state system, we could write down the Boltzmann
distribution. Note that heat capacity will peak when there is a maximum
change in state ($C_V = \pderiv{Q}{T} = \pderiv{U}{T}$.)

Let's go back a bit and try to understand where this equation is coming
from. Why does the probability that S in a quantum state energy $\epsilon$
decrease exponentially with $\epsilon$? As you increase $\epsilon$, since
the total energy $U_R$ is fixed, the energy and number of states in the
reservoir decrease (conservation of energy).

* Examples

Free particle at temperature $\tau$. Assumption: no additional degrees of
freedom (no spin, not a multi-atom molecule).

$\text{Pr}[dV , p+dp, d\Omega] = \frac{\sum \exp(-p^2/(2M\tau))}{Z}$

That's where we're using our recipe (result that we derived before) that
the density of states in phase space is merely $\frac{1}{\hbar^3}$. So the
number of states in a differential volume element is $\frac{dV d^3p}
{\hbar^3}$. Define $d^3p \equiv p^2 dp d\cos\theta d\phi$ (further defining
$d\Omega \equiv d\cos\theta d\phi$, where $\Omega$ is the solid angle
moment), i.e. convert to spherical coordinates. The above probability thus
reduces to $\frac{1}{Z} \exp(-p^2 /(2M\tau)) \frac{dV p^2 dp d\Omega}
{\hbar^3}$.

Normalizing to N particles (i.e. choosing $Z$ such that this sum is 1)
yields $f(v)dv d\Omega = n\left(\frac{M}{2\pi\tau}\right)^{3/2}
exp\left(-\frac{Mv^2}{2\tau}\right)v^2 dv d\Omega$. Note that $\hbar^3$
disappeared entirely. Important distribution, Boltzmann (we often call it
the Maxwell distribution).

Why does the Maxwell distribution have a $v^2$ term? It's a result of the
Jacobian matrix, which effectively tells us that the density of quantum
states per unit velocity interval in the system $S$ goes to zero as $v^2$
when $v$ goes to zero. Only works when the reservoir is very big relative
to the system. Cannot possibly be from the normalization, since this is a
function of $v$.

Notice that the slope of $f(v)$ is zero at $v=0$, whereas the slope of
$f(\epsilon)$ is $\infty$ at $v=0$.

Why doesn't the system S stay in a state of energy $\epsilon$? Continuous
exchange between $S \leftrightarrow R$ of excitations of energy
$\tau$. Thoughts: Uncertainty principle technically governs everything, but
that's not particularly useful. Each excitation in the reservoir will have
a typical energy $\approx \tau$. Thermal fluctuations of the order of
\tau. Difficult to get. $\epsilon \gg \tau$, $\text{Pr}[\epsilon]
\propto \exp(-\epsilon/\tau)$

With an electron cloud (since those are fermions), you have some more
complicated physics going on, but you have a Fermi gas, and you will be
exchanging energy on the order of $\tau$. In a crystal or a solid, you will
exchange phonons with energy on the order of $\tau$. Regardless of what
system you have, you are exchanging quantum energy packets on the order of
$\tau$.

Partition  function
-------------------
$Z = \sum_s \exp(-\epsilon_s/\tau$. Let's see, then, that we can compute
that. We can ask ourselves, what is the mean energy of the system? $U =
\avg{\epsilon} = \sum_s \frac{\epsilon_s e^{-\epsilon_s/\tau}}{Z}$. But
look, think about what $\pderiv{\log Z}{\tau}$ will look like.

Aside: we still have time to do the entropy.

$\sigma = -\sum p_s \log p_s = -\frac{\sum
e^{-\epsilon_s/\tau}}{Z}\left[-\frac{\epsilon_s}{\tau} - \log z\right]$.

What you see is just $\sum \frac{1}{\tau}\frac{\epsilon_s e^{-\epsilon_s
/\tau}}{Z} + \log Z = \frac{U}{\tau} + \log Z = \pderiv{\tau\log Z|}{\tau}$

$F = U - \tau\sigma = -\tau\log Z$.

[ done for the day. Fairly powerful tool. ]

Ideal gas (again!)
------------------
 * Entropy = Sackur-Tetrode formula

5.2 Exchange of particles
=========================
Gibbs factor
------------

Grand Partition Function as a calculation tool [ Gibbs Sum (grand canonical methods) ]
-------------------------------------
A very powerful tool. More technical, but important.

5.3 Fluctuations
================

<a name='17'></a>

Physics 112: Statistical Mechanics
==================================
Partition Function. Mar 2, 2012
-------------------------------

# Midterm
  * Office hours
# Partition function as computational tool
# Ideal gas

We are looking at a totally different method of computing entropy. Instead
of the microcanonical method -- counting states (impose U; difficult), Then
we are putting the system in contact with a reservoir. We came to the
conclusion that $\prob{i} = \frac{1}{Z}e^{-\epsilon_i/\tau}$. So that's a
totally different method, which tends to be much easier.

From what you have seen, it is quite easy to get ahold of the thermodynamic
quantities you know of.

$$
\sigma = \pderiv{\tau\log Z}{\tau}
\\ F =  U - \tau\sigma = -\tau\log Z \implies \sigma = -\pderiv{F}{\tau}
\\ U = \avg{\epsilon} = \sum \epsilon_i p_i = \tau^2 \pderiv{\log Z}{\tau}
= -\tau^2\pderiv{\frac{F}{\tau}}{\tau}
$$

Examples
--------

Consider a two-level system with energies 0 and $\epsilon$. $Z = 1 +
e^{-\epsilon/\tau}$, trivially. Therefore $U = \tau^2\pderiv{\log z}{\tau}
= \tau^2\frac{\frac{1}{\tau^2}e^{-\epsilon/\tau}}{1 + e^{-\epsilon/\tau}} =
\frac{1}{e^{\epsilon/\tau} + 1}$.

Now, for an ideal gas: $Z = \sum_s e^{-\epsilon_s/\tau} = \int \frac{d^3q
d^3p}{\hbar^3}e^{-\epsilon}{\tau}$. Phase space integral. Things are very
simple.

This is equivalent to $\frac{V}{\hbar^3}\int dp_x e^{-p_x^2/2M\tau} dp_y
e^{-p_y^2/2M\tau} dp_z e^{-p_z^2/2M\tau} = \frac{V}{\hbar^3}\left(
\sqrt{2\pi M\tau}\right)^3 = V\left(\frac{2\pi M\tau}{\hbar^2}\right)^3/2 =
n_Q$.

$\avg{\epsilon} = \frac{3}{2} \frac{\tau^2}{\tau} = \frac{3}{2}\tau$

The power of $Z$ is that either you can do these sums very easily
(e.g. geometric series), or the terms grow so fast that you can just take
the first term, or you can use the integral approximation as we have done
here.

Harmonic Oscillator
-------------------

$E = \sum e^{-s\hbar\omega/\tau} = \left(\sum e^{-\hbar\omega/\tau}
\right)^s = \frac{1}{1 - e^{\hbar\omega/\tau}}$

These are known as the canonical methods, which are fairly powerful. I may
come back to this question of density of states. I have probably told you
enough on how to sum over discrete states. We may come back when we review
the material.

I have spoken long enough about this fairly technical thing. Let's ask
ourselves how to extend this to multiple systems (e.g. 2).

The partition function of 2 systems is merely the product if the systems
are distinguishable, and the product divided by $2!$ (approximately) if
they are indistinguishable. Consider indistinguishability of "quantum
states", where each state is a system.

Therefore if we have N indistinguishable systems, $Z(N) \approx \frac{1}
{N!} Z(1)^N$. This is a low occupation number approximation due to Gibbs.

$$Z_1 = e^{-mB/\tau} + e^{mB/\tau} = 2\cosh\frac{mB}{\tau} \\ Z = Z_1^N =
2^N\cosh^N\frac{mB}{\tau} \implies U = -NmB\tanh\frac{mb}{\tau}.$$

Thus $M = \frac{U}{BV} = nm\tanh\frac{mB}{\tau}$.

[ curie temperature: where M disappears ]

* Why is the division of the product by N! approximate?

As mentioned earlier, this is a low concentration approximation, i.e. the
probability of having two systems in the same state is negligible. The
error we accumulate is due to fewer terms appearing in the sum.

In other words, we have very weak correlation coefficients.

<a name='18'></a>

Physics 112: Statistical Mechanics
==================================
Ideal gas, Gibbs distribution: Mar 5, 2012
------------------------------------------
Ideal Gas
=========

We previously focused on the partition function, which is $\sum_s
e^{-\epsilon_s/\tau}$. This so-called "canonical" method is much simpler,
usually, than counting states with the constraint that energy is fixed. So
that's the advantage of that method, and so, from the partition function by
appropriate derivatives (usu. of the log), you can get all the quantities
that you like (energy, entropy, free energy, chemical potential, pressure,
and so forth).

If I have $N$ systems, $Z = (Z_1)^N$ (if the systems are distinguishable),
and $Z \approx \frac{(Z_1)^N}{N!}$ if the systems are indistinguishable. We
discussed last time why this is an approximation: sparseness of states.

For the ideal gas, we found that $Z = Vn_Q$, where $n_Q\equiv \parens{
\frac{M\tau}{2\pi\hbar^2}}^{3/2}$. This is $\approx \frac{1}
{\lambda^3}$. So this is really a quantum density satisfied by putting
particles a wavelength apart, and I cannot do much better than that.

If I apply the Gibbs recipe there, what I get is that $Z_N =
\frac{1}{N!}\parens{Vn_Q}^N$. So $\log Z_N = N\log(Vn_Q) - \log N!$. We
use the Stirling approximation to say $\log N! \approx N\log N - N$. Thus
$\log Z_N = N\log(\frac{n_Q}{\frac{N}{V}}) + N = N\log \frac{n_Q}{n} + N$.

When we introduce free energy, we have $F = -\tau\log Z$; $p =
-\pderiv{F}{V}$; $\sigma -\pderiv{F}{\tau}$.

Barometric equation
-------------------
Assume the atmosphere has constant temperature. How does the density
decrease with altitude z? The way the book does it is $\mu = \text{const}$, since
we are in thermal equilibrium. But $\mu$ has two pieces: the internal
chemical potential ($\tau\log\parens{\frac{n}{n_Q}}$) and external chemical
potential, which is just the potential in the gravitational field, namely
$mqz$. This has to be constant, which implies that $n = n_0\exp\parens{
-\frac{mqz}{\tau}}$.

The problem with this derivation is that it is at a very high level. We
need to invoke the chemical potential. Very similar problem to density of a
centrifuge, or density of ions in the membrane of a cell.

This is one way of doing things. There are actually two other ways of doing
things.

Single-particle occupancy of levels at different altitude
---------------------------------------------------------
Instead of considering the atmosphere to be in equilibrium, I would
ask myself (the more intuitive way of doing it), what is the probability
that a given molecule is at the altitude $z$? I (Sadoulet) would say that
$\epsilon = \epsilon_k + mgz$ (energy is kinetic energy + potential
energy). The probability of being at the altitude $z$ would be proportional
to $\exp\parens{-\frac{\epsilon_k + mgz}{\tau}}$. The density, therefore,
has to be proportional to $\exp\parens{-\frac{mgz}{\tau}}$.

The problem with these two derivations is that they do not generalize very
well to the point where you are not in equilibrium.

Hydrodynamic equilibrium
------------------------
The third way of doing it (which you have likely done in Physics 7) is to
consider a slab of thickness $dz$ and consider the hydrodynamic
equilibrium. The force pushing up on this slab is $pA$, whereas the force
pushing down on the slab is $(p + dp)A$. Our slab has a certain mass and
particle density, and so the downward force (due to gravity) is $nmAz
g$. Putting that all together, we have $pA - (p + dp)A = nmgzA$. This leads
directly to $\frac{1}{n}\deriv{p}{z} = -mg$. This is totally general. If we
have $pV = N\tau$, $p = \frac{N}{V}\tau = n\tau$. Since $\frac{\tau}{p}
\deriv{p}{z} = -mg \iff \frac{1}{n} \deriv{n}{z} = -\frac{mg}{\tau} \implies
p \sim \exp\parens{-\frac{ngz}{\tau}}$. This generalizes to the case when
the temperature is not constant.

(various clicker questions)

Grand partition function: $\sum_{S,N} \exp\parens{-\frac{\epsilon(N) - \mu
N}{\tau}}$

Gibbs Distribution
==================
Exchange not only energy, but also particles.

<a name='19'></a>

Physics 112: Statistical Mechanics
==================================
Gibbs Distribution: Mar 7, 2012
-------------------------------
The mathematics of the Gibbs distribution is not difficult so much as
complicated. What is difficult is determining what phenomena this
explains.

$$\prob{S \in \epsilon_s(N_s), N_s} \propto g \propto \exp
\parens{-\frac{\epsilon_s(N_s)}{\tau}} \exp\parens{\frac{\mu}{\tau}}
\\ = \frac{1}{z} \exp\parens{-\frac{\epsilon_s - \mu}{\tau}}
\\ z \equiv \sum \exp\parens{-\frac{\epsilon_s - \mu}{\tau}}
$$

We call this the Gibbs distribution (z is, as we recall, the grand
partition function).

Often, chemists prefer to consider chemical potential $\lambda_i \equiv
\exp \parens{\frac{\mu_i}{\tau}}$. 

This is weak interaction. What it means is that as we keep adding particles
at the quantum level, we don't change the wave function. They don't care
how many particles are in the system.

Often, we will simply use $\prob{\epsilon_s} = \frac{1}{z}\exp \parens
{-\frac{(\epsilon_s - \mu)N}{\tau}}$.

A common problem with this distribution, by the way, is that we are
extremely general, and sometimes it is difficult to know what this
represents in practice, so we should take examples and try to think about
the examples to consider what these mean in practice.

Maybe the simplest example I can take is a Fermi-Dirac distribution. Let us
consider an energy level $\epsilon_s$, and I have a fermion, which has a
half-integer spin, e.g. an electron (spin $\frac{1}{2}$). If we listen to
Pauli, at most one fermion can occupy each state.

Therefore $N_s \in \{0,1\}$. $\prob{N_s=0} = \frac{1}{z}$; $\prob {N_s=1} =
\frac{1}{z} e^{-(\epsilon_s-\mu)/\tau}$. So $z = 1 + e^{-(\epsilon_s-\mu)/
\tau}$. Plugging this back in, we have $\prob{N_s=0} = \frac{1}{1 + e^{
-(\epsilon_s-\mu)/ \tau}}$; $\prob {N_s=1} = \frac{ e^{-(\epsilon_s-\mu) /
\tau}}{1 + e^{-( \epsilon_s-\mu)/ \tau}} = \frac{1} {e^{( \epsilon_s -
\mu)/\tau} + 1}$. Examples: gas absorption: heme in myoglobin, hemoglobin,
walls. Energy bands of materials (bandgaps).

Determining $\mu$, when considering hemoglobin and stuff. All we need is
the density of $O_2$ in the blood. So how can we compute this? Remember
what we said about mass action law. If we are a dilute system of particles,
they will have the same properties as the gas: they will barely interact
with each other, so states will be independent, and we can then apply the
ideal gas approach.

We can also apply this to our dissolved gas, and $\mu_{gas} = \tau\log
\frac{n}{n_Q}$. This is an ideal gas in the sense of weakly-interacting
n-body system.

Chemists and biologists like to put the pressure, since the partial
pressure is something you can measure easily. Langmuir adsorption isotherm:
$f = \frac{p}{\tau n_Q\exp\parens{\frac{\epsilon}{\tau}} + p}$.

Aside: Pauli was an enormous guy, German/Swiss physicist. Very bright but
very unforgiving. Lack of understanding: not a question.

Adsorption: fraction occupied $= f$. Same form as Fermi-Dirac. Adsorption
dependence on $\mu$ can clearly be observed to be positive: as $\mu$
increases, the fraction of occupied sites increases. However, as $\tau$
increases, the fraction of occupied sites decreases. (binding energy:
$-\epsilon$)

Ionized impurities in a semiconductor: K&K p370. Doping. Donor: tends to
have one more electron; acceptor: tends to have one fewer electron. $\mu$
(Fermi level) determined by electron concentration in semiconductor.

<a name='20'></a>

Physics 112: Statistical Mechanics
==================================
Gibbs Grand Partition Function: Mar 9, 2012
-------------------------------------------
Gibbs grand partition function, fluctuations, what is minimized when a
system is in thermal equilibrium with a bath?

Next midterm is Monday, March 19.

I would like to move the third midterm from April 20 to April 13 for two
reasons: one, it's a week before we finish; two, allows me to go to a small
workshop in Davis. Interesting workshop, announced at last minute, purpose
is to try to understand what the LHC tells us about dark matter.

There was an announcement by Fermilab that they may have seen the
Higgs. CERN might have seen the Higgs. Not convinced by announcements so
far: more publicity than anything else.

Let's go rapidly through the grand partition function. Remember, we were
speaking of a system, which was exchanging with a reservoir both energy and
particles. What we had shown was that $\prob{\epsilon_s(n)} = \frac{1}{z}
\exp (-\frac{\epsilon-\mu N}{\tau})$, $z = \sum_{s,N} \exp(-\frac{\epsilon
- \mu N}{\tau})$. In most cases, we'll have $\epsilon_s(N) = \epsilon_s
N$. So that's the Gibbs formalism. Almost exactly in the same way as in the
Boltzmann formalism, we can deduce a number of things about the derivatives
of the log of this partition.

For instance: taking into account one species, $\avg{N} = \sum_{s,N}
\frac{1}{Z} N\exp (-\frac{\epsilon_s(N)-N}{\tau})$. See, if I were to take
$\pderiv{\log Z}{\mu}$, I would have $\sum_{s,N} \frac{N}{\tau}\exp (-\frac
{\epsilon_s(N)-N}{\tau})$. And so $\mu = \tau\pderiv{\log Z}{\mu}$.

So let's take two examples: Fermi-Dirac distribution.

Fermions versus bosons: fermions have half-integer spins, follow
Fermi-Dirac distributions; bosons have integer spins, follow Bose-Einstein
distribution.

So in the Fermi-dirac, we have $\avg{N} = \tau \pderiv{\log Z}{\mu} =
\frac{\exp(-(\epsilon-\mu)/\tau)}{1 + \exp(-(\epsilon-\mu)/\tau)} =
\frac{1}{\exp((\epsilon-\mu)/\tau) + 1}$.

Bose-Einstein: $z = \sum_N e^{-\frac{(\epsilon-\mu)N}{\tau}}$. You
recognize this is a geometric series and is thus equal to
$\frac{1}{1-\exp(-(\epsilon-\mu)/ \tau)}$. $\avg{N} = \tau\pderiv{\log Z}
{\mu} = \frac{\exp((\epsilon-\mu)/\tau)}{1 - \exp((\epsilon-\mu)/\tau)} =
\frac{1}{\exp((\epsilon-\mu)/\tau) - 1}$

Note that as $\epsilon-\mu \to 0$, this quantity diverges: Bose-Einstein
condensation. On the other hand, for a Fermi-Dirac distribution, this
converges to 1.

Just pay attention to $\sigma = \sum_{s,N}p_{s,N}\log p_{s,N}$. I will put
into this expansion my Gibbs factor $\frac{1}{Z}\exp(-\frac{-\epsilon_s(N)
- \mu N}{\tau})$.

$$
\log z + \sum_{s,N} p_{s,N} \frac{\epsilon_s(N)}{\tau} - \sum_{s,N} p_{s,N}
\frac{\mu N}{\tau}
\\ = \log Z + \frac{\avg{\epsilon_s}}{\tau} - \frac{\avg{N}\mu}{\tau}
\\ = \pderiv{\tau\log Z}{\tau}
$$

You have to be careful. The formulae are different with the grand partition
as opposed to without the partition function. $\Omega \equiv F - \sum_{\mu_i}
\avg{N_i} = -\tau\log Z$.

Note that $\sigma = \pderiv{\tau\log Z}{\tau}$ while $\Omega = -\tau\log Z$
as a result of the thermodynamics identity.

Fluctuations
------------
Actually, we started to speak about what I am going to say. There are
fluctuations when we are exchanging particles or energy with the
reservoir. The number, the energy is not fixed, and if I am exchanging
particles, they fluctuate. I told you about the mean number of particles
there; we spoke before abotu the mean energy. But now we can try to compute
the variance (or root-mean-square/standard deviation) of this quantity.

For instance, you remember that for a Boltzmann distribution (not
exchanging particles, so I don't need the grand partition function),
$\avg{E} = \tau^2\pderiv{\log Z}{\tau}$. The variance, you should remmeber,
is simply $\sigma_E^2 = \avg{E^2} - \avg{E}^2 = \sum \epsilon_s^2
e^{-\epsilon_s/\tau} - \parens{\sum \epsilon_s e^{-\epsilon_s/\tau}}^2$. If
you differentiated this expression with respect to $\tau$, you got this
expression, which was this elegant, if not beautiful formula $\avg{N} =
\tau\pderiv{\log Z}{\mu} = \tau^2\pderiv{\log \avg{E}}{\tau} = \tau^2
\pderiv{\tau^2 \pderiv{\log Z} {\tau}}{\tau}$.

So $\sigma_N^2 = \avg{N^2} - \avg{N}^2 = \tau \pderiv{}{\mu}
\parens{\tau\pderiv{\log Z}{\mu}}$.

Let me quickly do my calculations for my Fermi-Dirac and Bose-Einstein
distributions, considering $\sigma_N$. So I have to take $\sigma_N^2 =
\tau\pderiv{\avg{N}}{\mu}$. So for Fermi-Dirac, we have $\frac {e^
{(\epsilon -\mu)/ \tau}}{e^{(\epsilon-\mu)/\tau} + 1} = \avg{N}(1-\avg{N})$.

Note that the variance is actually less than $N$, so less than the Poisson
distribution.

If I were to do the same thing for the Bose-Einstein distribution, I would
get $\avg{N}\parens{1 + \avg{N}}$. So the fluctuations at N = 0 are
absolutely enormous.

So we say that the Bosons like to travel in flux.

Physicist joke: astronomers are fermions, particle physicists are bosons.

<a name='21'></a>

Physics 112: Statistical Mechanics
==================================
What is Minimized; Black Body: Mar 12, 2012
------------------------------------------
Housekeeping
============
Remember that we have a midterm next Monday. Some material is in the
book. The next midterm would be Friday (April 13/14, depending on which is
Friday).

Today, office hours moved to 1:30-2:15. Review session on Saturday.

What is minimized?
==================
Would like to start by asking you a question: in the conditions we have
been speaking about (system s in contact with reservoir), exchanging only
energy, does it go to a state of minimum energy? No; remember the constant
exchange of energy (constant kicking, so to speak).

Contrary to a system which is able to lose energy to vacuum, Does not
evolve to state of minimum energy. Contrary to an isolated system, does not
evolve to a configuration of maximum entropy (entropy of combination of
reservoir and system is maximized).

Evolves to a configuration of minimum Free Energy ("balance between
tendency to lose energy and to maximize entropy")

Landau Free Energy & Enthalpy
-----------------------------
More rigorously: We cannot defint he temperature of the system out of
equilibrium. So we introduce $F_L(U_S) \equiv U_S \tau_R\sigma_S(U_S)$
(Landau Free Energy; constant volume) and $G_L(U_S, V_S) \equiv U_S
\tau_R\sigma_S(U_S,V_S) + p_RV_S$ (Landau Free Enthalpy; constant
pressure). The difference between ordinary free energy and the Landau free
energy is that the ordinary free energy is a function of the system $S$
that is only defined at equilibrium, whereas Landau Free Energy is defined
everywhere.

What we want to show that this $F_L$ is the value that is maximized. We can
simply count states.

$\sigma_{tot}(U_S) = \sigma_R(U-U_S) + \sigma_S(U_S) = \sigma_R(U) -
\pderiv {\sigma_R}{U}U_S + \sigma_S(U_S) = \sigma_R(U) - \frac
{1}{\tau_R}U_S + \sigma_S = \sigma_R(U) - \frac{1}{\tau_R}F_L(U_S)$

The most probable configuration maximizes $\sigma_{tot}$, which minimizes
$F_L$. Note that this implies that $\pderiv{F_L(U_S)}{U_S} = 0 \iff \pderiv
{\sigma_S(U_S)}{U_S} = \frac{1}{\tau_R}$ (by the definition of Landau free
energy).

When minimized, temperature of system is equal to temperature of reservoir.

Landau Grand potential
----------------------
If we exchange particles, what is minimized is $\Omega_L(U_S,N_S) \equiv
U_S - \tau_R\sigma_S(U_S,N_S) - \mu_R N_S$ (the Landau Grand Potential).

This will be useful when we do phase transitions. They get interesting in
statistical mechanics, and people are using this Landau Free Energy.

Aside
=====
This completes the material for the midterm. Since I do not like to
emphasize memorization, this time is that you get two pages (one sheet
double-sided) of notes of formulae. The main thing is not the formulae, but
rather how to apply them. So many formulae now that if you apply them now,

Black Body radiation
====================
Let us begin with the Planck distribution.

Usual way to consider a gas of photons in thermal equilibrium. (take
$\omega \equiv 2\pi v$) Let's think of it in a single mode of cavity, and
consider the number of photons in that mode. Harmonic oscillation:
$\omega$. If I have s photons in this mode, the energy would be $\epsilon
\equiv s\hbar\omega$; $s \in \mathbb{Z_+}$. So $Z = \sum_s e^{-s\hbar\omega
/ \tau}$, roughly. So $\avg{S} = \frac{\tau^2}{\hbar\omega} \pderiv{\log Z}
{\tau} = \frac{e^{-\hbar\omega/\tau}}{1 - e^{-\hbar\omega/\tau}} -
\frac{1}{e^{\hbar\omega/\tau} - 1}$. So $\avg{\epsilon_\omega} = \frac{\hbar
\omega}{e^{\hbar\omega/\tau} - 1}$

Two quantifications: first quantification (wave-like): discrete states in
massive particles; obvious cavity modes for photons. The second
quantification was of discrete particles: it was reversed -- it was obvious
that massive particles were quantized as discrete particles, but not so
much that photons were quantized in numbers -- Planck.

Questoin: why is the mean energy per mode decreasing with energy? For
$\hbar\omega > \tau$, it is more nad more difficult for the bath to create
a photon: I need $\hbar\omega$ to create a photon, and if it's too large, I
don't have enough energy available.

Photon properties. Maxwell equations in vacuum.

Mean energy density: Is $\hbar\omega$ the mean energy density as a function
of frequency? No; we have to fold in the frequency density of the modes
$D(\omega)d\omega$ which can be computed with our $\frac{1}{h^3}$ rule.

The density of states is $2\frac{d^3xd^3p}{h^3}$. (2 is the polarisation
factor) Note that $pc = \hbar\omega$, and $d^3p = p^2 dp d\Omega$. So our
density is $\frac{2d^3x(\hbar\omega)^2\hbar d\omega d\Omega}{c^3
\hbar^3}$. We can use the fact that $\hbar^3 = \frac{1}{8\pi/3}$. If we are
not interested in the direction of the photons, we integrate on solid angle
and we get $u_\omega d\omega = u_vdv = \frac{8\pi hv^3dv} {c^3\parens
{\exp\parens{hv/\tau} - 1}}$. I would like you to be able to derive this
from first principles, rather than rote memorization.

<a name='22'></a>

Physics 112: Statistical Mechanics
==================================
Black Body: Mar 14, 2012
========================
Office hours: today from 3:30-4:30; extra at Friday from 3-4.

Review Saturday @ 10:30.

Black Body
=========
Radiation energy density between $\omega$ and $\omega+d\omega$? 

Would like to rederive black-body law in a slightly different way. Recall:
speaking of photons in equilibrium with a metallic cavity. In that case,
the average number of photons at frequency $\omega$ is $\frac{1}{e^{\hbar
\omega/\tau} - 1}$. The minus is coming from the fact that we have a boson,
the spin of which is 1. Some of you are more comfortable with $\nu = \frac
{\omega}{2\pi}$, in which case the energy is $\frac{1}{e^{\hbar
\nu/\tau} - 1}$.

We can write $u_\nu(\nu,\theta,\phi) 2\frac{d^3xd\nu d\Omega}{h^3} =
\avg{s}h\nu 2\frac{d^3xd^p}{h^3}$ (we need to pull out this factor of two
to account for the polarization). We can then use that $p = \frac{\epsilon}
{c} = \frac{h\nu}{c}$. If I'm not interested in the direction, I have to
integrate over the angles, which gives me a factor of $4\pi$, and so our
net result is $u_\nu(\nu)d^3xd\nu = \frac{8\pi h\nu^3d\nu d^3x}{c^3(e^{h
\nu/\tau}-1)}$

Cosmic microwave radiation
--------------------------

Example of most perfect black body that we know: photons in equilibrium in
early universe. In the early universe, the tempmerature was over 3000 K. We
had mostly $p + e^-$ at that time. The mean free path was very low; protons
interacting with electrons. So what you had was a plasma; effectively
opaque to photons -- very high scattering. At about 3000 degrees, universe
then becomes transparent: hydrogen forms, and photons don't scatter.

So all around us, we see this radiation (discovered in the 60s), and it is
no longer at this temperature. The radiation has been shifted and is now at
about 3K -- in microwave band; roughly mm wavelength.

Difficult to make black body radiator to calibrate instrument: primary
limiting factor.

Fluctuations of temperature are $10^{-5}$ of mean temperature. You can
measure these as frequencies. You get this marvelous spectrum with wiggles,
and we see the plasma vibrating, in some sense. This gives us a lot of
information: tells us that the universe is especially flat; tells us the
amount of protons and neutrons in the universe; tells us the amount of dark
matter.

Allows us, for instance, to look at a lot of cosmology parameters.

We can also measure polarization; gravitational potential waves shaking
this plasma.

These fluctuations are (difficult to prove) responsible to the formation of
structure: they are responsible for the formation of galaxies.

European satellite this year named Planck, which will achieve more accurate
results.

Could lecture for over ten hours on this subject, but that is not the
subject of this class.

Planck
======

Before: physicists only considered continuum. We did not know about the
second quantization, that photons come with energy $h\nu$. Physicists of
19th century just wrote the partition function, summing over states. If you
do this, you get $\tau/\epsilon_0$, independent of frequency. The mystery
was you had to sum over modes (frequencies), and you'd get infinity. This
is a problem.

Planck introduced the quantization of states. Planck did not clearly
understand what he was saying. The photons comes in quanta of $\hbar
\omega$. Thus there is a cut-off at $\epsilon=\tau$, and so you do not have
what was called the ultraviolet catastrophe. This was 1903.

In 1905, Einstein published two articles, one which was about this
commenting on how quantization explains the photoelectric effect -- this is
why he got his Nobel prize. The same year he also published his paper on
special relativity, and so he did not have to work an 8-5 job.

Have we solved everything?
--------------------------
No: zero point energy. We have again an infinite sum. This is related to
the problem of the vacuum energy, dark energy, and the cosmological
constant.

Namely, $\epsilon_\omega = \frac{\hbar\omega}{2} + s(\hbar \omega )$. This
is related to what we consider vacuum energy, dark energy (maybe), and the
cosmological constant.

Note: important to sum instead of integrate.

Let me try to ask you why we did not use the Gibbs formalism? Photons
appear and disappear in interaction with cavity. However, this is a
different formula.

The reason why we do not use this is that the chemical potential of the
photon must be zero. Why? Special case of mass action law; entropy of the
reservoir does not change when we change the number of photons (keeping the
energy constant); and the photons is its own antiparticle.

Namely: $\mu_\gamma + \mu_e - \mu_e = 0 \implies \mu_y = 0$; $\pderiv
{\sigma_R}{N_{\gamma BB}}\bigg|_U = -\frac{\mu_\gamma}{\tau} = 0$. And
finally $\gamma + \gamma \leftrightarrow e \bar{e}$. We will see that the
chemical potential of the antiparticle is the same as that of a 

It is perfectly fine to use the Gibbs formalism; it is just that
$\mu_\gamma$ is zero.

Theme of this course: there are often three different ways of deriving the
same result: microcanonical (counting states), canonical (Boltzmann), and
grand canonical (Gibbs formalism).

Counting number of states: Kittel and Kroemer go through a painful counting
of number of states using quantum numbers. Of course, same result.

Flux through an aperture. Do not forget cosine factor: volume of oblique
cylinder is $cdtdA\cos\theta$.

<a name='23'></a>

Physics 112: Statistical Mechanics
==================================
Black Body: Mar 16, 2012
========================

As usual, housekeeping. Then comments on grand partition function. And then
we will come back to the black body approach and finish the
Stefan-Boltzmann law, speak about Kircchoff.

Wednesday moving again office hours: going to SF to participate in a
roundtable discussion between artists and scientists on the concept of
space: "how do we know that things we don't see exist?" (i.e. dark matter,
dark energy). The thing is very strange (suggested by an artist) is that
the main question is about creativity. Important for scientist, yes, but
this is not useful for invisible space; we do not create things; we are
forced to believe these things.

There has been some confusion regarding the grand partition
functions. $\frak{Z} = \sum_s e^{-\frac{\epsilon_s(N_s)-\mu
N_s}{\tau}}$. We have been using this primarily for a system of one state
$\epsilon_i$. In this case, the partition function $\frak{Z}_i =
\sum_{N_i} e^{(\epsilon_i-n_i)N_i/\tau}$. Then, we get similarly that the
average number of particles of this state is $\tau \pderiv{\log \frak
{Z}_i}{\mu}$.

Thus if we have a system with all possible states, $N = \sum \avg{N_i} =
\sum_i \tau \pderiv{\log\frak{Z}_i}{\mu_i}$. Therefore $\avg{U} =
\sum_i \tau\epsilon_i \pderiv{\log\frak{Z}_i}{\mu}$.

However, we could also approach this by considering our system to be an
ensemble of states from the start. In order to specify this, I must
specify the number of particles that have specific energies.

Rather, $\frak{Z} = \sum e^{-\frac{\sum \epsilon_i N_i - \mu\sum
N_i}{\tau}} = \prod_i(\frak{Z}_i)$.

We can then explore a bit: $\avg{N} = \tau\pderiv{\log \frak{Z}}{\mu} =
\sum_i \tau\pderiv{}{\mu}\log z_i$ (after some simple arithmetic
manipulations)

By the way, if you do it either way, you have no problem with the
distinguishability of the various states. You take that into account
automatically.

Note that this is different from the case where the system is an ensemble
of particles.

Recall: flux through an aperture requires us to integrate over an oblique
cylinder, which has area $cdtdA\cos\theta$.

$u_\omega(\theta,\phi d\omega d\Omega = \frac{\hbar\omega^3d\omega}{\pi^2
c^2(\exp(\hbar\omega/\tau) - 1)}$. This is the energy density of photons
moving in the direction $\theta, \phi$. If I'm interested in the flux
density, i.e. the brightness, there I am just looking at what happens
taking a unitary $dA$ perpendicular to the direction. We consider
$I_\nu(\theta,\phi)d\omega d\Omega dt dA = \frac{\hbar\omega^3
d\omega}{\pi^2 c^2(\exp(\hbar\omega/\tau) - 1)} cdt dA$. $I_\nu$ is just
$\frac{2h\nu^3d\nu dt dA}{c^2(\exp() - 1)}$.

With a fixed aperture, $J_\nu dA dt d\nu = \int \frac{2h\nu^3
d\nu}{c^3(\exp() - 1)} cdtdA\cos\theta d\Omega$. We have to be careful
here: we do not integrate beyond $\frac{\pi}{2}$, since those photons are
going the wrong way -- the only photons that go through the aperture are
moving toward the aperture.

So what we have finally is $\frac{4\pi h \nu^3 d\nu dtdA}{c^2(\exp(h\nu /
\tau) - 1)} = \frac{c}{4} u_\nu d\nu dA dt$. Note here that $u_\nu$ is the
energy density integrated over the solid angle.

Therefore if I am interested in the total energy in my volume, I will
integrate $\int u_\nu(\theta,\phi)d\nu d\Omega dV = \int \frac{8\pi h\nu^3
d\nu}{c^3(\exp(h\nu/\tau)-1)} = \frac{8\pi V}{h^3 c^3} \int_0^\infty
\frac{\tau^4 x^3 dx}{\exp(x)-1}$. The total energy, therefore, goes as $a_B
T^4\; a_B = \frac{\pi^2 k_B^4}{15\hbar^3 c^3}$.

Similarly, if you were to look at thte total flux through a fixed aperture,
we will do the same calculation, but now what we will get $J =
\frac{c}{4}a_B t^4 = \sigma_B t^4$.

You can also get the entropy and the number of particles by just
integration. For entropy, you can either integrate $d\sigma/d\tau$ or just
remember the density of states, which goes as $T^3$, as does the number.

Why do we have a $T^4$ for energy density but a $T^3$ for entropy or number
of photons? By the way, entropy is proportional to number of photons, which
makes sense. Mathematically, this appears as a result of change of
variables. So what is the effect that dominates? It is the increase of the
density of states with energy. Density of states goes as $\omega^2
d\omega$, which comes directly from the counting of states. Since $\omega$
is of the order of $\frac{\tau}{\hbar}$, we get here that the number goes
as $T^3$. Of course, when I'm looking at energy, I have one extra factor of
temperature ($\tau \equiv k_B T$), and that's where $T^4$ comes in.

<a name='24'></a>

Physics 112: Statistical Mechanics
==================================
Black Body: Mar 21, 2012
========================
Overview
========
Black body: Detailed balance, Kirchhoff laws

Midterm on the fifteenth. No homework due on thirteenth.

As mentioned last week, cannot be at office hours this afternoon, going to
SF for panel discussion between artists and scientists about space and the
unknown. Instead, I would like to propose office hours on Friday 3-4.

Examining of histogram. Happy about no very low grades; 7.5 points lower;
smaller spread.

There are still people in the class writing something like $\mu =
\pderiv{\sigma}{N} = \pderiv{U}{N}$ without putting any indication of what
the independent variables are. The second type of problem which seems
serious are confusions. One of these is that between isolated systems and
systems in contact with a bath. Of course, at equilibrium, the probability
of a given state is $\frac{1}{g_i}$ (H theorem), and in the second case,
they are not equiprobable and are given by the Boltzmann distribution (or
Gibbs).

Also, people assuming everything is an ideal gas. Don't do that. Putting
random formulae shows that you don't understand the problem, so you'll lose
points.

Statistical mechanics is much bigger than just **classical** ideal
gases. And it's much more than Thermodynamics identity. Those are
distortions of coming from Physics 7; you tend to write the Thermodynamics
identity over and over; we have much more powerful ways to do things: we
can compute entropy from first principles. And then people use $dU = \tau
d\sigma - pdV + \mu dN$, but people without a lash will put $U =
\tau\sigma$. Reverse-engineering, it does not work.

Also, we'll use the best two midterms out of three.

For these things, any questions? Alex has the midterms, and I will have
them on Friday.

Black Body
==========

We are in black body radiation. What I would like to focus on today is heat
imbalance. We have actually a very specific black body radiator, which is a
cavity with metallic walls. We were thinking about the modes in this cavity
and the photons in thermal equilibrium. Now, what we will do is put another
system in communication with this cavity and ask ourselves: what is the
radiation of this cavity? (these two systems are at the same temperature
and communicate through an internal aperture)

Suppose that first that the second system is a black body. By this, we mean
something that absorbs all radiation. So a cavity with a very small hole is
a very good approximation for a black body: if I send a photon into this
hole, it will not come back.

Can imagine more black bodies -- what we use in our field: rubber with a
lot of carbon in it (does not reflect, only absorbs).

By construction there, if we have these two systems communicating, the
energy emitted by one is the energy absorbed by the other.

First question, which is very simple: how does the energy emitted by system
1 compares to energy absorbed by system 1? Since they are at the same
temperature, the energy emitted by either system is the same (consider
formula derived last lecture).

**Principle of detailed balance**. Consequence: the spectrum of radiation
emitted by a black body is the "black body" spectrum calculated before.

This is a very simple argument, but very powerful. Proof: $\frac{c}{4}A
u_{BB} = \frac{c}{4}Au_{cavity} \implies u_{BB} = u_{cavity}$. Emits in an
isotopic way exactly as the cavity. We could have inserted a frequency
filter or a direction selector, and these still remain constant.

Let's modify the situation. Instead of a black body, let's consider a grey
body, and let's define an absorption coefficient $a \equiv \frac {\text
{power absorbed}}{\text{power received}}$. In principle, this could depend
on angle and frequency. So the question now that we ask ourselves is how does
the energy of a grey body compare to energy emitted by a black body?

For this, we must consider both the reflected BB energy and GB emission by
walls.

Notice that the energy received by the black body is $(1 - a)(BB) + a(BB) =
BB$. Emission coefficient = $e = \frac{\text{power emitted}}{\text{power
black body}}$. $a = e$ -- usually known as Kirchhoff law. The black body
receives back exactly what it emits. Therefore its temperature stays
constant.

Very useful in many applications. At the basis of the Nyquist noise or
Johnson noise. We will come back to this. You can show that the amount of
power emitted $U d\nu = 4kTRd\nu$. This is explained not very well, I'm
afraid, in Kittel and Kroemer, but this is the cause for many sources of
noise in our electronic circuits. More specifically, a theorem known as the
dissipation/noise theorem: any system capable of absorbing radiation is
making noise: if it absorbs radiation and has constant temperature, it will
have to emit *something* to stay at constant temperature. This is deeply
ingrained in quantum mechanics: anything that absorbs emits.

In order to detect anything, we absorb energy. And because we absorb
energy, we must emit energy.

There are many applications. Let me just give you an orientation. In many
cases, in all the sensing applications, we can say that we are at least
roughly a black body radiator, which has a certain surface area $A_e$, and
we are looking at it with some sort of telescope with a certain reception
area $A_r$. There is a simple relationship if the distance is $d$. The
source is seen from the receptor to fill a solid angle $\Omega_r$, which is
basically, for small angles, just $\theta^2$. Similarly, the solid angle as
seen by the emitter is $\Omega_e = \frac{A_r}{d^2}$; likewise, $\Omega_r =
\frac{A_e}{d^2}$, and so if you take the ratio of the two, you have
$\frac{\Omega_e}{\Omega_r} = \frac{A_r}{A_e}$. Purely from geometry, but an
important result.

If we have something that is diffraction-limited, then $\Delta \theta \sim
\frac{\lambda}{R}$. This means that $\Omega_r \approx \Delta\theta^2 \sim
\frac{\lambda^2}{R^2}$. Since our area goes as $\pi R^2$, $\Omega_r A_r =
\lambda^2$. With these two sets of equations, we can look at various
situations in astronomy. We'll do that rapidly at the beginning of next
lecture. I will also probably speak about phonons on Friday, and we'll see
if we can start the Fermi-Dirac/Bose-Einstein.

<a name='25'></a>

Physics 112: Statistical Mechanics
==================================
Black bodies and phonons: Mar 23, 2012
======================================

What I would like to do today, if you've looked at the homework for next
week, is finish black body radiation -- in particular stars -- and to speak
of phonons in a crystal. So, uhm, let's start with a simple question: a
star like the sun is to a first approximation a black body. Is the
radiation across the disk constant, brightening at the limb, or dimming at
the limb?

Experimentally, it looks constant, roughly. Why is this?  This is coming
from the fact that for black body radiation, the radiation is
isotropic. When we ask ourselves what is the amount of light that reaches
our photodetector in a time $dt$, this is basically $u(\nu, \theta, \phi)
d\nu d\Omega dA cdt$.

So if I take my sun, essentially what is happening is that I am looking at
a radiation shell of thickness $cdt$.

So that's one way of thinking about it: does not depend on angle. Another
way of considering it: area $dA$. Whatever emerges from this area is
independent of the angle. What I receive in my eye is not proportional to
$dA$ but rather $dA\cos\theta$ ($\cos\theta$ is normal to my line of
sight).

So apparent radiation is constant all over the disk, if I have a black
body, which is radiating isotropically, where I am not depending on
$\theta$ and $\phi$. That is why the disk of the sun is basically constant
luminosity, the moon is constant luminosity.

Why are we considering the sun a black body? The black body occurs in
thermal equilibrium when the photons (of a star), at least those very close
to the edge, are scattering so much that they are in thermal
equilibrium. Basically, this is coming from the fact that the photons are
scattering very much. It is not an exact black body for the following
reason: the sun is surrounded by its corona. When photons are coming
through that region, they are absorbed at certain frequencies. We have
absorption line at certain frequencies. By the way, that's how we
discovered helium: absorption lines we had no idea existed; was discovered
by looking at the sun through a spectrograph.

Essentially, that's a black body: photons in equilibrium.

Maybe 10 years ago, there was a professor from Ohio State (or something
like that) who published a full-page ad of the New York Times (which was twice
his monthly salary) how people talking about the Big Bang don't understand
anything about anything. Whole argument was that since this is not coming
from an oven with a small hole, this was just silly. Argued that stars were
not black bodies.

It shows you that people can get very emotional spending twice two months'
salary on a full-page ad in the New York Times.


Now, an interesting question is: what happens if the sun in practice is not
also a black body with very defined edges? The density in the sun goes down
as the radius increases; one over the mean free path does something like
$\rho\sigma$. The emissivity of the sun, therefore, as a function of
radius, is 1 very close to 0, and dies off at some point. This leads to
limb darkening. And by looking precisely at the intensity as a function of
the radius, you can have an idea of the mean free path, and of therefore
the density. That is how we mapped the density at the edges of the sun.

If $u$ (energy density) is a function of the radius, then $cdt$ at the
edges has more energy than $cdt$ at the edges. There is a whole field of
stellar astronomy devoted to this kind of stuff.

So any way. This kind of simple question (why the sun appears to be of
constant luminosity despite it being a sphere) is interesting and not
totally trivial to answer. Related to the isotropic behavior of the black
body.

Solid angles and surfaces at emission/reception
-----------------------------------------------

Showed last time these simple geometric relationships. The one at the
bottom is related to refraction and comes from the fact that the angle
$\theta_D$ at some radius R goes as $\frac{\lambda}{R}$. So the solid angle
goes as $\frac{\lambda^2}{R^2}$, and the area of my detector goes as $\pi
R^2$,and so $\Omega_r A_r \sim \lambda^2$.

This has an interesting consequence. Suppose that I am looking at a totally
diffuse object, e.g. the microwave background. If I have a
diffraction-limited telescope, how does the radiation I receive depend on
the diameter of my telescope? (i.e. how does the received energy depend on
the diameter of a diffraction-limited telescope?) Does it increase or stay
constant?

It indeed stays constant, for the following reason: the portion that I see
of this diffuse object is my $\Omega_r$. Therefore the area at emission is
just $\Omega_r d^2 = A_e$. Now whhat is received is also proportional to
the solid angle of my telescope, i.e. $I_\nu d\nu \Omega_e A_e$. So that is
equal to $I_\nu d\nu \frac{A_r}{d^2} \Omega_r d^2 = I_\nu d\nu \lambda^2$.

If I am looking, however, at a point object (i.e. something significantly
small), that is not correct. That is why astronomers go for very large
telescopes; to capture as much light as possible.

So if you have a diffuse emitter, it [increasing area] does not change the
power. Size of microscope is not important in terms of power, but is
definitely important if you're trying to look at ripples from fluctuations
in temperature of microwave background. Larger telescope means more detail,
better angular resolution.

This leads to a number of interesting results. For instance: if the sun is
a black body, the amount of radiation that I get in my telescope is a
measure of its diameter. More exactly, apparent diameter (i.e. diameter
divided by distance) of the star. So let's take a star that emits power
(absolute luminosity) $L$ isotropically. If I am now trying to look at the
apparent luminosity $\ell$, this is $\frac{\text{Power received}}{\text{Area
of telescope}}$. Since our object is much smaller than the telescope, this
does depend on area of the telescope. This is the apparent luminosity. I
can compute that and say "look, my star is emitting a power L over the
whole $4\pi$ solid angle, so over my unit solid angle it emits
$\frac{L}{4\pi}$. So what do I see? $\frac{L}{4\pi}\frac{A^2}{d^2}$. So
$\ell = \frac{L}{4\pi}\frac{1}{d^2}$. So for a black body, $L = 4\pi r_e^2
\sigma_B T^4$. That's my Stefan-Boltzmann law. So $\ell = \frac{4\pi
r_e^2}{4\pi d^2} \sigma_B T^4 = \expfrac{r_e}{d}{2}\sigma_B
T^4$.

There are a number of objects that are vibrating or exploding (so they are
changing their diameters and often also their temperatures). So we can do
the same thing with supernovae. If we look at $\deriv{\ell}{t}$, we have
two terms: $\frac{2 r_e \deriv{r_e}{t}}{d^2}$ and $\frac{r_e^2}{d^2}
\sigma_B 4T^3 \deriv{T}{t}$. We can measure both of these changes over
time, so now if we make a spherical approximation, I can get
$\deriv{r_e}{t} = \deriv{r_\perp}{t} = \deriv{r_\parallel}{t}$. We can
measure this last derivative by Doppler shift. If we assume that, then we
can measure the distance. And that is how we measure distance to stars that
are too far to see parallaxes and how we are able to measure the expansion
of the universe.

Pretty clever method. It relies on this assumption, which if a star is
vibrating, is not an unreasonable assumption. It is a much less rigorous
assumption if you have an explosion, since stability varies.

We used this method for supernova 1987A to check that it was indeed (at the
same distance as) the Magellanic cloud.

Another little thing that radio astronomers do is related to the antenna
temperature. This is very simple, actually: $I_\nu d\nu dA d\Omega =
\frac{c}{c^3}\frac{2h\nu^3 d\nu}{e^{h\nu/\tau}-1}$. If $\frac{h\nu}{\tau}
\ll 1$, $e^{h\nu/\tau} - 1 \sim \frac{h\nu}{\tau}$. so this goes to
$\frac{\tau}{c^2} \nu^2 d\nu dA_e d\Omega_e$. If our telescope is
diffraction-limited, then we know that this is roughly $2\tau
\frac{\nu^2}{c^2} d\nu \lambda^2$. So $I_\nu d\nu dA d\Omega \sim 2\tau
d\nu$, which means that the amount of power received by my telescope is
$2\tau d\nu$ (independent of area of object since this is a diffuse object,
and we are diffraction-limited). So the amount of power received is just
$\tau$; $k_B T$. Antenna temperature is just amount of power at low
frequency.

<a name='26'></a>

Physics 112: Statistical Mechanics
==================================
Phonons, Quantum gases: April 2, 2012
=====================================

We have the third midterm a week from Friday. It will cover material up
through Friday's lecture.

So, phonons are vibrations in a crystal and are quantized. This means that
as before, $\epsilon_1 = \hbar\omega$, and $\epsilon_\omega =
\avg{s_\omega}\hbar\omega$. If you look at the dispersion relations,
plotting energy and momentum, $\omega, k$ (proportional by a $\hbar$
factor), in crystals there are three acoustic modes. To a first order, they
are linear at very low energy.

We will make some approximation, forget that they are of different
velocities, and just consider all the photons to have the same velocity. So
we will say the energy $E = p c_s$. Typically, this velocity is of the
order of a few kilometers per second, which is roughly $10^{-5}c$. There is
one detail we need to take into account: a crystal is not a continuous
medium. If I'm speaking of transverse phonons, I can move the atoms
transversely, and this corresponds to a certain wavelength and
momentum. It's clear that wavelengths that are too short are equivalent to
a much longer wavelength: you forget about the oscillations between the
particles. Thus $k = \frac{p}{\hbar} \le \frac{a}{\pi} = k_D$. There is a limit
which is $\frac{\hbar\pi}{a}$, which is called the Debye limit. The viable
region, therefore, is known as the Brillom zone. The corresponding
frequency is $\omega_D = \frac{a}{\pi}c_s$.

One way of thinking about it: suppose I have a crystal with N atoms, each
of which can move in three directions. I therefore have 3N degrees of
freedom. So the sum from 0 to the Debye limit of my density of states,
multiplied by the three polarizations, has to be equal to 3N. If you work
out the computation (done in the notes, with spherical approximation), we
get $c_s (6\pi^2 \frac{N}{V})^{1/3}$. This is slightly different from what
you should get, but this is merely a result of the spherical approximation.

The thing you just should remember is that there is a limit in the energy
up to the momentum due to the fact that this is not a continuous medium.

So: is the Debye temperature $\theta = \frac{\hbar\omega_D}{k_B}$ useful?
Evidently not. In the case of photons, I will get the mean occuplation
number as $\frac{1}{\exp(\hbar\omega/\tau) - 1}$. These are bosons, and
chemical potential is zero because they can disappear at the walls. If I
have a small temperature, I will excite low-energy phonons. At low
temperature, same results as the black body but replacing $c$ by $c_s
\approx 10^{-5} c$. In particular, $U = 3\int d^3 x \int_0^{p_D} \frac{d^3
p}{h^3} \frac{1}{\exp(\hbar\omega/\tau) - 1}$, and I will have a similar
result where $U$ goes as $T^4$, except we have three degrees of freedom as
opposed to two, and the velocity is different. $C \propto \frac{1}{c_s^3}
T^3$, $\sigma \sim \frac{1}{c_s^3} T^3$, $\avg{N_p} \sim \frac{1}{c_s^3}
T^3$. What you can show easily (which I will not do in detail) is that $U
\propto N\expfrac{T}{T_D}{4}$, and that $C \propto \expfrac{T}{T_D}{3}$.

Consequences: with a very small heat capacity, we can measure very small
energies with large temperatures.

We are sensitive enough to measure the difference in temperature of the
crystal when we look at some very distant, very faint radiation. These are
among the most sensitive instruments you can imagine, and this is because
the heat capacity plummets at very low temperatures. Okay, so probably
enough. The phonons behave essentially exactly as the photons. The velocity
of sound is roughly $10^{-5} c$, and there are three polarizations. Else,
almost everything else applies. The fact that we have a limit in the
momentum of the phonons due to the fact that the crystal is not continuous,
is irrelevant at low temperatures.

Do the calculation once; nothing is difficult.

Let us speak about quantum gases. This is the last chapter, which is really
at the core of the course. So let's just summarize what we did: we
basically started from the H theorem (microcanonical methods of counting
states). We can physically deduce all of thermodynamics. But you would
agree that counting states (especially when you impose restrictions) is
actually not very easy. So there was the trick that Boltzmann had invented,
which was to put the system in equilibrium with a reservoir. The whole
ensemble (reservoir + system) was isolated. We could apply once and for all
the microcanonical method, and we got that the probability of a certain
state of energy was $e^{-\epsilon/\tau}$.

We could generalize this with Gibbs if the number of particles was not
constant, i.e. the grand canonical method, where the probability of states
goes as $e^{-\frac{\epsilon-\mu}{\tau}N}$. What we then derived (either
from Boltzmann or Gibbs) was the black body radiation, where the average
number of photons $\avg{s}$ was $\frac{1}{\exp(\hbar\omega/\tau) - 1}$. I
would now like to use this method, but for particles where $\mu \neq 0$. So
we derived that the mean number of particles in a state of energy
$\epsilon$ was $\frac{1}{\exp((\epsilon-\mu)/\tau) \pm 1}$. Remember that
fermions don't blow up at $\epsilon - \mu = 0$.

There is something we will speak about, the Bose-Einstein condensation,
which is due to the fact that this fraction actually diverges.

skip density of states. How do we determine chemical potential? We compute
the mean number of particles. How do we compute this number? Integrate the
product of the average value with the density of states.

<a name='27'></a>

Physics 112: Statistical Mechanics
==================================
Fermi-Dirac/Bose-Einstein: April 4, 2012
========================================
No housekeeping.

Focus on density of states to be sure that this concept is ingrained in
your minds by now. Focus on Fermi-Dirac and basically what we will see is
that normal operating temperatures, $\tau \ll \mu$. There are a number of
interesting approximations we can make which allow us to make these
calculations.

Once again: recall that the minus sign in the Bose-Einstein distribution is
responsible for the Bose-Einstein condensation, which we will cover. There
is no divergence for the Bose-Einstein distribution because $\mu$ is
slightly negative, so we don't have to worry about the case where they are
equal.

Density of States
=================

We have $\avg{s(\epsilon)} = \frac{1}{\exp\parens{\frac{\epsilon -
\mu}{\tau}} \pm 1}$. What we have to do is sum over $g_i \avg{
s(\epsilon_i)}$. As we get further, the density of states increases. In
that case, we can replace this sum with an integral approximation (in
particular at small energy): $\int_0^\infty g(i) \avg{s(\epsilon)} D(s)
d\epsilon$. For Fermi-Dirac it does not matter much (since there are few
states of small energy, but Bose-Einstein it will matter. Therefore this
only holds for large $\epsilon$.

We know that in phase space, the number of spatial quantum states
(orbitals) is $\frac{d^3 x d^3 p}{h^3}$. I will need to multiply by some
kind of degeneracy factor $g$ (e.g. number of spin states: for an electron,
this would be equal to 2).

In order to go to $\epsilon$, I will have to integrate over space and the
angles and make the change of variables from p to $\omega$. Thus we have
$\frac{g}{h^3}\int_{\text{space}} d^3 x \int_{\text{angles}} p^2 dp d\Omega
= \frac{4\pi g V}{h^3}p^2 dp = \frac{gV p^2 dp}{2\pi^2 \hbar^3}$. Now we
must distinguish between two cases.

Non-relativistic ($\epsilon = \frac{p^2}{2m} \implies p =
\sqrt{2m\epsilon}$). Most of literature does not put volume in density of
states, since that is a trivial factor in front.

We can replace our $p^2$ by $2m\epsilon$ and $dp$ by $\sqrt{\frac{m}
{2\epsilon}}$, so we now have $D(\epsilon) d\epsilon = \frac{g}{4\pi^2}
\expfrac{2m}{\hbar^2}{3/2} \sqrt{\epsilon} d\epsilon$. If in two
dimensions, instead of $p^2 dp$ we would have $pdp$, which means that it is
constant.

In general, we are relativistic, and so $\epsilon = \sqrt{pc^2 +
m^2c^4}$. If we are ultrarelativistic, $\epsilon = pc$. If you do the
calculation for the ultrarelativistic case, it goes as $\epsilon
d\epsilon$.

Recall: we determine $\mu$ by computing the mean number of particles.
That is, $V\int_0^\infty \avg{s(\epsilon)} D(\epsilon d\epsilon$ (with this
convention). It does not really matter; just stick to _one_ convention. The
number of states is always proportional to the volume: comes from the $d^3
x$.

One interesting thing is that this gives us in the limit of small
occupation number the result of the Boltzmann distribution. In the case
where $\epsilon - \mu$ close to 0, then we have degeneracy, and this is a
fully quantum gas.

Number of particles is just a sum over energies of occupation number
multiplied by density of states (as we've determined previously). SO that's
a way you can determine $\mu$: $\mu(\tau)$ is set by the requirement that N
is the total number of particles. ($\neq$ black body $N_\gamma \alpha
\tau^3$ -- you will have to do this integral using ultrarelativistic density
of states).

The energy is also triial to get: $U = \avg{\epsilon} = V \int_0^\infty
\frac{\epsilon D(\epsilon) d\epsilon}{\exp\parens{\frac{\epsilon -
\mu}{\tau}} \pm 1}$. You will get the classical case only if you neglect
the $\pm 1$.

The entropy is not a particularly useful expression, except that for
Fermi-Dirac, it only appears in the region of the chemical potential and
goes back to zero. There is no disorder where $\avg{s} = 1$, and there is
no disorder in states that are empty. This is a theme with Fermi-Dirac: all
the action is around the chemical potential.

Similar things happen for the Bose-Einstein, but we'll come back to that.

So: for Fermi-Dirac, for $\tau = 0$, we have a perfectly square
distribution. In that case, we can trivially do the calculations: $N = V
\int_0^\mu D(\epsilon) d\epsilon$.

Let's first consider a nonrelativistic gas. In that gas, $D(\epsilon) =
\frac{g}{4\pi^2} \expfrac{2m}{\hbar^2}{3/2}\sqrt{\epsilon}d\epsilon$. I can
put that back into our expression, and we get $VA \frac{2\mu^{3/2}}{3}$.

$\mu(\tau = 0) = \epsilon_F = \text{Fermi energy}$. This goes as $\expfrac
{N}{V}{2/3} \equiv n^{2/3}$. If you take the density of free electrons in a
metal, $\epsilon_F \sim 5\text{ eV} \to \sim 4 \cdot 10^4 \text{ K}$. By
the time I am finished, I am obliged to require my electrons to have a
fairly large energy. Velocities on the order of $.003c$. This is just a
result of the Pauli exclusion principle. This I would like you to know
this. As a consequence, $4 \cdot 10^4 \gg \text{ lab temperature}$. This
approximation is quite good, in practice. So we are very close to a square
distribution.

So once I have the chemical potential, I can compute the energy, $U =
\int_0^{\epsilon_f} \epsilon D(\epsilon) d\epsilon$. I will have to
integrate $\epsilon^{3/2}$, so, if you do the math, this will give
$\frac{3}{5} N \epsilon_F = F$ -- no disorder. I can laso compute $p =
-\pderiv{F(\sigma, \tau, V)}{V} = \frac{2}{5} n \epsilon_F$ ($\sigma = 0$,
constant $\tau$).

If you are ultrarelativistic, you can do the same calculation, but you get
different coefficients and formulae. Does not matter; these are the same
idea. too many electrons in a white dwarf reaches this ultrarelativistic
limit. Becomes unstable; will collapse. Similarly for neutron stars.

Interpretation
==============
Pauli exclusion principle. Must apply Heisenberg uncertainty principle,
large relative momentum, since position is constrained to within this
lattice.

$\mu$ does not change very much with temperature, but it does change. The
distribution rounds off. Reason for slight decrease in 3 dimensions:
density of states increases with energy. When we are rounding the
distribution, what is happening is that in the tail, we have more states
available, and therefore the contribution to the integral is larger.

Origin of thermocouple effect.

<a name='28'></a>

Physics 112: Statistical Mechanics
==================================
Fermi-Dirac/Bose-Einstein: April 6, 2012
========================================
Once again, no special announcements. Midterm in a week. I will tell you
during this lecture or the next lecture where the mditerm finishes.

What we will speak first about is holes and electrons. More precisely,
hole-electron excitations.

Then we will get into crystals and speak about metals and heat capacity of
metals.

So that's the program for today.

The discussion we had at the end of the last lecture applies to not just
fermions, but any particle with half-integer spin. Cannot have more than
one particle per quantum state.

Fermi energy: ~5eV in a metal. Much much bigger than temperature in normal
conditions. To a first order, this is a square distribution ($\mu \gg
\tau$). Therefore when $\epsilon < \mu$, $\avg{s(\epsilon)} = 1$; when
$\epsilon > \mu$, $\avg{s(\epsilon)} = 0$. ($\theta(\mu-\epsilon)$). Not
exact; there is some rounding off of the distribution due to thermal
fluctuations. One of the themes of this lecture (and of the last lecture)
is that all of the action occurs around the Fermi level.

We have to finish the lecture by asking ourselves what happens when we
increase the temperature. The main thing that happens is that density of
states goes down, yes, but there is no reason for potential to stay
put (thermocouple effect!). We have to push the chemical potential slightly
down.

This applies to three dimensions; for a two-dimensional electron gas, you
can show that chemical potential is constant, and for a one-dimensional
gas, you can show that it increases with temperature.

So what am I doing here? I am taking the same graph we just showed, but now
flipping the coordinates. At zero temperature, all the states are full. We
actually speak of the sea of electrons, which is totally filled at zero
temperature.

So what happens? It increases with temperature (to first-order, you can
ignore change of potential), and it starts to round off: the sea is not
totally filled -- electrons start to pop out of the lattice, and we have
what is called a "hole". A hole is not truly a particle (it's the absence
of one, really), and in solid state we speak of "quasi-particles".

The first thing we can ask ourselves is the charge of this
quasiparticle. It has a positive charge.

Suppose I have an electric field. In some sense, I am tilting the energy:
$\epsilon = \epsilon_0 - \abs{q} V$ (where V is the electric potential, q
is the elementary charge). So if I have a field going to the right, V going
down, and the electric field is constant and positive along the x, this
corresponds to tilting.

The hole will tend to migrate toward the right; the electron will tend to
migrate toward the left.

In some sense, holes act as anti-electrons (positrons). This is how Dirac
interpreted negative energy states in the solution of his equation for
half-integer spin particles.

We have a constant number of particles. $\avg{\frac{N}{V}} = \int_0^\infty
f(\epsilon) D(\epsilon) d\epsilon$ (forgetting about temperature dependence
for now). Also equal to $\int_0^{\epsilon_F} D(\epsilon) d\epsilon$ at zero
$\tau$.

$$= \int_0^{\epsilon_F} f(\epsilon,\tau) D(\epsilon) d\epsilon +
\int_{\epsilon_F}^\infty f(\epsilon, \tau) D(\epsilon) d\epsilon =
\int_0^{\epsilon_F} D(\epsilon) d\epsilon
\\ \implies \int_{\epsilon_F}^\infty f D(\epsilon) d\epsilon = \int_0
^{\epsilon_F}\bracks{1 - f(\epsilon, \tau)}D(\epsilon d\epsilon
$$

Recall: $f$ corresponds to electrons; $1-f$ corresponds to holes. Hole-like
excitation, electron-lilke excitation.

$u(\tau) - u(0) = \int_0^\infty \epsilon f D(\epsilon) d\epsilon -
\int_0^{\epsilon_F} \epsilon D(\epsilon) d\epsilon =
\int_{\epsilon_F}^\infty \epsilon f D(\epsilon) d\epsilon -
\int_0^{\epsilon_F} \epsilon (1-f) D(\epsilon d\epsilon$. Adding zero, we
can get $\int_{\epsilon_F}^\infty (\epsilon - \epsilon_F) f D(\epsilon)
d\epsilon - \int (\epsilon - \epsilon_F) (1-f)D(\epsilon) d\epsilon$.

We can use the symmetry we had before. We can write this explicitly by
substituting the values we had for $f$, $1-f$. Holes: increasing energy
going "down"; electorns: increasing energy going "up".

So let's do, rapidly, energy band structure. Up until now, I've just
considered a gas of electrons; have not said anything about containment. In
practice, electrons are in some kind of medium, and it is easiest to
discuss crystals because then it is in a periodic medium.

In a (cubic) crystal, the atoms are regularly spaced. If you try to solve
the Schrodinger equation for this kind of periodic lattice, what you will
arrive at is that the energy is a function of the momentum (or wave
number), but there are regions of momenta where the electrons can tunnel
resonantly from one region to the next. In other words, they are free to
move if the wavelength is right. If the wavelength is not right, they will
get stuck locally.

You may have some energy band diagram. Energy gap: region of energy where
the electrons cannot propagate. So: we have several things that happen,
depending on the element that we are considering. Sometimes, the element
also has some states above the gap (conduction band) are populated. That is
what happens for metals. In some sense, this is all what we have described
so far (our Fermi sea) -- we did not have to worry about the states below
the valence band.

Mass related to the curvature is considerably smaller in crystals than the
electrons.

So the other possibility is that basically your Fermi level wants to be
inside the energy gap. In that case, you have no small temperature; no
electrons available; they're all stuck in the valence band, so you have an
insulator.

We will see later on that if you have impurity levels, you could have
bending of the bands.

Let me briefly introduce the next subject, which I was hoping to finish by
the end of the lecture, which is the heat capacity of a metal. What the
heat capacity will be just $\pderiv{U}{T} = V\pderiv{}{t} \int_0^\infty
\epsilon f(\epsilon,\tau) D(\epsilon) d\epsilon$. The other thing that
depends on the temperature is f.

$\deriv{f}{\tau} = -\frac{(\epsilon - \mu)}{\tau^2}
\frac{1}{\parens{\exp(\frac{\epsilon - \mu}{\tau}) + 1}^2}$

Midterm material will stop here.

<a name='29'></a>

Physics 112: Statistical Mechanics
==================================
Fermi-Dirac/Bose-Einstein: April 9, 2012
========================================
Several things to discuss: midterm on Friday. Basically, the first seven
chapters of the notes, stopping at slide 10 of the notes without
questions. Try to have something less long, less difficult than midterm
#2. Mostly interested in concepts. Difficulties many of you have is that
you get confused between the various concepts. You really should be asking
yourself what method to apply. Understand how all the concepts are related
to each other. Clear emphasis on black body & Fermi-Dirac, but I will try
to judge how you put that in context with the rest. So one question that
comes from before. Things like definition of entropy that you need to know.

The two things I wanted to do today: metals -- $C \propto T$;
semiconductors. On Wednesday, we will finish the Fermi-Dirac and get into
Bose-Einstein.

Reminder: in crystals, the relationship between energy and momentum (what
we call in Physics the dispersion relations): gap between conduction and
valence bands -- energies are not allowed. Sometimes, the conduction band
is naturally filled. There are enough electrons in the crystal such that
you have a Fermi level above the energy of the conduction band.

In that case, we have basically the same formalism as we have had so far,
except that the energy is something like $\epsilon = \epsilon_c
\frac{\parens{p - p_0}^2}{2m_e^*}$. This mass is not the mass of the
electron; it is the mass of the electron inside the crystal (which is
usually smaller). All we have done can be generalized to that case. The
only thing which really changes is the mass of the electron. (also, usually
$p_0$ goes away)

Now, let's look at the heat capacity of the electrons in the crystal. In
order to have the heat capacity, I must compute the energy of the
eleectrons. That is very straightforward: $V\int_0^\infty \epsilon
\frac{1}{e^{\frac{\epsilon-\mu}{\tau}} + 1}D(\epsilon) d\epsilon$. Since $C
= \pderiv{U}{T}\Big|_V = h\deriv{U}{\tau} = k_BV\int_0^\infty \epsilon
\deriv{}{\tau}\parens{\frac{1}{e^{()} + 1}}D(\epsilon)
d\epsilon$. Derivative of $s(\epsilon)$ w.r.t $\tau$, not $\epsilon$. So
the action is occurring only around the chemical potential. So that is what
we will use. It's the narrow region around $\mu$. We have seen $\mu$ does
not vary rapidly with temperature, so let's take $\mu \approx
\epsilon_F$. (we have already used this, since we did not use chain rule
for $\deriv{\mu}{\tau}$. Number of particles is $\int s(\epsilon)
D(\epsilon) d\epsilon$. But number of particles is not changing, so
$\pderiv{N}{\tau} = 0$. 

Thus $C = k_B V\int_0^\infty \frac{\parens{\epsilon - \epsilon_F}^2}{\tau^2}
\frac{e^{\parens{\frac{\epsilon - \epsilon_f}{\tau}}} D(\epsilon)
d(\epsilon - \epsilon_F)}{\parens{e^{\frac{\epsilon - \epsilon_f}{\tau}} +
1}^2}$. Also, using the limits from $-\infty$ to $\infty$ is making the
approximation that $\epsilon \gg \tau$. This is a quantity that you
compute. $C \sim k_B D(\epsilon_F) A V \tau$.

This linear dependence on temperature is because the number of electrons
involved is proportional to temperature.

Taking into account phonons, $C_{tot} = C_e + C_\phi = \gamma T + AT^3$;
$C_e \ll \frac{3}{2}N k_B$. This by the way solved a great quandary that
people had at the beginning of the 19th century. There were electrons in
metals at the time, and we could actually compute their density. Heat
capacity estimate using ideal gas law was way off: only electrons that
affected anything were those close to the Fermi energy.

Semiconductors
==============

Semiconductors are substances where the Fermi level is somewhere in the
gap. At zero temperature, they will be totally insulators. The difference
between insulators and semiconductors is the magnitude of the gap. If the
gap is very big, you can only excite electrons from the valence band to the
conduction band at very high temperatures. For semiconductors, the gap is
somewhat smaller, and you can excite them at lower temperatures. We still
have our usual Fermi-Dirac distribution, but now the density of states is
somewhat different: you make parabolic approximations, and the density of
states of electrons is $D_e(\epsilon) d\epsilon \frac{2}{4\pi^2}
\parens{\frac{2m^*_e}{\hbar^2}}^{3/2} \sqrt{\epsilon - \epsilon_c}
d\epsilon$. (2 is from the spin)

The density of states for holes is inverted, since it is in the opposite
direction, and the masses are fairly different.

Basically, we can compute the total number of electrons: $n_{Te} = \int
f(\epsilon) D(\epsilon) d\epsilon = \int_0^{\epsilon_v} f(\epsilon)
D_h(\epsilon) d\epsilon + \int_{\epsilon_c}^\infty f(\epsilon)
D_e(\epsilon) d\epsilon$. Let us use the fact that $1 - \frac{1}{e^{\frac
{\epsilon - \mu}{\tau}} + 1} = \frac{1}{e^{\frac{\mu-\epsilon}{\tau}}+1}$
and rewrite this. What we get is that $\int_0^{\epsilon_v} \frac{1}{e^{
\frac{\mu - \epsilon}{\tau}} + 1}D_h(\epsilon) d\epsilon = \int_0
^{\epsilon_v} \frac{1} {e^{\frac{\epsilon - \mu}{\tau}} + 1}D_e(\epsilon)
d\epsilon$. Namely, number of holes is the same as the number of (free)
electrons.

Note that from this, ,we can see that the number of holes in the valence
band decreases with increasing $\mu$. Furthermore, we can determine $\mu$
by imposing charge neutrality.

The interest of semiconductors is that impurities are localized states in
the gap (not the band!). We still need to enforce charge
neutrality. Acceptors shift fermi level down to valence band, and I will
have holes in the valence band, and mostly positive carriers: p-type
material.

<a name='30'></a>

Physics 112: Statistical Mechanics
==================================
Fermi-Dirac/Bose-Einstein: April 11, 2012
=========================================
Several housekeeping items, and midterm on Friday. What I would like to do
today is finish Fermi-Dirac and speak in particular about the Chandrasekhar
limit and Bose-Einstein condensation.

So: after Monday, we will have only two weeks of class remaining. The
question is what do we want to speak about after Fermi-Dirac and
Bose-Einstein. Would like to speak about phase transitions and nonideal
gas, but this will take one or two lectures. So we have one week of free
subject we can choose. Propositions: transport phenomenon (diffusion,
drift), semiconductors, or cosmology.

Correction: heat capacity in metals. When thinking of heat capacity, we had
to take the derivative with respect to temperature of $\int_0^\infty
\epsilon \mathcal{f}(s,\tau)\mathcal{D}(\epsilon)d\epsilon$. This is just
the energy of a Fermi-Dirac gas, and, taking the derivative with respect to
temperature, we can do a change of variables to $\epsilon^\prime \equiv
\epsilon - \epsilon_F$ without changing our result (the jacobian is 1).

So let me provide other examples of degenerate Fermi gas. $^3$He has spin
$\frac{1}{2}$. cf problem set. very different behavior from $^4$He: phase
separation. Behaves as a magnetic fluid. Nobel prize of Richardson and
Oscheroff (?). At low temperature, these two fluids will not mix, and that
is what we actually use for supercooling.

Nuclear matter: protons and neutrons in the nucleus are also fermions, and
a fairly good model (bag model) is that these have relatively small
interactions with respect to each other. Have surface tension; tend to
stick together because of the bag. Not very modern way of thinking: muons
and whatnot. But to a first order, a fairly good approximation.

Typical radius of nucleus: $R \approx 1.3 \cdot 10^{-13} A^{\frac{1}{3}}$
cm. Velocity very high: $T_F \approx 3 \cdot 10^{11}$ K. Fermi
momentum. Used here at LBL to produce first pions. Machines were not very
powerful at that time: one of first cyclotrons (380 MeV), and they sent an
$\alpha$ onto a $^{12}C$, which produced this pion.

One of the most interesting applications of Fermi-Dirac statistics is in
white dwarves and neutron stars. What I told you so far is because we have
to stack the particles' energy (because I cannot put more than one particle
in each state), they are fairly large energies on the order of the Fermi
energy. This results in pressure. So the equilibrium of a star is the
equilibrium between (gravitational) potential energy and pressure from the
kinetic energy.

There is one class of stars (white dwarves), which is what our sun will
become. At some point in their lives, some stars will discard their
envelopes and contract into what is known as a white dwarf. High pressure;
very dense. What is providing the pressure is the degenerate gas of
electrons. There are of course protons and neutrons around, but they are
just not active in defining the pressure.

One way to express this equilibrium between gravitational pull (the star
tends to collapse, and the pressure which tends to keep it from collapsing)
is to look at the kinetic energy and the potential energy. Let's compare
the potential energy: let us assume our star is round. Take a constant
density $\rho$ (not true: physically, it goes as $\frac{M}{\frac{4}{3}\pi
R^3}$ -- this means that $n \propto \frac{M}{R^3}$).

This potential means we have to be related to the force and go as
$\frac{GM^2}{R}$. There will be some geometric factor in front, which you
will compute in your problem set. There is a negative sign, of course, and
let us call this $U_{\mathrm{pot}}-b\frac{M^2}{R}$. So what is the kinetic
energy? It goes as $\propto M\epsilon_F$. Let us distinguish between two
cases: first, if you are nonrelativistic, $\epsilon_F \propto n^{\frac{2}
{3}}$, so the kinetic energy goes as $\frac{M^{\frac{5}{3}}}{R^2}$. And if
I am ultrarelativistic (which can happen if mass of object is fairly
large), $\epsilon_F \propto n^{\frac{1}{3}}$, and so $U_k \propto \frac{
M^{\frac{4}{3}}}{R}$.

So in the nonrelativistic case, if I take the sum of the two energies, the
star has a minimum energy at a specific $R$. So the star is stable. This is
to be contrasted in the ultrarelativistic case: we then have still the
potential energy $U_p = -b\frac{M^2}{R}$, and kinetic energy which goes as
$U_k = c\frac{M^{\frac{4}{3}}}{R}$. For small M, the star expands; goes to
nonrelativistic cases and beocmes stable; at some sufficiently large M, the
sum is negative, and the star collapses. First described by Chandrasekhar
during his PhD. Degeneracy pressure cannot balance gravity if M too big:
roughly $1.4 M_\odot$: stars beyond this limit will go supernova.

Same story with neutrons, except now $\epsilon_F \approx 300 MeV$. Also has
a Chandrasekhar limit $3 M_\odot$, beyond which the star collapses on
itself and also gives rise to a supernova. Accretion from neighboring
stars.

Large stars collapse into neutron stars, and if the neutron star is too
large, it will further become a black hole.

Type Ia supernovae can be normalized: the story going to smoke is a little
more complex. Standard amount of material that just goes. What you see is
that universe expansion is accelerating instead of decelerating. Gravity
becomes repulsive (result of dark energy). Recent Nobel Prize (Saul
Perlmutter).

Bose-Einstein Condensation
==========================
The plus one is what gives you the square distribution in the Fermi-Dirac.

Note that the Pauli-exclusion principle only applies to Fermi-Dirac
particles. I can put as many particles in the ground state as I want. Talk
about choosing $\mu$ (since it is, after all, one of our random variables)
such that $\mu \approx \epsilon_0 - \frac{\tau}{N}$: set $\frac{N(\epsilon_0
- \mu)}{\tau} = 1$. Issue with using the method we've been using up to this
point (i.e. for Fermi-Dirac gas), the continuous approximation is not
accurate enough, since the gaps are actually important. You must rely on
the discrete sum. You do indeed solve this equation. What you get is that
indeed $f = \avg{s(0)} = \frac{1}{\exp(-\frac{\mu}{\tau})} = -\frac{\mu}
{\tau}$, so we get an incredibly small $\mu$: $10^{-26}$ eV. And if you
look at the second state, there are very few particles in the second state.

Temperature dependence: calculate separately condensed phase and normal
phase. Can use continuous approximation for excited state, but must isolate
ground state. We show that we have a certain Einstein condensation
temperature; $\tau_E = \frac{2\pi\hbar^2}{m}\expfrac{N}{2.612 V}{2/3}
\implies N_{exc} = N\expfrac{\tau}{\tau_E}{3/2}$. For large densities,
$\tau_E$ is not very small. 

<a name='31'></a>

Physics 112: Statistical Mechanics
==================================
Bose-Einstein Condensation: April 16, 2012
==========================================
Today: In particular, speak about number of states, superfluidity in, for
instance, liquid helium, and discoveries of Bose-Einstein condensates.

Midterms will be graded by tomorrow, presumably. You will have them on
Wednesday. So the final is on May 7, so three weeks from today, early in
the morning (sorry about that, but you are accustomed now). Of course, it
will cover everything that you have covered. After Bose-Einstein
condensates, I will have a short chapter on phase partitions (that is an
important subject in statistical mechanics), and then we will spend some
time on cosmology next week to show you how you can apply this to a
practical problem (it is not that practical).

Office hours Wednesday from 3-4; today is as usual (11-12).

Bose-Einstein Condensates
=========================

Bose-Einstein had an occupation number of $\frac{1}{\exp\parens{
\frac{\epsilon - \mu}{\tau}} - 1}$. This negative one is critical and will
determine the behavior of the condensation. What we saw was that when
$\frac{\mu - \epsilon_0}{\tau} \sim -\frac{1}{N}$ (for some $\epsilon_0$
being our ground state), roughly all of the particles are in the ground
state.

In principle we should make the calculation of $\mu$ by just looking at the
total number of particles: by the usual sum. Recall that when measuring
$\mu$, we cannot use the integral approximation that we used in the
Fermi-Dirac case, since our states of low energy are not very close
together. The integral approximation does not take into account the spacing
between the states. When $\mu$ is very small, this is not a very good
approximation. One way of thinking about it: states get denser at higher
$\epsilon$, but what happens with the Bose-Einstein condensation? When
$\frac{\mu - \epsilon_0}{\tau} \sim \frac{1}{N} \ll \epsilon - \epsilon_0$,
this spacing is critical: it will enforce that most of the particles are in
the ground state, and very few are in excited states.

So can we make calculations of this $\mU$ analytically? No; this is a
numeric problem.

We can talk, however, of isolating the first term and then using the
integral approximation on all excited states. That is an approximation, and
we would like this to be equal to N. We are interested in the second term,
the number of excited states. We would like $\frac{\epsilon_0 - \mu}{\tau}
\sim \frac{1}{N}$, so we can replace the excited states with $N_{exc}
\equiv V \int_{ \epsilon_1}^\infty \frac{1}{\exp \parens{\frac{\epsilon_0 -
\mu}{\tau}} \exp \parens{\frac{\epsilon - \epsilon_0}{\tau}} - 1}
D(\epsilon) d\epsilon$.

Working through the math, and setting $\epsilon_0$ to 0, we get $N_{exc} =
2.612 n_Q V$. It does not depend on N if $\frac{\mu}{\tau} = 0$. We thus
define the Einstein condensation temperature as $\tau_E \equiv \frac{2\pi
\hbar^2}{m} \expfrac{N}{2.612 V}{2/3}$, so $N_{exc} = N\expfrac{\tau}
{\tau_E} {3/2}$.

Liquid $^4$He
-------------
If you look in the slides, I have actually computed (also probably in
Kittel) the numerical values for $^4$He. If you apply this naively, you
will get 3.1K. So $^4$He is expected (if there were no interactions between
the atoms) to behave like a Bose-Einstein condensate. Not exactly true:
behaves as a Bose-Einstein condensate about 2.17K. This is important:
called the Landau point (also called lambda point because this looks like a
lambda). Helium is liquid about 4K. Literally changes sign at 2.17K.

All of your particles are in the same state and becomes a macroscopic
quantum state. Very fun to see (oh god!). Basically in the same way as in
electromagnetism, which is doing a square root of number of photons and
plane waves: we have a wave function which is the square root of energies.

With this quantum effect: you can use vortices which are quantized: have a
certain amount of angular momentum. You have the equivalent of the two-slit
experiment, where basically you have liquid helium go through two slots,
and they diffract exactly like Young's double-slit experiment. You have
basically all the interference phenomena.

The most dramatic macroscopic property is superfluidity. Not only dramatic,
it is a pain for experimentalists working at low temperature. Basically
what is happening is that the atoms are not subject to any kinds of forces
from the wall. They begin to flow on the wall as if it had no roughness
(explanation forthcoming!). It makes the helium have no surface tension on
the surface and go through cracks. One of the problems of experimentalists
working at low temperature is something that is essentially leak-proof
above the Landau point (2.17K), but once you cross that threshold, bang!
the thing begins to leak like a sieve.

And of course 2.17K is something that you go and look; you'd have to warm
up and try to understand where the leak could have come from, redo the
solder, get back down, and maybe nine times out of ten, this thing is
leaking again. That's why low-temperature is sometimes called
slow-temperature physics. It takes a lot of tries to fix a system which is
leaking.

To give you an idea of what is going on, I would like you the following
question: when is energy transfer maximized? When the two masses are equal;
easy to show via conservation of energy and conservation of
momentum. Important consequence: if $M \ll m$, then $\frac{1}{2}mv^2 \to
0$. In one dimension (you can of course generalize to several dimensions),
with a particle of mass M, $E = \frac{p^2}{2M}$. I have to conserve energy
and momentum, so the dispersion relationship of my particle of mass $m$ can
be expressed graphically by the intersection of two parabolas. If $m = M$,
the curves have the same width, so energy transfer is maximized. If m is
infinite, this is flat: I am not losing any energy.

We have a large effective $m$, but the analogy breaks down: system that is
very soft: no way to transfer a lot of momentum. When we send a little ball
into a superfluid liquid helium, it does not lose energy: keeps going as if
it were in a vacuum.

If your velocity is large enough, you can lose energy to phonons. In liquid
helium, there are also quantized oscillations. You have a system with
excitations, and there are phonons. If I am below the tangent, there is no
way I can have phonons (i.e. if travelling below velocity of sound). Only
if I am above the speed of sound can I lose energy. It will only lose
energy to phonons, and not to kicking of the system. Can emit excitations
(phonons) if velocity large enough. This may remind you of Cherenkov
radiation. This ia a phenomenon remarkably similar to that. If a particle
goes through a medium faster to the local velocity of light (smaller than c
because of diffraction index), then you will emit light. Same thing: if you
go above the velocity of sound, you will emit phonons.

So a lot of interesting physics; you can do the calculations, but the graph
is good enough to show what is happening.

By the way, there is one small experiment, which is somewhat interesting:
if you put a little pipe going through the surface of liquid helium in a
container with glass walls, and you begin to pump at 4K, and the
temperature of the helium goes down. Suddenly at 2.17K, you have a fountain
of liquid helium coming out of your tube. Very cool. Another thing that
happens is that the helium rises up on the sides and heats up to 2.17K
where it evaporates. It goes through cracks.

In the late 90s, there were interesting successful attempts by two groups
to artificially create Bose-Einstein condensation: one at NIST/JILA in
Boulder, and one at MIT.

This is an example where they were trapping atoms in the form of a ring,
which you can observe rotating. This is just the spectacular demonstration
that the particles are totally coherent.

Any way: how do we do that? What you need to make a Bose-Einstein
condensate: low temperature (need to cool atoms) and high density (of the
order of the quantum density). So how do you cool atoms? Having them bounce
on the wall is not a very efficient way of cooling them.

The breakthrough came from what was called laser cooling: suppose I have an
atom that I want to cool. This atom is going in many directions. Let's
choose an absorption line of this atom which has some resonance and
frequency. Instead of sending a laser at the resonance frequency, let's
send a laser slightly below this frequency. What is happening? This is if I
were in the rest frame of the atom. If the atom is moving towards the
laser, in this rest frame, it sees the frequency of the laser slightly
blue-shifted, so it absorbs the laser more, and it will emit the photons
over $4\pi$ after a while, and it has lost kinetic energy. If it goes away
from the laser, it will scatter less (it will see the frequency
red-shifted). The net result is if I am sending laser light from all
directions, I will tend to cool my atoms and decrease their energy.

We can use the same idea to trap the atoms: put magnetic field on the side:
frequency is changing; oblige particles to be in the area of zero magnetic
field.

In practice this is a little more complex than this: you cannot make a
magnetic field that looks like an infinite square well, but you can have a
rotating magnetic field, so every time the particles want to go out, they
will see the magnetic field (whose energy will be higher: particles are
slow since they have been cooled). Two groups in our department are doing
that as their main research.

<a name='32'></a>

Physics 112: Statistical Mechanics
==================================
Fermi-Dirac, Bose-Einstein, Phase transitions: April 18, 2012
=============================================================
Reasoning why chemical potential does not vary much at low temperatures: it
looks fairly rectangular under normal circumstances. When we have a finite
temperature, we have some rounding of the distribution.

The occupation number of holes: if I am a distance $\delta$ from $\mu$,
this is the occupation number $\lambda$ of electrons. The two are equal
because of this addition. On the other hand, that's not what we want to
have: we want to multiply by density of states. We have to plot
$f(\epsilon, \tau)$ and integrate over that. In two dimensions,
$D(\epsilon)$ is constant. So this is the same graph, except now we have
$D(\epsilon)$ on our axis. At a distance $\delta$ from the chemical
potential, now the _number_ of holes is equal to the _number_ of electrons
(as opposed to occupation number: we've taken into account density of
states, so this is for the entire system).

Because of this symmetry, the sum from 0 to infinity of $f(\epsilon, \tau)
D(\epsilon) d\epsilon$ is exactly equal to $\int_0^\mu D(\epsilon
d\epsilon$. This is known to be $\int_0^{\epsilon_F} D(\epsilon)
d\epsilon$. Slightly different from what happens in 3 dimensions:
$D(\epsilon) \propto \sqrt{\epsilon}$, so my function $fD$ looks different
because I am losing less on the hole-side than gaining on the electron, so
I have to reduce the chemical potential a little bit at $\tau$ at 0.

Don't confuse occupation number (which is symmetric) with the number (which
is not symmetric in general). Symmetric only in two-dimensional case
because $D(\epsilon)$ constant.

Let me, then, finish rapidly what I wanted to say on Fermi-Dirac and
Bose-Einstein. We were speaking about this very nice experiment: BEC atoms,
cooling in a trap. Now becoming routine, but before were very difficult to
do with atoms. And now people are doing that with molecules; they are
making artificial crystals; there is a whole industry. They take atoms and
arrange them in a particular fashion and potential. Now that the technology
of cooling the atoms and trapping them is well understood, there is a lot
of physics happening.

Graph corresponds to spatial density of atoms. Claim: not a great
discovery; just a technical feat. Superconductivity: in low-temperature
superconductors, you have electrons pairing in Cooper pairs for phonon
interactions.

Condensation theory is a bad approximation: interactions between Cooper
pairs are important. The temperature at which superconductivity appears is
much smaller than you would naively compute. Similar effects: zero
resistance (as in superfluidity), vortices: quantization of flux, phase
shift effects: all the $n^2$ behavior. Superconductor with two junctions is
equivalent to Young's double-slit experiment. Very similar properties; very
important devices.

$^3He$ is spin $\frac{1}{2}$, and you have pairing of the spin to create a
spin of 1 to create superconductivity. Then, because this is in vacuum, you
have very strange effects: magnetic properties.

This is a very important effect in condensed-matter physics. Emerging
phenomenon: completely different phenomenon at low temperature. Surprising:
not that low of temperature for sufficiently dense systems.

Energy density for both bosons and fermions goes as $T^4$. Useful when
considering early universe when considering expansion.

Pressure: we have never solved problem of scattering of particles (shown
force per unit area). Once again, define independent variables when taking
partial derivatives. What is constant is energy and number of particles (if
we want to use $p = \tau \pderiv{\sigma}{N}$.

The force per unit area on the wall can be readily computed in the
following way: I am considering a small area on the wall $dA$. Now, if I
have a particle coming in (I will assume, by the way, because of the
symmetry, the angle of reflection is the same as that of incidence), the
force is merely $\pderiv{p}{t}$, i.e. what is the change of momentum per
unit time? And the pressure will be the force divided by $dA$. I will have
to compute this: $\frac{1}{dA\Delta p}\int 2p\cos\theta v\Delta t dA
\cos\theta n(p) p^2 dp d\Omega = 2\pi \int cos^2\theta d\cos\theta \int 2pv
n(p)p^2dp$. The $\theta$ integral gives me $\frac{1}{3}$, and what we have
is that my pressure is $\frac{4\pi}{3} \int pv n(p) p^2 dp$. Depending on
whether you are nonrelativistic or (ultra)relativistic, pv is just $mv^2 =
2\epsilon$, so $P = \frac{2}{3}U$. If you are relativistic, $pv$ is just
$pc = \epsilon$, the pressure is therefore just $\frac{1}{3}U$. And check
with our various results: this is the same pressure as the thermodynamic
definition $\tau\pderiv{\sigma}{V}\Big|_{U,N}$

Explanation for why we have pressure for Fermi-Dirac even at zero
temperature: I have to stack up my states in energy space, and I have to
have states that are high velocity even at zero temperature. That's one of
the interpretations of the pressure of a Fermi-Dirac gas.

phase transitions: system in contact with reservoir, but not necessarily in
equilibrium. What is minimized? Landau free energy. We have seen this: free
energy is not defined because $\tau$ is not defined. Energy is not minimzed
because system is constantly kicked by thermal fluctuations.

<a name='33'></a>

Physics 112: Statistical Mechanics
==================================
Phase transitions: April 23, 2012
=================================

Would like to finish phase transitions if possible. The modern way of
looking at phase distributions involves looking at the Landau
distributions: consider the Landau free energy $F_L = U_s - \tau_R
\sigma_s$ and Landau free enthalpy $G_L = U_s - \tau_R\sigma_s + p_R
V_s$. The first one is used when considering constant volume, and the
second one is used at constant pressure.

Generally speaking, you will look at the dependence of $U_s, \sigma_s, V_s$
on an order parameter $\xi$, and we are looking at equilibrium, which is
obtained at the minimum.

You may be somewhat confused by the fact that you cannot define the state
of a system by just one parameter. We must almost actually minimize with
respect to all other variables.

This minimization comes in usually by the expression of $\sigma_s
(\xi)$. When you speak of $\sigma_s(\xi)$, usually energy depends directly
on $xi$, whereas $\sigma$ depends on probabilities. You will maximize
$\sigma_s$ at some given $\xi$.

When I was speaking of ferromagnetism, at one point I was changing in the
expression of the entropy $\frac{mB}{\tau} \to \tanh^{-1}\parens{\frac{M}
{nm}}$, I was already doing this minimization.

The net result is that if I plot F as a function of the magnetization, at
high temperature, the magnetization wants to be zero (since that is the
minimum of the Landau free energy), and this curve will move upwards until
suddenly, at a critical temperature (the Curie temperature), it develops a
minimum, and the equilibrium magnetization becomes nonzero.

If I plot the magnetization as a function of teh temperature, it is zero
above this temperature. This is a second-order phase transition, and you
move smoothly from $m=0$ to $m \neq 0$. There is no discontinuity in
$m$. This is very different from the case in which we go from gas to
liquid. Continuous evolution: the thing that is discontinuous is the first
derivative.

Classical gases: what are we missing in our description (point-like
particles which just scatter when they make contact with each other).

Issues: limit to compressibility (not taking into account volume of
particles). Interaction forces (long-distance): attractive Van der Waals
forces (polarization due to fluctuations induces polarizations in other
local particles). So how do these forces look? I have a very strong
repulsive force when they are in contact and a weaker $\frac{1}{r}$ force
when they are sufficiently far apart.

$V \to V - Nb$ (where $b$ is the volume of the atom). So this is the
approximation. Instead of a very fast approaching force, we linearize about
this point. For the attractive force, I will treat in a similar manner to
what we did for magnetism: mean field approximation. $\avg{U} \to \avg{U} -
\avg{\phi}\frac{N(N-1)}{2}$. I will say that $U = T - \frac{N^2 a}{V}$
because the average of $\phi$ is $\frac{\int \phi d^3 r}{V} \equiv
\frac{2a}{V}$. I will make this approximation: there is an attractive force
that goes as $N^2$.

We want to compute $G_L$. I have $U_s = T - \frac{N^2 a}{V}$, and, back to
counting of states, $\sigma_s = N \bracks{\log \bracks{}\frac{\expfrac{M
U_K}{3\pi\hbar^2 N}}{\frac{N}{V - Nb}} \equiv N \log \frac{n_Q}{n} +
\frac{5}{2}N$ (the Sackur-Tetrode formula).

At $U_k = \frac{3}{2} N\tau$, I am not yet in equilibrium with the
reservoir, so there is no real way to define temperature.

What is the pressure? There is a critical pressure $\frac{a}{27b^2}$ (don't
ask me; just result of calculation) above which things behave normally:
$G_L$ normally, and as temperature goes down, $G_L$ as a function of $V_s$
moves downward. But below this limit, I start to develop two minima: moves
up and to the left as temperature goes down.

$\pderiv{G_L}{V_s$ gives us the Van der Waals equation of state,
$\parens{p_R + \frac{N^2a}{V_s^2}}\parens{V_s - Nb} = N\tau_R$. I have
already defined $p_c = \frac{a}{27b^2}$, and $\tau_c = \frac{8a}{27b}$.

At this critical temperature, it begins to develop a certain inflection
point, and the liquid/gas relationship emerges.

If you do this calculation numerically, it is not easy to plot: there is a
big difference between the volume of the gas and the volume of the gas for
different values of the pressure compared to the critical pressure.

At high pressure compared to teh critical pressure, you stay always in the
gas phase. As you increase the temperature, it will decrease, and the
minimum goes down: the volume just changes. Nothing special happens. If you
are below the critical temperature, at high temperature, volume is large,
and you see a minimum at high temperature, and there is a second minimum
which develops: the liquid. That is what is happening.

Transition from liquid to gas as we increase the temperature: it does not
go by itself: there is a potential barrier between the two phases: liquid
$\to$ gas needs a wall or a dust particle (creating a bubble takes work.

Even if the gas has a smaller free enthalpy, I still have to overcome this
potential barrier (we are stuck in the liquid if nothing else
happens). Takes work to create a bubble.

Meta-stable states: superheated liquid or supercooled vapor: need surfaces
for transition to occur.

Unless you increase the temperature high enough such that there are no more
local minima, you will go extremely brutally.

<a name='34'></a>

Physics 112: Statistical Mechanics
==================================
Phase transitions, Cosmology: April 25, 2012
============================================

What I wanted to do was speak about the final. You have the right to have
four pages now (single-sided) of notes. As usual, my advice is to rewrite
your notes because this class is more about concepts and how they relate to
each other than formulae. As should be quite obvious from the midterms, if
you take the wrong formula and apply to a situation, the result is
unpredictable.

I think we all agree that 8am is not advisable. So what I can propose is a
review session either on Wednesday 4-6, Friday 10-12, or Friday 2-4 (Alex's
is on Thursday 1-3pm in 9 Lewis). I will focus the review on chemical
potential, since we have not really seen this before.

Strong preference for Wednesday.

So let's look at phase transitions. We were looking at this question of how
the system goes from liquid to gas as we increase the temperature. The
thing I wanted to attract your attention that for this kind of first-order
phase transition, the behavior is not continuous: there is a discontinuity
because there are to minima in $G_L$. Because there is a potential barrier
between the two minima, the system can be stuck in one of the states. It is
not true that if you heat (pure) water at about 100 degrees Celsius, it
will not boil. It will be stuck in a metastable state of superheated
liquid. Will only boil because of defects.

Import in stuff like bubble chambers and particle detectors (important for
detection of dark matter). Can stay metastable for minutes. This is fairly
characteristic of what we call first-order transitions.

Chemical potential as a function of $p, \tau, N$ has no dependence on
$N$. We showed that $G = N\mu(p,\tau)$.

Entropy of liquid is lower than that of gas with same parameters. Related
to the fact that there are fewer degrees of freedom, so smaller number of
states. Using that the Gibbs free energies are the same, $\Delta H = LN >
0$, where $L$ is the latent heat per particle.

Coexistence: you can follow the separation between the liquid and gas as a
function of pressure and temperature. When the Landau free enthalpy is
equal between the systems, you are on this locus where gas and liquid
coexist, and of course it stops when you reach critical pressure and
critical temperature, which we call the critical point. This is of course
of intense interest to us.

There is a very famous formula derived in the mid-nineteenth century by
Clausius and Clapeyron, which is very simple. Clearly we have
$G_L(p(\tau),\tau) = G_g(p(\tau),\tau)$ (equation at the coexistence
line). Now, taking the derivative with respect to $\tau$, we get
$\pderiv{G_L}{\tau}\deriv{p}{\tau} + \pderiv{G_L}{\tau} = \pderiv{G_g}
{\tau}\deriv{p}{\tau} + \pderiv{G_g}{\tau}$. So what are these terms?

$dG = -\sigma d\tau + Vdp + \mu dN$, so $\pderiv{G}{p} = V$,
$\pderiv{G}{\tau} = -\sigma$. Thus we can solve: $\deriv{p}{\tau} =
\frac{\sigma_l - \sigma_g}{V_g - V_l} = \frac{1}{\tau}\frac{L}{v_g - v_l}$,
where $v_g \equiv \frac{V_g}{N}$. If you use that $v_l \ll v_g \sim
\frac{\tau}{p}$, then this is roughly $-\frac{pL}{\tau^2}$, or $p \sim
\exp\parens{-\frac{L}{\tau}}$. If you express the partial pressure, you
have a straight line, which is actually the latent heat per particle. Very
good approximation for water (given the number of assumptions we have made)
and ice (since we can do the same thing between solid and liquid). Also an
excellent approximation for $^4\mathrm{He}$.

That's basically all regarding phase transitions. These arise from
correlations between particles: no phase transitions with ideal gases. The
method used here is the mean field approximation as a first-order. Two
types: first order (coexistence, latent heat, metastability) and second
order (continuous transformation -- discontinuity in derivative). In first
order, there is a critical point. Very important in modern statistical
mechanics.

Cosmology
=========
Let me dissipate ambiguities regarding presence on final. The details of
what I will tell you will not be on the final. But the kind of principles
that I am applying (the thermal physics and statistical mechanics) are
clearly on the final: these are the things we have spoken about in
considerable detail over the last 14 weeks.

What I would like to speak to you about is basically the thermal evolution
of the universe. We have something (we call this the Big Bang). Big
explosion: a lot of unknown particle physics at the beginning. At about a
tenth of a nanosecond in, what we see is fairly well defined. A few
thousand years gives us the microwave background.

How do we know that the universe is expanding? We can measure the Hubble
recession of distant galaxies. To a first approximation, their velocity is
proportional to their distance. There is essentially 80 years of research
where we have learned to measure distances, account for local velocities,
and more.

THe second thing (which we have spoken about) is that we have observed this
background radiation (about 3K). The final thing (which I will speak about
in more detail on Friday) is that if we, in the early universe, not only
observe protons and electrons, but that pi-modal -- helium and deuterium
have been formed -- in order to understand how these things happened, we
need a very hot phase.

Best way to think about this expanding universe (which is mind-boggling
because everything is changing) is to divide out the expansion. We have
something called the scale parameter a(t) and go from the physical
coordinate to the comoving coordinate, where we take this expansion away.

Now, there is something that we call the Friedman equation: the sum of
kinetic energy and potential energy is constant. We can compute constants
in general relativity. If the curvature of the universe is infinite, this
is constant.

For all practical purposes, we believe this all started from a phase
transition: inflation. This second-order phase transition led to
exponential expansion. What is going on? We assume that we have a field
which we have never seen (order parameter -- inflaton). Same that we've
used, except now in quantum mechanics: instead of classic variables, we now
have quantum fields. As temperature decreases, this begins to develop a
second minimum. This will induce a phase transition. System feels that its
energy is not equal to zero, which leads to an exponential increase of the
scale parameter. We call that inflation. We believe that in the space of
less than a tenth of a nanosecond, the universe has expanded by a factor of
60E40. For all practical purposes, this is what we call the big bang.

<a name='35'></a>

Physics 112: Statistical Mechanics
==================================
Cosmology: April 25, 2012
=========================

Thermal history of the universe.  How thermodynamics / statistical physics
is applied to the field. Before I do that: let me remind you that next week
we will have review sessions Wed 4-6 in 325 Leconte and Th 1-3 9 Lewis.

What I am going to do is finish talking about inflation, then speak of the
evolution of temperature as a function of time, and finally give you an
idea about nucleosynthesis: how the elements (which have nuclei) were
formed. This will give us the opportunity to speak about three important
aspects of the course: phase transitions, more general arguments about
evolution of entropy, and the mass-action law.

For instance: looking at a proton and an electron, we get hydrogen. Or a
neutron and a proton: deuterium. Or deuterium and a proton: Helium-3.

The universe is expanding in a homogenous and isotropic manner. The
physical coordinates are related to comoving coordinates by a certain
expansion factor. This is interesting: relates speed of expansion to energy
density.

Did speak on Wednesday regarding what happens in the early universe: phase
transition (postulate). We believe that we had a phase transition, where
what was happening as a function of order parameter, the Landau free energy
developed a minimum, and suddenly the universe wants to go to this
point. When it does that, it discovers that is has a nonzero energy
density, and it begins to expand.

On the order of 60E40.

So: why do we need something like that? Need to justify cosmic microwave
background. Remember this is the radiation from the plasma in the early
universe at a given temperature. Recombined into hydrogen, so universe
became transparent.

Things were close (in causal contact). Then things were put very far
apart. In GR, there is no problem with having the space expand faster than
the speed of light.

That was the main reason for inflation: some reason for extremely fast
expansion of universe, which then settles down.

Space flat, so no worry regarding initial conditions. Quantum fluctuations
are frozen in and expand with space. Will provide seed for large scale
structure.

If you plot the power spectrum of density fluctuations as a function of
spatial frequency $k$ (just a Fourier transform). We have a power spectrum
that looks roughly parabolic (with a maximum), and we understand the
shape. If we measure the microwave background on this plot and extrapolate
from the expansion factor, it links perfectly with what we measure in the
galaxies in terms of structure. That was the great excitement about the
cosmic microwave background when we first measured these fluctuations: they
were right were we needed them to be.

We have no real mechanism for this field. Cosmology points to physics at
much higher energy: $10^{16}$ GeV. Best accelerators are $10^4$ GeV. One of
reasons for switching to cosmology.

What can we test? Measure polarization of microwave background: see
gravitational field. This is very much related to discussions in media on
multiverses.

What is constant in this comoving sphere during the expansion? The entropy
-- no heat transfer. The energy cannot be constant: the sphere is working
against the rest of the universe. There is this pressure. The volume
increases, $-pdV$ acts, and so the energy inside decreases by $pdV$. The
entropy on the other hand should not decrease: universe is isotropic and
homogeneous.

No generation of entropy if there are no first order phase transitions
(which would mean irreversibility).

This tells us that entropy per unit comoving volume has to be constant. $T
\propto \frac{1}{a(t)}$. Remember: we did show that the energy density for
relativistic particles (which dominated the entropy during the early
universe) goes as $T^4$. There is a factor corresponding to the degrees of
freedom, which is 1 per polarization for bosons and $\frac{7}{8}$ per
polarization for fermions So $\frac{\sigma}{\gamma} \propto g^* T^3$. That
is related to relativstic number of the number of particles.

So what is the $\frac{\sigma}{V_{\text{com}}} \propto g^*$. In that case,
we have $S_{com} \propto a^3 g^* T^3$, which gives us that $T \sim
\frac{1}{a(t)$. Same result as in GR.

Reason why temperature goes as $\frac{1}{a(t)}$ is related to the Doppler
shift. As the universe expands, the wavelength of the relativistic
particles is stretching out in GR, and the wavelength increase, frequency
decreases, therefore the temperature decreases.

If there is no change of degrees of freedom, $T \propto \frac{1}{a(t)}$. In
the parabolic graph, used that we can compute (from first principles)
temperature of fusion of hydrogen to be ~3000K. Universe was 1000x smaller
than it is now.

If the number of degrees of freedom is changing, you have a kink in the
temperature evolution.

With high enough temperature compared to binding energy, the product,
for all practical purposes, does not exist.

Indeed, in this case, the chemical potentials add.

Problem: running out of time. Try to tell a little bit about how we discuss
the formation of atoms in the early universe. Neutrons, protons,
electrons. At the early part (before about 3 minutes in the age of the
universe), we had too high of energy, and the neutrons plus protons could
not form deuterium. When the temperature dropped, deuterium was able to
form, and we had that. Then we could form Helium-3, Helium-4, etc. We have
to be a little careful when we have two charged particles, we have a
positive potential from the EM forces between the particles.

Let me show just one thing: we can use this kind of argument to follow the
expansion of the density of various components. In the space of a few
moments, you are forming all of the light nuclei in the universe. Can try
to measure amount of deuterium and whatnot. You arrive at the fact that
ordinary matter is only a tiny part of what we observe in the universe.

By the way: cosmic microwave background gives exactly the same results with
totally different physics.

Conclusion: what I wanted to conclude was the link between nuclear physics
at small scale and the universe at large scale. Now attempting to explore
links between particle physics / quantum gravity and the universe.

Inflation: origin of small scale quantum structure.
