**Optimal Market Making for**

**Cryptocurrency Options**

*The Guéant--Lehalle--Fernandez-Tapia Framework and its Extensions*

A 10-Week Summer Research Program

North Carolina State University

**Industry Mentor**

Dendi Suhubdy

*Bitwyre*

San Francisco

2026

1\. Course Overview

This ten-week summer research program prepares students in the North
Carolina State University Financial Mathematics graduate program to
design, implement, and evaluate optimal market making strategies for
cryptocurrency options. The program is organized around the
Guéant--Lehalle--Fernandez-Tapia (GLFT) framework, a modern
stochastic-control approach to liquidity provision that generalizes the
earlier work of Avellaneda and Stoikov. The central pedagogical question
is how to extend GLFT, which was originally formulated for linear
instruments, to non-linear derivatives whose inventory risk is
multi-dimensional in the Greeks.

The program is mentored by Dendi Suhubdy. Students will work with live
and historical Coincall data throughout the program and will produce a
research-grade final report and code repository suitable for further
academic or industry use.

1.1 Learning Objectives

Upon successful completion of this program, students will be able to:

1.  Formulate a market making problem as a continuous-time stochastic
    optimal control problem and derive the associated
    Hamilton--Jacobi--Bellman (HJB) equation.

2.  Solve the HJB system for the Avellaneda--Stoikov and
    Guéant--Lehalle--Fernandez-Tapia models, including the asymptotic
    regime in which closed-form quote expressions are available.

3.  Calibrate parametric volatility surfaces (SVI, SABR) to live
    cryptocurrency options data and assess their stability across time.

4.  Implement production-grade fast pricing routines using
    characteristic function methods (Carr--Madan FFT, Fang--Oosterlee
    COS) and compute the full Greek vector via adjoint algorithmic
    differentiation.

5.  Extend the GLFT framework to a multi-Greek inventory penalty
    following El Aoud and Abergel, and reduce the resulting HJB system
    to a numerically tractable form.

6.  Integrate a dynamic hedging policy with the quoting engine and
    analyze the resulting P&L attribution.

7.  Build and validate an event-driven backtest that consumes real
    Coincall order book data and produces interpretable P&L, risk, and
    Greek-exposure diagnostics.

8.  Communicate research results in writing and orally at a level
    suitable for industry quantitative research interviews.

1.2 Prerequisites

Students are expected to have completed or be concurrently enrolled in
graduate coursework covering: stochastic calculus (Itô integration,
Itô\'s lemma, Girsanov\'s theorem), continuous-time stochastic processes
(Brownian motion, Poisson processes, jump-diffusions),
Black--Scholes--Merton option pricing, partial differential equations at
the level of Evans, and probability theory at the level of Durrett.
Programming maturity in Python is required; familiarity with NumPy,
SciPy, and JAX is advantageous but not required.

1.3 Structure

Each week of the program comprises two ninety-minute lectures, one
ninety-minute recitation, and approximately fifteen hours of independent
reading, problem-solving, and programming. Weeks 5, 7, and 9 are
designated milestone weeks at which students deliver a working software
component built on top of the preceding weeks\' material. The final week
is devoted to a chosen extension topic and the preparation and
presentation of a research-grade final report.

The compression from a longer original schedule to ten weeks places
additional self-study expectations on students: in particular, the
survey of GLFT variants (multi-asset, adverse selection,
discrete-inventory) is moved from a dedicated lecture week into required
independent reading during week 5, and the practitioner-oriented
treatment of dynamic hedging is integrated into the options market
making theory week rather than receiving a standalone week. Students are
expected to complete the corresponding readings on schedule.

1.4 Assessment

Final grades are determined as follows. Weekly problem sets account for
thirty percent of the grade. The three milestone deliverables in weeks
5, 7, and 9 jointly account for thirty percent. The final report and
presentation account for thirty percent. Active participation in
lecture, recitation, and code review accounts for the remaining ten
percent.

1.5 Mentorship Model

Students will have access to weekly thirty-minute one-on-one office
hours with the industry mentor, in addition to scheduled lectures and
recitations. Office hours are intended for clarification of difficult
material, code review of milestone deliverables, and discussion of
research directions for the final week. Students are expected to come to
office hours with specific questions and prepared work.

2\. Program Milestones at a Glance

The program is organized around three milestone deliverables. Each
milestone integrates the material from the preceding weeks and produces
a software artifact that is incorporated into the final research
repository.

  ---------- ------------------ -------------------------------------------
  **Week**   **Title**          **Deliverable**

  5          Linear-asset GLFT  Working Python implementation of the GLFT
             engine             model on a single linear asset, validated
                                against simulated dynamics and benchmarked
                                on one month of Coincall BTC-PERP order
                                book data.

  7          Fast pricing and   Benchmarked pricing and Greeks library for
             Greeks library     European options under Black--Scholes and
                                Heston dynamics, with characteristic
                                function pricing (FFT and COS) and full
                                Greek vector computation via algorithmic
                                differentiation. Latency target: full
                                Coincall BTC surface revaluation in under 5
                                milliseconds.

  9          Full options       Event-driven backtest of the multi-Greek
             market making      market making engine on three months of
             backtest           Coincall BTC and ETH options data, with
                                full P&L attribution, risk metrics, and
                                Greek-exposure time series.
  ---------- ------------------ -------------------------------------------

3\. Week-by-Week Schedule

Each of the following ten sections gives the learning objectives,
lecture outlines, recitation activity, required reading, problem set,
and (where applicable) milestone deliverable for one week of the
program. Sections are designed to be read end-to-end as a working
syllabus for instructors and as a study plan for students.

Week 1 --- Foundations of Market Microstructure

*Theme: from limit order books to the economic role of the market
maker.*

Learning Objectives

- Reconstruct a limit order book from raw exchange feeds and compute
  standard liquidity metrics.

- Articulate the three classical components of the bid-ask spread and
  identify them in real data.

- Explain the role of the market maker as a continuously quoting
  liquidity provider, and contrast with directional traders.

Lecture 1 --- Limit Order Book Mechanics

An introduction to the institutional setting in which the rest of the
program takes place. The lecture begins with the mechanics of central
limit order books on modern electronic exchanges, then introduces order
types, matching rules, and the basic vocabulary of microstructure. The
lecture closes with a tour of the Coincall exchange architecture as a
concrete example.

- Order types: market, limit, IOC, post-only, hidden.

- Price-time priority and the matching algorithm.

- Order book aggregation: L1, L2, L3 views and what each reveals.

- Tick size, lot size, and the discrete grid of available prices.

- Coincall-specific architecture: contract specifications, fee
  structure, market maker tiers.

Lecture 2 --- Spread Decomposition and the Role of the Market Maker

The bid-ask spread is the market maker\'s source of revenue, but it is
also the compensation demanded for three distinct costs. This lecture
decomposes the spread into adverse selection, inventory, and
order-processing components, drawing on the classical models of Roll,
Glosten--Milgrom, and Kyle.

- The Roll (1984) model: estimating effective spread from trade prices
  alone.

- Glosten--Milgrom (1985): asymmetric information and the rational
  quote-setter.

- Kyle (1985): the strategic informed trader and market depth.

- Empirical decomposition: realized spread, effective spread, price
  impact.

- Why crypto markets exhibit different microstructure characteristics
  than equities.

Recitation

Hands-on session reconstructing the order book from a Coincall
tick-level recording. Students will load one hour of BTC-PERP feed data,
replay the events in time order, and produce a time series of
mid-prices, spreads, and book depth. Output: a Python class that
maintains a live order book state from raw events.

Required Reading

- Cartea, Jaikumar, and Penalva (2015), Algorithmic and High-Frequency
  Trading, Chapters 1--3.

- Roll (1984), A Simple Implicit Measure of the Effective Bid-Ask
  Spread.

- Glosten and Milgrom (1985), Bid, Ask and Transaction Prices in a
  Specialist Market with Heterogeneously Informed Traders.

Problem Set 1

1.  Implement an order book reconstruction class in Python that consumes
    a stream of order events (new, cancel, modify, trade) and maintains
    the current state of the L2 book. Apply it to a one-hour sample of
    Coincall BTC-PERP data and produce a plot of the mid-price and
    quoted spread over time.

2.  Compute the Roll estimator of the effective spread on the same data
    sample, and compare it to the directly observable bid-ask spread.
    Comment on any discrepancy.

3.  Derive analytically the quote-setter\'s bid and ask in the
    Glosten--Milgrom model under the assumption of a single informed
    trader and a Bernoulli arrival of informed versus uninformed orders.

4.  Numerically simulate the Glosten--Milgrom model with parameters of
    your choice and verify your derivation in problem 3. Plot the
    convergence of the public belief about asset value as trades arrive.

5.  Compute the realized spread and price impact on one hour of Coincall
    data using a five-minute decomposition window. Comment on what these
    metrics imply about the toxicity of the order flow.

Week 2 --- The Avellaneda--Stoikov Model

*Theme: a fully worked example of optimal market making through
stochastic control.*

Learning Objectives

- Set up the Avellaneda--Stoikov market making problem as a
  continuous-time stochastic control problem with exponential utility.

- Derive the associated HJB equation and reduce it to a system of ODEs
  through the appropriate ansatz.

- Solve the system in closed form under the simplifying assumptions of
  the original paper and interpret the resulting quote formulas
  economically.

Lecture 1 --- Setup and Dynamics

The lecture introduces the Avellaneda--Stoikov framework: a market maker
quoting bid and ask prices on a single asset whose mid-price follows
arithmetic Brownian motion, with order arrivals modeled as Poisson
processes whose intensities depend exponentially on the quote distance
from the mid. The wealth and inventory processes are derived, and the
optimization problem is stated.

- Mid-price dynamics: arithmetic Brownian motion as a local
  approximation.

- Poisson order flow with intensity λ(δ) = A exp(-κδ).

- Wealth and inventory state dynamics under continuous quoting.

- Exponential utility: motivation, properties, and why it makes the
  problem tractable.

- The terminal liquidation penalty and finite-horizon formulation.

Lecture 2 --- HJB Derivation and Solution

Starting from the dynamic programming principle, the lecture derives the
HJB equation for the value function and applies the standard ansatz that
separates the value function into wealth, inventory, and time
components. The resulting reduced system of ODEs admits an asymptotic
closed-form solution that exposes the structure of the optimal quotes.

- The dynamic programming principle and the HJB equation.

- Separation ansatz: V(t, x, S, q) = -exp(-γ(x + qS)) θ(t, q).

- Reduction to a system of ODEs in θ(t, q).

- The reservation price r(s, q) = s − qγσ²(T − t).

- Optimal half-spread expression and its decomposition into a
  risk-aversion and an order-flow component.

Recitation

Workshop on the derivation. Students bring partial derivations to the
recitation and complete them in pairs. The mentor walks through the
verification theorem step by step. Output: a complete typed derivation
in LaTeX, to be referenced throughout the program.

Required Reading

- Avellaneda and Stoikov (2008), High-Frequency Trading in a Limit Order
  Book.

- Cartea, Jaikumar, and Penalva (2015), Chapter 10.

Problem Set 2

1.  Derive the HJB equation for the Avellaneda--Stoikov model from first
    principles, justifying each step. Show that the value function
    ansatz V(t, x, S, q) = -exp(-γ(x + qS)) θ(t, q) reduces the HJB to a
    system of ODEs in θ.

2.  Solve the reduced ODE system in the asymptotic regime T → ∞ and
    obtain the closed-form expressions for the reservation price and
    optimal half-spread.

3.  Implement the Avellaneda--Stoikov quote engine in Python. Simulate
    one trading day of mid-price dynamics with σ = 2 USD/√s, fill
    arrivals with κ = 1.5 and A = 140, and compare the P&L distribution
    of the optimal strategy against a symmetric quoting strategy that
    ignores inventory.

4.  Perform a sensitivity analysis on the risk-aversion parameter γ.
    Plot inventory variance and Sharpe ratio against γ over a range
    covering three orders of magnitude, and identify the regime where
    the model is most effective.

5.  Discuss the assumption that mid-price dynamics are independent of
    the market maker\'s quotes. Identify at least three empirical
    phenomena in real markets that violate this assumption and discuss
    how each would affect the optimal strategy.

Week 3 --- Stochastic Optimal Control in Continuous Time

*Theme: the general theory underlying the previous week\'s worked
example.*

Learning Objectives

- State and apply the dynamic programming principle in a general
  continuous-time setting.

- Derive the HJB equation for a generic stochastic control problem and
  articulate the conditions of the verification theorem.

- Recognize the role of CARA and CRRA utilities in producing tractable
  problems and identify the consequences for the inventory penalty.

Lecture 1 --- Dynamic Programming and the HJB Equation

The lecture develops the dynamic programming principle in continuous
time and derives the HJB equation as a consequence. The treatment is
rigorous but informal: viscosity solutions are mentioned as the natural
setting for non-smooth value functions, but the program will focus on
classical solutions throughout.

- Controlled diffusions and admissible controls.

- The dynamic programming principle: heuristic and formal statement.

- Infinitesimal generator of a controlled diffusion.

- Derivation of the HJB equation by passing to the limit.

- Boundary and terminal conditions; finite vs infinite horizon.

Lecture 2 --- Verification Theorems and Tractable Utility Functions

The HJB equation is a necessary condition; the verification theorem
provides the converse, stating that a sufficiently smooth solution of
HJB is the value function. The lecture then discusses why exponential
(CARA) utility produces tractable problems in market making, and why
power (CRRA) utility appears in consumption-investment problems instead.

- Statement and proof sketch of the verification theorem.

- Smooth-fit conditions at free boundaries.

- Viscosity solutions: when classical solutions fail.

- CARA, CRRA, and HARA utility families; properties and use cases.

- Why CARA decouples the value function from wealth in market making.

Recitation

Worked solutions to classical control problems: Merton\'s portfolio
problem under CARA and CRRA utility, an optimal liquidation problem with
linear price impact. Students will identify the pattern of HJB
derivation, ansatz selection, ODE reduction, and solution that will
recur throughout the program.

Required Reading

- Pham (2009), Continuous-time Stochastic Control and Optimization with
  Financial Applications, Chapters 3--4.

- Cartea, Jaikumar, and Penalva (2015), Chapter 6.

Problem Set 3

1.  Solve the Merton portfolio problem in continuous time under CRRA
    utility. Derive the HJB equation, propose an ansatz, reduce to an
    ODE, and solve for the optimal consumption and investment policy.

2.  Repeat the previous problem under CARA utility and contrast the
    structure of the solution. Explain economically why the optimal
    portfolio depends on wealth under CRRA but not under CARA.

3.  Solve the Almgren--Chriss optimal execution problem in its
    continuous-time formulation. Derive the optimal trading trajectory
    under quadratic transient impact and verify your solution against
    the original discrete-time result.

4.  State the verification theorem in your own words and identify the
    precise role of each assumption (smoothness, growth conditions,
    admissibility class). Construct a counterexample in which one
    assumption fails and the conclusion of the theorem fails as well.

5.  Read the introduction of Pham Chapter 4 on viscosity solutions and
    explain in two paragraphs why viscosity solutions are needed in
    problems with non-smooth value functions, using the obstacle problem
    as your example.

Week 4 --- The GLFT Model, Part I --- Setup and HJB Derivation

*Theme: generalizing Avellaneda--Stoikov to arbitrary intensity
functions.*

Learning Objectives

- State the GLFT problem setup and identify the assumptions that
  distinguish it from Avellaneda--Stoikov.

- Derive the HJB system for the GLFT problem and recognize the role of
  the intensity functions Λ⁺ and Λ⁻.

- Recover the Avellaneda--Stoikov solution as a special case of GLFT
  with exponential intensities and verify the limiting behavior.

Lecture 1 --- The GLFT Setup

The lecture introduces the Guéant--Lehalle--Fernandez-Tapia framework.
The setup is similar to Avellaneda--Stoikov but generalizes in two
important directions: arbitrary intensity functions (subject to
regularity conditions), and a clean treatment of an inventory constraint
that bounds the position from below and above.

- Generalized intensity functions Λ⁺(δ) and Λ⁻(δ): regularity
  assumptions.

- Inventory constraint and the truncation of admissible quotes at the
  boundary.

- Wealth and cash dynamics; the cash process as a state variable.

- Comparison to Avellaneda--Stoikov: what generalizes, what does not.

- Discussion of the asymptotic regime that will become central next
  week.

Lecture 2 --- HJB Derivation in the GLFT Framework

The lecture derives the HJB system carefully, paying attention to the
boundary behavior at the inventory limits. The same separation ansatz
used in Avellaneda--Stoikov is applied, but the resulting reduced system
is a coupled system of ODEs that does not admit a closed-form solution
for general intensities.

- HJB equation in the multi-jump setting.

- The separation ansatz V(t, x, S, q) = -exp(-γ(x + qS)) θ(t, q) and its
  validity.

- Reduced ODE system in θ(t, q): coupling structure across q.

- Boundary conditions at the inventory limits q_min and q_max.

- Verification of the Avellaneda--Stoikov limit when Λ(δ) = A exp(-κδ).

Recitation

Pair derivation session. Students re-derive the GLFT HJB step by step,
with the mentor checking work in real time. The recitation closes with a
discussion of how the choice of intensity function reflects assumptions
about the order flow that the market maker faces.

Required Reading

- Guéant, Lehalle, and Fernandez-Tapia (2013), Sections 1--3.

- Guéant (2016), The Financial Mathematics of Market Liquidity, Chapter
  9.

Problem Set 4

1.  Derive the HJB system for the GLFT problem from first principles,
    carefully justifying the treatment of the inventory boundary.
    Identify the precise step at which the regularity assumptions on Λ
    are needed.

2.  Show analytically that the GLFT HJB system reduces to the
    Avellaneda--Stoikov HJB when Λ(δ) = A exp(-κδ) and the inventory
    constraint is relaxed.

3.  Consider three families of intensity functions: exponential,
    power-law, and logistic. For each, plot the implied order arrival
    rate as a function of quote distance and discuss what assumption
    about trader behavior the family encodes.

4.  Derive the inventory dynamics under a generic intensity function Λ
    and compute the expected change in inventory over a short interval,
    conditional on the current inventory and the chosen quotes.

5.  Read Section 2 of Guéant, Lehalle, and Fernandez-Tapia (2013) and
    write a one-page summary of the modeling choices that differ from
    Avellaneda--Stoikov. Comment on which differences are mathematically
    substantive and which are notational.

Week 5 --- The GLFT Model, Part II --- Asymptotic Solution,
Implementation, and Variants

*Theme: the asymptotic regime in which GLFT admits closed-form quotes, a
working implementation, and a self-study survey of the GLFT variants
literature.*

Learning Objectives

- Derive the closed-form GLFT quote expressions in the asymptotic regime
  via the appropriate change of variable.

- Implement the GLFT engine in Python, validated against simulated
  dynamics.

- Backtest the engine against Coincall BTC-PERP order book data and
  produce P&L, inventory, and Sharpe diagnostics.

- Read and summarize the major extensions of GLFT (multi-asset,
  predictive signals, adverse selection, discrete inventory) for use in
  the final-week extension project.

Lecture 1 --- The Asymptotic Regime and Closed-Form Quotes

The technical centerpiece of the GLFT paper. Under the asymptotic regime
in which the trading horizon is far from the terminal date, the change
of variable u(q) = θ(t, q)/θ(t, q+1) linearizes the reduced ODE system
into an eigenvalue problem, whose dominant eigenvector encodes the
optimal quoting policy. The lecture works through this derivation
carefully. The lecture closes with a brief survey of variants
(multi-asset, predictive signals, adverse selection, discrete inventory)
that students will read about independently this week as preparation for
the final-week extension topic.

- The asymptotic regime: motivation and conditions.

- Change of variable u(q) and the resulting linear system.

- Eigenvalue problem and the role of the Perron--Frobenius theorem.

- Closed-form expressions for the optimal bid and ask quotes.

- Decomposition of the quote into a \'fair price adjustment\' and a
  \'spread\' component.

- Brief survey: pointers to multi-asset, signal, and adverse-selection
  extensions in Guéant (2016).

Lecture 2 --- Numerical Implementation and Validation

The lecture transitions from theory to code. The closed-form quotes are
computed via solution of a linear system; the simulation infrastructure
is built from the order book and trade-arrival models studied in week 1.
The bulk of the lecture is dedicated to validation: comparing simulated
P&L distributions against theoretical predictions, and identifying
common implementation pitfalls.

- Solving the linear system for u(q) numerically with sparse linear
  algebra.

- Mapping the model\'s continuous time to discrete event arrivals in
  simulation.

- Calibrating intensity functions Λ⁺, Λ⁻ from historical Coincall fill
  data.

- Backtest harness: replay engine, fill simulator, P&L attribution.

- Common bugs: off-by-one inventory indexing, sign errors in cash
  dynamics, miscalibrated intensities.

Recitation

Code review of student implementations. Each student presents their
implementation and walks through one complete simulated trading day. The
mentor identifies issues in real time and the group resolves them
collectively. Time permitting, the recitation closes with a brief
discussion of the variants reading.

Required Reading

- Guéant, Lehalle, and Fernandez-Tapia (2013), Sections 4--6.

- Guéant (2016), Chapters 9--11 (independent self-study; required as the
  survey of GLFT variants in lieu of a dedicated lecture week).

Problem Set 5

1.  Carry out the change of variable u(q) = θ(t, q)/θ(t, q+1) in the
    GLFT reduced ODE system and show that, in the asymptotic regime, the
    result is a linear system whose solution determines the optimal
    quotes.

2.  Solve the linear system numerically for a problem with inventory
    limits q ∈ {-10, \..., +10} and intensity functions Λ⁺(δ) = Λ⁻(δ) =
    1.0 exp(-1.5δ). Plot the optimal bid and ask half-spreads as
    functions of inventory.

3.  Reproduce Figure 2 of Guéant, Lehalle, and Fernandez-Tapia (2013) on
    simulated data with the parameters given in the paper. Comment on
    any discrepancies.

4.  Calibrate the intensity functions from one week of Coincall BTC-PERP
    fill data using maximum likelihood. Report the fitted parameters and
    goodness-of-fit diagnostics.

5.  Run a complete one-month backtest of your GLFT implementation
    against Coincall BTC-PERP data and report mean P&L, P&L volatility,
    Sharpe ratio, maximum drawdown, mean inventory, and inventory
    standard deviation. Compare against a baseline that quotes
    symmetrically without inventory adjustment.

6.  Submit a two-page summary of Guéant (2016) Chapters 10--11,
    identifying one extension you find most relevant to crypto options
    market making and articulating why. This summary will be returned in
    week 10 as a candidate extension topic.

Milestone Deliverable: Milestone 1 --- Linear-Asset GLFT Engine

Submit a Python package implementing the GLFT optimal market making
model on a single linear asset, together with calibration, simulation,
and backtesting infrastructure. The deliverable must include a
reproducible backtest on one month of Coincall BTC-PERP data, with
results documented in a short technical report following the structure
of the original GLFT paper.

**Datasets provided by Coincall:**

  -------------------------------------------- ---------------------------------------------------
  **Dataset**                                  **Contents and Coverage**

  coincall_btc_perp_l2_2025Q4.parquet          BTC-USDT perpetual futures L2 order book snapshots
                                               at 100ms resolution for October--December 2025. Ten
                                               levels each side. Columns: timestamp, bid_px_0..9,
                                               bid_sz_0..9, ask_px_0..9, ask_sz_0..9,
                                               sequence_number.

  coincall_btc_perp_trades_2025Q4.parquet      BTC-USDT perpetual futures trade tape for the same
                                               period. Columns: timestamp, price, size,
                                               aggressor_side, trade_id.

  coincall_intensity_calibration_set.parquet   Pre-aggregated fill events grouped by quote
                                               distance from mid, suitable for maximum likelihood
                                               calibration of intensity functions. Provided as a
                                               convenience; students are expected to also produce
                                               the same aggregation from the raw L2 and trade data
                                               above.
  -------------------------------------------- ---------------------------------------------------

**Acceptance criteria:**

- GLFT quote computation runs in under 100 microseconds per update on a
  single CPU core.

- Intensity calibration produces a non-trivial fit, with χ²
  goodness-of-fit reported.

- Backtest produces P&L within ±50% of a reference implementation
  provided by the mentor.

- Code passes linting and includes unit tests covering the core quote
  computation.

- Technical report is at most ten pages excluding appendices.

Week 6 --- Options Pricing, the Volatility Surface, and Calibration

*Theme: a single concentrated week on options theory and the practical
construction of a volatility surface.*

Learning Objectives

- Recall the Greeks of European options and their economic
  interpretation, including the second-order Greeks vanna and volga.

- State the no-static-arbitrage constraints on the volatility surface
  and verify them on parametric surfaces.

- Calibrate SVI and SABR parameterizations to live Coincall options data
  with attention to stability.

Lecture 1 --- Greeks and the Volatility Surface

The lecture begins with a brisk review of European option pricing under
Black--Scholes and the Greeks delta, gamma, vega, theta, vanna, and
volga. The empirical phenomenon of the volatility smile and the term
structure of implied volatility is then introduced, along with
Gatheral\'s formulation of the no-static-arbitrage conditions. The
lecture concludes with a discussion of the specific features of the
cryptocurrency options surface.

- Black--Scholes formula and the Greek vector: closed forms and
  identities.

- Vanna, volga, and their role in volatility risk.

- The implied volatility smile and term structure: empirical
  regularities.

- Calendar arbitrage, butterfly arbitrage, and the corresponding
  inequalities.

- Crypto options surfaces: sparse strikes, wide wings, and quote
  staleness.

Lecture 2 --- Parameterization and Calibration

The lecture covers the two dominant parametric families: SVI (stochastic
volatility inspired, Gatheral) and SABR (stochastic alpha-beta-rho,
Hagan et al.). Each is introduced, its no-arbitrage form discussed, and
its calibration procedure derived. The lecture spends substantial time
on the practical issues of calibration to noisy data.

- Raw SVI parameterization and the arbitrage-free \'eSSVI\' formulation.

- Calibration of SVI by nonlinear least squares; sensitivity to initial
  guess.

- SABR formula and the small-time expansion of Hagan et al.

- Time-stability of calibrated parameters: smoothing across days.

- Diagnostic plots: residuals, leave-one-out errors, parameter time
  series.

Recitation

Live calibration session. Students load a Coincall options chain
snapshot, fit SVI and SABR surfaces, and produce the standard diagnostic
plots. The session ends with each student comparing their calibration to
the others and discussing the sources of variation.

Required Reading

- Gatheral (2006), The Volatility Surface, Chapters 1--5.

- Gatheral and Jacquier (2014), Arbitrage-Free SVI Volatility Surfaces.

- Hagan, Kumar, Lesniewski, and Woodward (2002), Managing Smile Risk.

- Hull (2021), Chapters 15, 19--21 (review of Greeks and basic surface
  concepts).

Problem Set 6

1.  Derive the closed-form expressions for vanna and volga under
    Black--Scholes. Verify your derivation by finite-difference
    computation against the Black--Scholes price and report the maximum
    relative error across a range of moneyness and maturities.

2.  Implement the raw SVI parameterization and the arbitrage-free
    constraints from Gatheral and Jacquier. Apply the constraints to a
    deliberately misparameterized surface and observe which constraints
    are violated.

3.  Calibrate SVI to one Coincall BTC options chain snapshot using
    nonlinear least squares. Report the fitted parameters, residuals at
    each strike, and the resulting RMS error in implied volatility
    units.

4.  Calibrate the SABR model to the same snapshot. Compare its fit
    quality against SVI and discuss the strengths and weaknesses of each
    parameterization for crypto options.

5.  Run daily SVI calibration over one month of Coincall data and
    produce a time series of each SVI parameter. Comment on the
    stability of the calibration and suggest a smoothing scheme that
    would improve day-to-day consistency.

Week 7 --- Fast Computation of Prices, Greeks, and Surfaces

*Theme: the latency budget of an options market maker, and the numerical
methods that meet it.*

Learning Objectives

- Implement and benchmark characteristic function pricing methods
  (Carr--Madan FFT and Fang--Oosterlee COS).

- Compute the full Greek vector via adjoint algorithmic differentiation
  rather than finite differences.

- Vectorize pricing and Greek computation across an entire surface to
  meet a production latency budget.

Lecture 1 --- Characteristic Function Pricing

Closed-form Black--Scholes pricing covers only one model. As soon as
students consider Heston or any stochastic-volatility model for the
underlying, they need numerical pricing infrastructure. The lecture
covers the two dominant approaches in the practitioner literature: the
Carr--Madan FFT method, which exploits the structure of the call price
under exponential damping, and the Fang--Oosterlee COS method, which
uses Fourier-cosine series and converges geometrically for smooth
payoffs.

- The characteristic function of log-returns under Black--Scholes and
  Heston.

- The Carr--Madan FFT method: dampened payoff, FFT, recovery of prices.

- The Fang--Oosterlee COS method: truncation interval, cosine
  coefficients, convergence.

- Comparison: when each method dominates in accuracy or speed.

- Monte Carlo as the baseline; variance reduction by control variates.

Lecture 2 --- Algorithmic Differentiation and Vectorization

Finite-difference Greeks are correct but slow: each Greek requires
re-evaluating the price, and a market maker quoting on dozens of
contracts with several Greeks per contract quickly exhausts the latency
budget. Adjoint algorithmic differentiation (AAD) computes the entire
Greek vector in time comparable to a single price evaluation. The
lecture covers forward-mode AD, reverse-mode AD, and their use in
derivatives pricing, with concrete examples in JAX and a brief
discussion of C++ implementations via Adept and Enzyme.

- Forward-mode and reverse-mode automatic differentiation: theory and
  complexity.

- Smoking adjoints: Giles and Glasserman\'s foundational application to
  Monte Carlo Greeks.

- JAX in practice: grad, jacfwd, jacrev, vmap, jit.

- Pathwise versus likelihood-ratio Greeks: when each is applicable.

- Vectorization across a surface: SIMD, JAX vmap, and GPU offload.

- C++ AAD: Adept, Stan Math, and the emerging compiler-level option via
  Enzyme.

Recitation

Hands-on optimization session. Each student profiles a naive
implementation of surface revaluation, identifies the bottleneck,
applies vectorization and AAD, and re-measures. The goal is a measured
speedup of at least one order of magnitude over the naive baseline.

Required Reading

- Carr and Madan (1999), Option Valuation Using the Fast Fourier
  Transform.

- Fang and Oosterlee (2008), A Novel Pricing Method for European Options
  Based on Fourier-Cosine Series Expansions.

- Giles and Glasserman (2006), Smoking Adjoints: Fast Monte Carlo
  Greeks.

- Capriotti (2011), Fast Greeks by Algorithmic Differentiation.

- Glasserman (2003), Monte Carlo Methods in Financial Engineering,
  selected sections on variance reduction.

Problem Set 7

1.  Implement the Carr--Madan FFT pricer for European calls under the
    Heston model. Verify against a Monte Carlo benchmark and report the
    convergence rate as a function of the FFT grid size.

2.  Implement the Fang--Oosterlee COS pricer for the same problem.
    Compare its accuracy and runtime against your Carr--Madan
    implementation across a range of moneyness and maturities.

3.  By hand, derive the forward-mode AD for the Black--Scholes call
    price and verify that the resulting derivatives match the analytical
    Greeks. Document the dual-number arithmetic explicitly.

4.  Use JAX to compute the full Greek vector (delta, gamma, vega, theta,
    vanna, volga) for a portfolio of fifty Heston-priced options.
    Compare the runtime against finite-difference Greeks computed by
    re-evaluating the COS pricer with bumped inputs.

5.  Vectorize your surface revaluation using JAX vmap and measure the
    speedup against a naive Python loop. Report the result in
    nanoseconds per option-Greek-evaluation.

6.  Optional advanced exercise (for students with C++ experience):
    compile a small Black--Scholes pricer through Enzyme or Adept and
    benchmark its AAD performance against your JAX implementation.

Milestone Deliverable: Milestone 2 --- Fast Pricing and Greeks Library

Submit a Python (and optionally C++) library that prices European
options under Black--Scholes and Heston models via characteristic
function methods, computes the full Greek vector via algorithmic
differentiation, and revalues the entire calibrated Coincall surface
within a strict latency budget. The deliverable must include
benchmarking results, accuracy validation against an independent Monte
Carlo reference, and unit tests.

**Datasets provided by Coincall:**

  ----------------------------------------------------- ---------------------------------------------------
  **Dataset**                                           **Contents and Coverage**

  coincall_btc_options_chain_snapshots_2025Q4.parquet   Five-minute-frequency snapshots of the BTC options
                                                        chain for October--December 2025. Each snapshot
                                                        includes all listed expiries with bid, ask, mid,
                                                        mark, and implied volatility for every strike.
                                                        Columns: timestamp, expiry, strike, type, bid, ask,
                                                        mark, mark_iv, underlying_price.

  coincall_calibrated_svi_surfaces_2025Q4.parquet       Pre-calibrated SVI parameters at each five-minute
                                                        snapshot, provided as a baseline. Students will use
                                                        these as the input to the fast revaluation
                                                        pipeline.

  coincall_reference_prices_2025Q4.parquet              Reference theoretical prices computed by
                                                        Coincall\'s internal pricing engine for a
                                                        representative subset of contracts. Used for
                                                        accuracy validation.
  ----------------------------------------------------- ---------------------------------------------------

**Acceptance criteria:**

- Full Coincall BTC options surface (typically 300--500 contracts)
  revalues with full Greek vector in under 5 milliseconds on a single
  CPU core.

- Accuracy: maximum relative error of 1e-4 against the reference prices.

- Library exposes a clean Python API and is importable as a package.

- Unit tests cover all pricers, all Greeks, and the calibrated surface
  adapter.

- Benchmarking results documented in a short technical note with latency
  distributions, not just means.

Week 8 --- Options Market Making Theory and Dynamic Hedging

*Theme: extending GLFT to a multi-Greek inventory penalty, and
integrating a dynamic hedging policy.*

Learning Objectives

- Set up the El Aoud--Abergel framework for market making on options, in
  which inventory is a vector of Greeks.

- Derive the multi-Greek HJB system and identify the structure of the
  inventory penalty as a quadratic form.

- Understand the mechanics and economics of delta and gamma hedging, and
  quantify the P&L attribution of a hedged options book.

- Integrate a dynamic hedging policy with the quoting engine and
  identify the interaction effects.

Lecture 1 --- Multi-Dimensional Inventory and the Multi-Greek HJB

The lecture states the conceptual shift required to extend market making
to options. A single option position is simultaneously a position in the
underlying (delta), in convexity (gamma), in volatility (vega), and in
time decay (theta). The inventory state is therefore a vector, and the
appropriate notion of inventory risk is a quadratic form on that vector.
Following El Aoud and Abergel, the lecture derives the multi-Greek HJB
and applies the now-familiar separation ansatz to reduce it to a PDE on
the inventory vector. The reduction to GLFT in the one-dimensional limit
is verified.

- Greek aggregation across a portfolio of options.

- The inventory vector q = (Δ, Γ, ν, \...) and its dynamics under
  quoting.

- Inventory penalty as a quadratic form: economic interpretation of the
  penalty matrix.

- HJB equation in the multi-Greek setting and the separation ansatz.

- Reduction to a PDE on the inventory vector; closed-form quotes under
  quadratic penalty.

- Truncation: which Greeks enter the optimization, which are managed by
  external hedging.

- Verification of the reduction to GLFT in the one-dimensional case.

Lecture 2 --- Dynamic Hedging and Integration with Quoting

The market making engine produces quotes; a separate or integrated
hedging policy manages the resulting Greek exposures. The lecture covers
the canonical practitioner perspective on delta hedging and gamma
scalping, decomposes the daily P&L of a hedged option book into its
constituent streams, and then covers the two architectures for
integrating hedging with quoting: external hedging by a separate
algorithm that runs at lower frequency, and integrated hedging in which
the quoting engine itself takes hedge orders into account.
Coincall-specific issues are discussed, especially the use of the
perpetual futures contract as the delta-hedging instrument.

- Continuous and discrete delta hedging; the
  gamma--theta--realized-variance identity.

- Gamma scalping mechanics and the P&L distribution of a long-gamma
  position.

- Vega hedging through other options; basis risk and skew risk.

- External hedging policies: threshold-triggered rebalancing.

- Integrated hedging: hedge orders as part of the quoting engine\'s
  action space.

- Cost-aware hedging: balancing risk reduction against transaction
  costs.

- Perpetual futures as the delta-hedging instrument; funding rate
  considerations.

Recitation

Hybrid workshop. The first half is a derivation exercise on the
multi-Greek HJB, performed in pairs with the mentor circulating. The
second half is a simulation exercise: students run a hedged-book
simulation under various hedge policies and compare the resulting P&L
distributions. The recitation closes with a discussion of which hedge
policy will be used in the week 9 milestone backtest.

Required Reading

- El Aoud and Abergel (2015), A Stochastic Control Approach to Option
  Market Making.

- Taleb (1997), Dynamic Hedging, selected chapters on Greek aggregation,
  gamma scalping, and vega risk.

- Cartea, Jaikumar, and Penalva (2015), Chapter 11.

Problem Set 8

1.  Derive the inventory dynamics for a market maker quoting on a
    portfolio of options, with inventory vector q ∈ ℝᵏ representing the
    aggregated Greeks. Identify the precise structure of the jumps when
    a fill occurs.

2.  Set up the HJB equation for the El Aoud--Abergel problem and apply
    the separation ansatz. Reduce the equation to a PDE on the inventory
    vector, and show that it reduces to the GLFT HJB when only one Greek
    is tracked and one option is traded.

3.  Choose a quadratic inventory penalty matrix that reflects the
    empirical covariances of delta, gamma, and vega exposures in a
    representative crypto options portfolio. Justify each entry from one
    week of Coincall data.

4.  Derive the P&L of a continuously delta-hedged short call position
    under Black--Scholes dynamics. Show that the P&L equals the integral
    of half-gamma times the difference between realized and implied
    variance.

5.  Implement a delta-hedging policy that triggers a hedge order when
    \|Δ\| exceeds 0.1 BTC of underlying exposure, and apply it to one
    week of Coincall data. Report the resulting hedging cost and risk
    reduction, and combine the hedger with your GLFT quoting engine from
    week 5 to observe the interaction.

6.  Discuss three modeling assumptions in El Aoud and Abergel (2015)
    that are reasonable for equity options but less appropriate for
    crypto options, and propose a modification for each.

Week 9 --- Backtesting and Risk Analysis

*Theme: assembling the full system and validating it on historical
data.*

Learning Objectives

- Implement an event-driven backtest harness suitable for options market
  making.

- Produce a full P&L attribution that decomposes daily P&L into spread
  capture, inventory drift, gamma scalping, and hedging costs.

- Analyze the resulting risk metrics and identify regimes in which the
  model performs well or poorly.

Lecture 1 --- Backtesting Architecture for Options

Backtesting an options market maker is substantially harder than
backtesting a directional strategy. The lecture covers the architectural
choices: an event-driven simulator that replays order book events, a
fill simulator that probabilistically determines which of the market
maker\'s quotes are filled, and a state machine that tracks the full
inventory and Greek state. Common pitfalls are emphasized.

- Event-driven simulation: clock, event queue, deterministic replay.

- Fill simulator: probabilistic fills conditional on quote distance and
  observed order flow.

- State tracking: cash, inventory by contract, aggregated Greeks, hedge
  position.

- Pitfalls: look-ahead bias, unrealistic fill rates, latency
  assumptions, contract expiry handling.

- Stress tests: known regime shifts in the historical data.

Lecture 2 --- Risk Metrics and P&L Attribution

The lecture covers the standard suite of risk and performance metrics,
but emphasizes attribution. A market maker\'s daily P&L is the sum of
several conceptually distinct streams, and isolating each is essential
for understanding what the strategy is actually doing. The lecture also
covers regime analysis: identifying conditions under which the strategy
outperforms or underperforms.

- Sharpe ratio, Sortino ratio, maximum drawdown, Calmar ratio.

- P&L attribution: spread P&L, inventory P&L, gamma P&L, vega P&L,
  hedging P&L.

- Regime analysis: high-volatility versus low-volatility days.

- Greek-exposure time series and stationarity analysis.

- Capacity analysis: how P&L scales with position limits.

Recitation

Code review of the full backtest. Each student presents one regime (one
week of the three-month window) and walks through the P&L attribution.
The mentor probes the implementation for the pitfalls discussed in the
lecture.

Required Reading

- Cartea, Jaikumar, and Penalva (2015), Chapters 10--11 (re-read).

- Bailey and López de Prado (2014), The Deflated Sharpe Ratio.

- López de Prado (2018), Advances in Financial Machine Learning,
  Chapters 11--13.

Problem Set 9

1.  Implement an event-driven backtest harness that consumes Coincall
    order book and trade events and produces a deterministic replay.
    Validate it by running an identical configuration twice and
    confirming bitwise-identical results.

2.  Implement a fill simulator that models the probability of fill on
    the market maker\'s quotes as a function of quote distance from mid
    and the observed depth of opposite-side flow. Calibrate it from
    historical data and validate the calibration on a holdout period.

3.  Run a full one-month backtest of your multi-Greek market making
    engine on Coincall BTC options. Report mean and standard deviation
    of daily P&L, Sharpe ratio, maximum drawdown, and time series of
    aggregated Greeks.

4.  Decompose the daily P&L into the four attribution streams discussed
    in lecture (spread, inventory, gamma, hedging) and produce a
    stacked-area plot of the cumulative attribution over the backtest
    period.

5.  Identify the day in the three-month window with the worst drawdown
    and produce a forensic analysis of that day: what was the market
    environment, which positions drove the loss, and what (if anything)
    could have been done differently.

Milestone Deliverable: Milestone 3 --- Full Options Market Making
Backtest

Submit a complete backtest of the multi-Greek options market making
engine on three months of Coincall BTC and ETH options data, with full
P&L attribution, risk metrics, and Greek-exposure time series. The
deliverable must include reproducible code, a configuration file
documenting all hyperparameters, and a technical report that analyzes
the results and identifies failure modes.

**Datasets provided by Coincall:**

  -------------------------------------------- ---------------------------------------------------
  **Dataset**                                  **Contents and Coverage**

  coincall_btc_options_l2_2025Q4.parquet       BTC options L2 order book snapshots at 1-second
                                               resolution for October--December 2025. Five levels
                                               each side. All actively quoted contracts.

  coincall_btc_options_trades_2025Q4.parquet   BTC options trade tape for the same period.
                                               Columns: timestamp, contract_id, price, size,
                                               aggressor_side, mark_iv_at_trade.

  coincall_eth_options_l2_2025Q4.parquet       ETH options L2 order book snapshots at 1-second
                                               resolution for the same period.

  coincall_eth_options_trades_2025Q4.parquet   ETH options trade tape for the same period.

  coincall_btc_eth_perp_l2_2025Q4.parquet      BTC and ETH perpetual futures L2 snapshots at 100ms
                                               resolution. Used as the delta-hedging instrument.

  coincall_funding_rates_2025Q4.parquet        Hourly perpetual futures funding rates for BTC and
                                               ETH. Required for accurate hedging cost accounting.
  -------------------------------------------- ---------------------------------------------------

**Acceptance criteria:**

- Backtest is fully reproducible from the provided configuration file.

- P&L attribution sums to total P&L within a tolerance of 1 basis point.

- Sharpe ratio is reported with confidence interval estimated by block
  bootstrap.

- Greek exposure time series remain bounded within the configured
  position limits at all times.

- Technical report is at most twenty pages excluding appendices, and
  includes a forensic analysis of at least one drawdown event.

Week 10 --- Extensions, Final Report, and Presentations

*Theme: pursuing one novel direction and communicating results.*

Learning Objectives

- Select and complete one extension of the baseline model from a menu of
  approved options.

- Write a final research report at the level expected of a quantitative
  research interview or working paper.

- Present the work clearly to a mixed academic and industry audience.

Lecture 1 --- Extension Topics

The lecture surveys the menu of approved extension topics and outlines
what a credible week-long investigation of each would look like.
Students choose by end of day one. The topics are non-trivial but
tractable within the time budget given the infrastructure built over the
preceding nine weeks, and they connect directly to the GLFT-variants
survey from week 5.

- Skew trading: quoting asymmetrically across moneyness based on signals
  derived from the calibrated SVI parameters.

- Term-structure arbitrage detection: identifying when the front and
  back of the term structure imply inconsistent variance forecasts.

- Machine-learned order flow prediction: training a model to predict
  short-horizon order arrivals as an input to the quoting engine.

- Cross-exchange market making: extending the engine to quote
  simultaneously on Coincall and at least one other venue.

- Robust optimization: replacing the point-estimate inventory penalty
  with a worst-case penalty over a confidence set.

- Multi-asset extension: extending the engine to quote BTC and ETH
  options simultaneously with a correlated covariance matrix.

Lecture 2 --- Research Communication

The lecture covers the structure and style of a quantitative research
report: how to motivate a problem, present methodology, report results,
and acknowledge limitations. Examples of well-written papers in the
field are discussed. The lecture closes with guidance for the oral
presentation.

- Structure of a quantitative research paper: abstract, introduction,
  methodology, results, discussion, limitations.

- Writing for an industry audience: avoiding both excessive formalism
  and excessive informality.

- Presenting empirical results: figures, tables, and the use of
  confidence intervals.

- Acknowledging limitations: a sign of strength, not weakness.

- Oral presentation: structure, pacing, and the use of slides.

Recitation

Final dry-run presentations. Each student gives a fifteen-minute
presentation to the cohort, and the cohort provides feedback. The mentor
focuses on questions that an industry audience would ask.

Required Reading

- El Aoud and Abergel (2015), re-read with the extension topic in mind.

- Guéant (2016), the chapter most relevant to the chosen extension.

- One additional paper relevant to the chosen extension, identified by
  the student in consultation with the mentor.

Problem Set 10

1.  Submit a one-page proposal for your chosen extension by end of day
    one of week 10, including problem statement, methodology, expected
    results, and risk factors.

2.  Implement the extension on top of the infrastructure from weeks 5,
    7, and 9.

3.  Quantify the improvement (or lack thereof) over the baseline
    established in week 9 using the same risk and P&L metrics.

4.  Write a final technical report not exceeding thirty pages,
    structured following the lecture\'s guidance, and incorporating all
    previous milestone work.

5.  Prepare and deliver a twenty-minute final presentation to the cohort
    and invited industry guests.

3\. Comprehensive Reference List

The references below are organized by the role they play in the program.
Primary references are required reading; secondary references provide
context and depth; supplementary references support specific weeks or
extension topics.

3.1 Primary References

Avellaneda, M., and Stoikov, S. (2008). High-frequency trading in a
limit order book. Quantitative Finance, 8(3), 217--224.

Guéant, O., Lehalle, C.-A., and Fernandez-Tapia, J. (2013). Dealing with
the inventory risk: a solution to the market making problem. Mathematics
and Financial Economics, 7(4), 477--507.

Guéant, O. (2016). The Financial Mathematics of Market Liquidity: From
Optimal Execution to Market Making. Chapman & Hall / CRC.

El Aoud, S., and Abergel, F. (2015). A stochastic control approach to
option market making. Market Microstructure and Liquidity, 1(1),
1550006.

Cartea, Á., Jaikumar, S., and Penalva, J. (2015). Algorithmic and
High-Frequency Trading. Cambridge University Press.

3.2 Volatility Surface and Options Pricing

Gatheral, J. (2006). The Volatility Surface: A Practitioner\'s Guide.
Wiley Finance.

Gatheral, J., and Jacquier, A. (2014). Arbitrage-free SVI volatility
surfaces. Quantitative Finance, 14(1), 59--71.

Hagan, P. S., Kumar, D., Lesniewski, A. S., and Woodward, D. E. (2002).
Managing smile risk. Wilmott Magazine, September, 84--108.

Hull, J. C. (2021). Options, Futures, and Other Derivatives (11th ed.).
Pearson.

Taleb, N. N. (1997). Dynamic Hedging: Managing Vanilla and Exotic
Options. Wiley.

3.3 Fast Computation Methods

Carr, P., and Madan, D. (1999). Option valuation using the fast Fourier
transform. Journal of Computational Finance, 2(4), 61--73.

Fang, F., and Oosterlee, C. W. (2008). A novel pricing method for
European options based on Fourier-cosine series expansions. SIAM Journal
on Scientific Computing, 31(2), 826--848.

Giles, M., and Glasserman, P. (2006). Smoking adjoints: fast Monte Carlo
Greeks. Risk Magazine, January, 88--92.

Capriotti, L. (2011). Fast Greeks by algorithmic differentiation.
Journal of Computational Finance, 14(3), 3--35.

Glasserman, P. (2003). Monte Carlo Methods in Financial Engineering.
Springer.

3.4 Stochastic Optimal Control

Pham, H. (2009). Continuous-time Stochastic Control and Optimization
with Financial Applications. Springer.

Fleming, W. H., and Soner, H. M. (2006). Controlled Markov Processes and
Viscosity Solutions (2nd ed.). Springer.

Øksendal, B. (2003). Stochastic Differential Equations: An Introduction
with Applications (6th ed.). Springer.

3.5 Market Microstructure

Roll, R. (1984). A simple implicit measure of the effective bid-ask
spread in an efficient market. Journal of Finance, 39(4), 1127--1139.

Glosten, L. R., and Milgrom, P. R. (1985). Bid, ask and transaction
prices in a specialist market with heterogeneously informed traders.
Journal of Financial Economics, 14(1), 71--100.

Kyle, A. S. (1985). Continuous auctions and insider trading.
Econometrica, 53(6), 1315--1335.

O\'Hara, M. (1995). Market Microstructure Theory. Blackwell.

3.6 Supplementary

Bailey, D. H., and López de Prado, M. (2014). The deflated Sharpe ratio:
correcting for selection bias, backtest overfitting, and non-normality.
Journal of Portfolio Management, 40(5), 94--107.

López de Prado, M. (2018). Advances in Financial Machine Learning.
Wiley.

Almgren, R., and Chriss, N. (2001). Optimal execution of portfolio
transactions. Journal of Risk, 3(2), 5--40.

Appendix A. Coincall Dataset Catalog

The following datasets are provided by Coincall to the program. All
datasets are delivered as Parquet files on a secure object store
accessible to enrolled students under a non-disclosure agreement. The
naming convention is consistent across datasets:
coincall\_{instrument}\_{data_type}\_{period}.parquet.

A.1 Order Book Data

Order book data is provided as L2 snapshots, with the top ten price
levels on each side aggregated by quantity. Snapshots are taken at fixed
intervals (1 second for options, 100 milliseconds for perpetual
futures). Each snapshot row contains the bid and ask prices and sizes at
each level, a sequence number that strictly increases within the file,
and an exchange timestamp.

The L2 representation is preferred over L3 for this program for two
reasons: it is sufficient for both calibrating intensity functions and
constructing the simulation environment, and it is several orders of
magnitude smaller, which keeps the data engineering tractable for a
ten-week program.

A.2 Trade Data

Trade data is provided as a tape of all executed trades within the
period. Each trade includes the contract identifier, price, size, the
aggressor side (whether the trade was initiated by a buyer or seller),
and a Coincall trade identifier that can be cross-referenced with the
order book data to identify which resting order was filled.

For options, each trade additionally includes the mark implied
volatility at the time of the trade. This is useful for the volatility
surface calibration in week 6 and for the fill simulator\'s calibration
in week 9.

A.3 Surface Data

Calibrated SVI parameters are provided at five-minute frequency as a
baseline for the fast revaluation pipeline in week 7. Students are
expected to also produce their own calibrations as part of week 6, but
the provided baseline is useful for sanity-checking and for downstream
pipelines.

A.4 Auxiliary Data

Funding rate data for the perpetual futures contracts is provided at
hourly frequency. This is required for accurate accounting of the
hedging cost in week 9. Additionally, a snapshot of the exchange\'s
contract specifications (tick size, lot size, fee schedule, position
limits) is provided as a static file.

A.5 Access and Use

Students will receive credentials to a secure S3-compatible endpoint at
the start of the program. Data may be downloaded locally for analysis
but may not be redistributed or used for any purpose other than the
program. The full terms are specified in the data use agreement that
each student signs at enrollment.

Coincall retains the right to update the dataset catalog during the
program in response to material market events or changes in available
data. Any such updates will be communicated to students and the program
coordinator with at least one week of notice.
