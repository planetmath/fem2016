# fem2016
2016 Edition of the Free Encyclopedia of Mathematics (top-level repo)

# Overview

## The Plan

Use [git-repo](https://github.com/esrlabs/git-repo) to manage a
collection of repositories, one for each top-level MSC class, *viz.*

- 00\_General
- 01\_History\_and\_biography
- 03\_Mathematical\_logic\_and\_foundations
- 05\_Combinatorics
- 06\_Order\_lattices\_ordered\_algebraic\_structures
- 08\_General\_algebraic\_systems
- 11\_Number\_theory
- 12\_Field\_theory\_and\_polynomials
- 13\_Commutative\_rings\_and\_algebras
- 14\_Algebraic\_geometry
- 15\_Linear\_and\_multilinear\_algebra\_matrix\_theory
- 16\_Associative\_rings\_and\_algebras
- 17\_Nonassociative\_rings\_and\_algebras
- 18\_Category\_theory\_homological\_algebra
- 19\_K-theory
- 20\_Group\_theory\_and\_generalizations
- 22\_Topological\_groups\_Lie\_groups
- 26\_Real\_functions
- 28\_Measure\_and\_integration
- 30\_Functions\_of\_a\_complex\_variable
- 31\_Potential\_theory
- 32\_Several\_complex\_variables\_and\_analytic\_spaces
- 33\_Special\_functions
- 34\_Ordinary\_differential\_equations
- 35\_Partial\_differential\_equations
- 37\_Dynamical\_systems\_and\_ergodic\_theory
- 39\_Difference\_and\_functional\_equations
- 40\_Sequences\_series\_summability
- 41\_Approximations\_and\_expansions
- 42\_Fourier\_analysis
- 43\_Abstract\_harmonic\_analysis
- 44\_Integral\_transforms\_operational\_calculus
- 45\_Integral\_equations
- 46\_Functional\_analysis
- 47\_Operator\_theory
- 49\_Calculus\_of\_variations\_and\_optimal\_control\_optimization
- 51\_Geometry
- 52\_Convex\_and\_discrete\_geometry
- 53\_Differential\_geometry
- 54\_General\_topology
- 55\_Algebraic\_topology
- 57\_Manifolds\_and\_cell\_complexes
- 58\_Global\_analysis\_analysis\_on\_manifolds
- 60\_Probability\_theory\_and\_stochastic\_processes
- 62\_Statistics
- 65\_Numerical\_analysis
- 68\_Computer\_science
- 70\_Mechanics\_of\_particles\_and\_systems
- 74\_Mechanics\_of\_deformable\_solids
- 76\_Fluid\_mechanics
- 78\_Optics\_electromagnetic\_theory
- 80\_Classical\_thermodynamics\_heat\_transfer
- 81\_Quantum\_theory
- 82\_Statistical\_mechanics\_structure\_of\_matter
- 83\_Relativity\_and\_gravitational\_theory
- 85\_Astronomy\_and\_astrophysics
- 86\_Geophysics
- 90\_Operations\_research\_mathematical\_programming
- 91\_Game\_theory\_economics\_social\_and\_behavioral\_sciences
- 92\_Biology\_and\_other\_natural\_sciences
- 93\_Systems\_theory\_control
- 94\_Information\_and\_communication\_circuits
- 97\_Mathematics\_education

and in these repositories, store all of the LaTeX files from
PlanetMath.  The current directory will contain instructions for
building the entire encyclopedia as one (giant) PDF.  The
subdirectories will contain instructions for building that book as a
stand-alone PDF.

## Editorial policy

Ideally we'll find expert editors for each of the MSC classes.

# Details

## Quickly create the repositories from the command line

[//]: # Carried out March 7th and 8th, 2016 -jac

```
curl -u 'TOKEN' https://api.github.com/user/repos -d '{"name":"REPO"}'
```

And then, from within a repository with some boilerplate content, for each repo of interest, run a command like this:

```
git push --mirror https://github.com/holtzermann17/REPO.git
```

Then transfer (by hand :boom:) to the planetmath organization.

Now the repositories are available at places like https://github.com/planetmath/00_General and they can be cloned (and populated).
