**Tutor Handbook**

**Optimal Market Making for Cryptocurrency Options**

*The Guéant--Lehalle--Fernandez-Tapia Framework and its Extensions*

A 10-Week Summer Research Program

North Carolina State University

Prepared for distribution to teaching assistants,

recitation leaders, and graders

*Program Mentor: Dendi Suhubdy (Bitwyre)*

*Edition: 2026*

How to Use This Handbook

This handbook is the operational companion to the student-facing
syllabus. It is intended for tutors --- teaching assistants, recitation
leaders, and graders --- who will deliver the day-to-day instruction of
the program under the high-level direction of the program mentor. It is
not a substitute for the syllabus; you should read the syllabus first so
that you understand the arc of the program from the student\'s
perspective.

The handbook is organized into four parts. Part I is your orientation:
it covers your role, your relationship with the mentor, the weekly
rhythm of the program, and the policies you will need to enforce. Part
II is the heart of the handbook: a week-by-week teaching guide that
includes lecture emphasis, common student confusions, recitation lesson
plans, problem set solution sketches, and grading rubrics. Part III
provides milestone evaluation rubrics that you will use to grade the
three software milestones. Part IV is an administrative reference
covering academic integrity, late work, accommodations, and crisis
escalation.

If you are new to the program, read Parts I and IV in full before the
first week. Refer to the Part II week section the weekend before each
week, and to the relevant Part III rubric in the week before each
milestone deadline. Part II is intentionally written so that you can
read one week in roughly thirty minutes of focused preparation; the goal
is utility, not exhaustiveness.

Conventions Used in This Handbook

Throughout the document, the following conventions apply:

- Boldface marks the single most important point in a section.

- Italics indicate a quotation from the student-facing syllabus,
  included for cross-reference.

- A "red-flag" icon (annotated in the heading) marks situations where
  you should escalate to the mentor rather than handling the issue
  yourself.

- Grading rubrics are presented as tables with point allocations summing
  to the total for that problem.

All time allocations are recommendations rather than requirements. Adapt
to the cohort in front of you. The recitation lesson plans in particular
are starting points; an engaged cohort may move faster, a struggling one
slower.

Part I. Tutor Orientation

1.1 Your Role

Tutors are responsible for the day-to-day delivery of the program.
Concretely, your responsibilities are: leading the weekly ninety-minute
recitation, holding three weekly office hours of one hour each, grading
weekly problem sets within seven days of submission, providing
first-pass evaluation of milestone deliverables (final evaluation rests
with the mentor), and flagging at-risk students to the mentor within
twenty-four hours of identifying a concern.

Tutors are not responsible for delivering the main lectures (those are
delivered by the mentor or invited faculty) or for unilaterally changing
the syllabus, problem sets, or grading rubrics. If you believe a change
is necessary, raise it with the mentor; the mentor decides.

1.2 Relationship with the Mentor

The program is mentored by Dendi Suhubdy. The mentor sets program
direction, delivers the main lectures, and makes final decisions on
grading disputes and milestone evaluations. Tutors operate under the
mentor\'s direction but are expected to exercise independent judgment
within the scope defined above.

Standing communication channels with the mentor:

- A weekly thirty-minute tutor-mentor sync, held on the same day each
  week, covering the previous week\'s recitation outcomes, problem set
  performance, and any flagged students.

- A shared Slack workspace for asynchronous questions. The mentor
  commits to responding within twenty-four hours during business days.
  Do not wait on Slack for time-critical issues; for those, call.

- An emergency escalation path: a direct phone line for crisis
  situations (student in acute distress, suspected academic integrity
  violation, data security incident). Use sparingly.

1.3 Weekly Rhythm

Your typical week, assuming standard cohort size of six to eight
students, will look like this:

  ---------------- --------------------------------------- ---------------
  **Day**          **Activity**                            **Estimated
                                                           Time**

  Sunday evening   Read the relevant Part II section of    2--3 hours
                   this handbook; prepare recitation       
                   materials; review the previous week\'s  
                   problem set submissions if not yet      
                   complete.                               

  Monday           Attend lecture 1 (you do not deliver,   1.5 hours
                   but you should be present to flag       
                   confusions for the recitation).         

  Tuesday          Office hour 1.                          1 hour

  Wednesday        Attend lecture 2.                       1.5 hours

  Thursday         Lead recitation.                        1.5 hours

  Friday           Office hour 2.                          1 hour

  Saturday         Office hour 3 (typically Saturday       1 hour
                   morning to support weekend problem-set  
                   work).                                  

  Weekend          Grade the previous week\'s problem set; 4--6 hours
                   prepare for the next week.              
  ---------------- --------------------------------------- ---------------

Total weekly commitment is approximately fifteen to twenty hours,
peaking during milestone weeks when you also participate in code review.

1.4 Office Hours Guidance

Office hours are the most variable part of your week. Some weeks you
will have full attendance for the entire hour; other weeks no one will
come. Both are normal. The following principles apply:

- Resist solving problems for students. The instinct is strong; resist
  it. Ask the student to explain what they have tried; ask what they
  think the next step should be; provide the smallest hint that unblocks
  them.

- Distinguish between conceptual confusion and implementation confusion.
  The remedy differs. For conceptual confusion, return to the lecture
  material; for implementation confusion, ask to see the code and read
  it together.

- Watch for the student who comes to every office hour with the same
  kind of confusion. That is a signal worth flagging to the mentor ---
  they may benefit from one-on-one mentor time.

- If two students come with the same question on the same day, it is
  probably a class-wide gap. Note it and address it at the start of the
  next recitation.

- Office hours are not consulting. Do not give code review on milestone
  deliverables during office hours. That happens in scheduled code
  review sessions during milestone weeks. The reason: if you debug a
  student\'s milestone code in office hours, your judgment when grading
  is no longer independent.

1.5 Grading Standards

Consistency matters more than calibration of an individual grade. If you
have two tutors, you must coordinate: grade the same three problems
together for the first problem set to calibrate, and spot-check each
other thereafter. The grading rubrics in Part II are starting points,
not constraints; if you find a rubric is misleading once you have seen
real submissions, raise it with the mentor and the rubric will be
updated.

Specific standards:

- Mathematical derivations are graded on correctness and clarity.
  Skipping a non-trivial step costs at most one point; getting the wrong
  answer with the right structure typically receives roughly half
  credit.

- Implementation problems are graded on correctness, reproducibility,
  and code quality, in that order. Code that runs and produces the right
  answer with poor style is graded above code that does not run at all.

- Discussion problems are graded on substantive engagement. A discussion
  that takes a defensible position and supports it with the material
  from lecture receives full credit; a discussion that restates the
  question without engaging receives zero.

Return graded work within seven days of the submission deadline. Provide
written feedback on at least one problem per problem set, even when full
marks are awarded.

1.6 Tutor Calibration Session

Before the program begins, the mentor holds a half-day tutor calibration
session. The agenda is: review the syllabus; walk through one full week
of teaching notes from this handbook together; grade a sample problem
set (provided by the mentor) as a group; review the milestone rubrics;
and resolve any open questions. Attendance is mandatory.

Part II. Week-by-Week Teaching Notes

Each of the ten weekly sections below is structured identically: the
spine of the week, lecture emphasis notes, common student confusions
with suggested handling, a recitation lesson plan, and the problem set
solution sketches with grading rubric. Read the section for the upcoming
week in full before the Sunday preparation block.

Week 1. Foundations of Market Microstructure

**THE SPINE OF THIS WEEK**

Students must leave this week able to think of a market maker as a
continuously quoting participant whose existence is justified by the
spread, and able to read a limit order book without having to look up
vocabulary. Everything in the next nine weeks builds on this.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Limit Order Book Mechanics

The lecture is intentionally not mathematical; its goal is vocabulary
and institutional fluency. The mentor will move quickly through order
types and matching rules. The important conceptual point, which students
often miss because it is delivered casually, is that price-time priority
creates a queue at each price level and that being earlier in that queue
is a real economic asset. This will matter in week 5 when fill
probabilities are calibrated.

*Watch for student reactions at:*

- When the mentor introduces post-only orders. Students often confuse
  these with limit orders and do not understand the economic motivation.

- When the mentor explains the difference between L2 and L3 data.
  Students with prior equity-finance exposure often think L2 is the only
  thing that exists.

Lecture 2 --- Spread Decomposition and the Role of the Market Maker

Three models are covered in one lecture: Roll, Glosten--Milgrom, and
Kyle. This is fast. The mentor will likely pause to draw the
Glosten--Milgrom decision tree on the board, and that drawing is the
most important artifact of the lecture. Encourage students to copy it
exactly. The Kyle model is included for completeness and is the one
students consistently struggle with; the mentor may downplay it
depending on time.

*Watch for student reactions at:*

- The transition from Roll to Glosten--Milgrom. Students sometimes think
  Glosten--Milgrom is just a fancier version of Roll. It is not: they
  answer different questions.

- The Kyle equilibrium. Several students will be lost. Do not worry;
  week 1 problem 5 does not require Kyle.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why does the market maker    Walk through the time horizon. A market
  quote both sides? Why not    maker commits in advance; a reactive
  just buy low and sell high   trader commits in response. The bid-ask
  reactively?                  spread is the compensation for committing
                               in advance under uncertainty.

  Aren\'t all orders limit     Mathematically yes; institutionally no.
  orders, since a market order Market orders are explicitly different
  is a limit order at          objects on real exchanges because they
  infinity?                    have different fee schedules and matching
                               priority. Refer to the Coincall fee
                               schedule for a concrete example.

  L2 and L3 --- when does it   L3 matters when you care about queue
  matter which you use?        position (your specific order, not
                               aggregate depth). For the calibration work
                               in week 5, L2 is sufficient because we
                               model aggregate intensity rather than
                               individual queue dynamics.

  The Roll estimator gives a   Almost certainly not. The Roll estimator
  different number than the    estimates the unobserved component of the
  observed spread. Bug in my   spread, which differs from the quoted
  code?                        spread by adverse-selection and
                               price-impact effects. The discrepancy is
                               the interesting finding, not a bug.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Every student leaves recitation with a working Python class that
reconstructs an L2 order book from a stream of events. This is the
foundation for everything in week 5 and beyond.

Materials needed:

- A small (one-hour) Coincall BTC-PERP event stream in JSON, distributed
  to students in advance.

- A reference solution to the order book reconstruction class, available
  to the tutor only.

- A laptop projector or shared screen.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--10         Greet the cohort; recap the goal of the week; quick poll on
                which parts of the two lectures landed well and which did
                not.

  10--20        Live demo of loading the data file in Python; show the shape
                of an order event; demonstrate one minute of order book
                reconstruction manually on the whiteboard.

  20--60        Pair programming. Students work in pairs to extend the
                partial scaffold (provided) into a working reconstructor.
                Circulate continuously. The most common bug is forgetting to
                clean up empty price levels after a cancel; if you see this
                in one pair, announce it to the room.

  60--75        Reconvene. One pair presents their reconstructor to the
                room; the cohort debugs any final issues collectively.

  75--90        Wrap-up. Address questions from the lectures that were
                flagged during the cohort poll. If time remains, sketch how
                this code will be extended in week 5 to support a fill
                simulator.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- If most pairs are not converging by minute 50, stop the pair
  programming and walk through the reference solution together. It is
  better that everyone leaves with working code than that some struggle
  through a half-finished version.

- Save the working code; students will reuse it throughout the program.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        10        Working Python class that       Most common error: not
                     reconstructs the L2 book event  handling cancels on empty
                     by event; a plot of mid-price   price levels. -2. Second
                     and quoted spread over one hour most common: incorrect
                     of data.                        handling of the trade event
                                                     (decrementing the wrong
                                                     side). -3. If code does not
                                                     run at all: at most 3 points
                                                     for an apparent design.

  2        8         Roll estimator computed;        Computing the Roll estimator
                     comparison plot with the quoted with the wrong sign
                     spread; brief discussion of the convention (it should be the
                     discrepancy that correctly      square root of negative
                     identifies the role of          serial covariance, and
                     asymmetric information.         students often miss the
                                                     sign). -3. Discussion that
                                                     simply notes the discrepancy
                                                     without engaging: -3.

  3        10        Analytical derivation of the    Skipping the Bayesian update
                     Glosten--Milgrom                step: -3. Confusing the bid
                     quote-setter\'s bid and ask.    with the ask: -2. Failing to
                     Should arrive at expressions    acknowledge that the spread
                     involving the probability of    is endogenously determined
                     informed trading and the prior  by the indifference
                     on asset value.                 condition: -2.

  4        8         Simulation of Glosten--Milgrom  Plotting only one
                     with chosen parameters; a plot  realization rather than
                     of the public belief converging averaging: -2. Using a
                     toward true asset value over a  non-rational prior (e.g.,
                     sequence of trades.             starting the simulation with
                                                     the correct belief): -2.

  5        9         Realized spread and price       Computing realized spread
                     impact computed over a          with the wrong sign of trade
                     five-minute window; discussion  direction: -3. Discussion
                     of order-flow toxicity that     that does not reference the
                     engages with the empirical      actual numbers from the
                     numbers obtained.               data: -3.
  -------- --------- ------------------------------- ----------------------------

Week 2. The Avellaneda--Stoikov Model

**THE SPINE OF THIS WEEK**

Students must leave this week with a complete worked example of the
stochastic-control pipeline: dynamics, HJB, ansatz, ODE reduction,
closed-form solution. Everything in weeks 3--5 will be variations on
this template.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Setup and Dynamics

The lecture establishes the modeling choices. The two most important:
arithmetic Brownian motion for the mid-price (not geometric --- this
matters; the linearity simplifies the HJB enormously), and exponential
utility (which decouples the value function from wealth). Make sure
students appreciate that these are choices made for tractability, not
laws of nature.

*Watch for student reactions at:*

- When arithmetic versus geometric Brownian motion comes up. Some
  students will object; they should be told this is a local
  approximation valid over the trading horizon.

- The introduction of the intensity function. Students often want to
  immediately ask where it comes from empirically; defer this to week 5.

Lecture 2 --- HJB Derivation and Solution

The technical centerpiece of the week. The separation ansatz V(t, x, S,
q) = -exp(-γ(x + qS)) θ(t, q) is the move students must internalize,
because it appears in every subsequent control problem in the program.
The mentor will derive the reduced ODE system carefully; this is the
place where attendance matters most.

*Watch for student reactions at:*

- The moment the ansatz is introduced. If students do not understand why
  this is the right ansatz, they will not understand any subsequent HJB
  reduction. Plan to revisit in recitation.

- The boundary terms. Students often miss that the terminal condition
  feeds into the asymptotic expansion.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why exponential utility? It  It is unrealistic; this is purely a
  seems unrealistic to assume  tractability choice. CARA decouples the
  traders have CARA            value function from wealth, which makes
  preferences.                 the problem solvable. Without it, you
                               cannot make analytical progress. The
                               mentor\'s view: model market makers\'
                               \"effective\" risk preferences over a
                               short horizon, not their lifetime
                               preferences.

  The ansatz seems to come out It does, in the sense that there is no
  of nowhere.                  algorithm for guessing ansätze. But it is
                               principled: under exponential utility plus
                               arithmetic mid-price dynamics, the value
                               function inherits a multiplicative
                               structure across the state variables,
                               which the ansatz reflects. Students should
                               accept this on faith for now; we will see
                               the same pattern in three more weeks.

  Why is the optimal           Different quantities. The reservation
  half-spread symmetric in     price is the indifference point
  inventory, but the           (asymmetric because being long shifts your
  reservation price            indifference point lower). The optimal
  asymmetric?                  half-spread is the width of the quoting
                               band around that reservation point
                               (approximately symmetric to first order).
                               They are independent design choices.

  My P&L is huge in            No. The Avellaneda--Stoikov simulation
  simulation. Is that          assumes you are alone in the market and
  realistic?                   the order flow is exogenous. Real markets
                               have competitors and the order flow
                               responds to your quotes. Weeks 5 and 9
                               calibrate to real Coincall data and the
                               P&L estimates become more realistic.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Every student completes the HJB derivation on the whiteboard with
the cohort, then implements the simulation and runs sensitivity analysis
on the risk-aversion parameter.

Materials needed:

- Whiteboard or large shared canvas for the derivation.

- A Python notebook scaffold for the simulation, with the dynamics and
  intensity functions implemented but the quote-computation left blank.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--30         Group derivation on the whiteboard. The tutor leads, but
                students contribute each step. Aim to complete the
                derivation from dynamics through reduced ODE in thirty
                minutes.

  30--60        Pair programming: students fill in the quote-computation
                function in the provided notebook. Most pairs will get this
                working in twenty minutes; remaining time is for the
                simulation.

  60--80        Run the sensitivity analysis: each pair varies γ over three
                orders of magnitude and reports back the inventory variance
                and Sharpe ratio. Aggregate results on the projector.

  80--90        Discussion. What does the sensitivity plot tell us about the
                model? Where would you set γ for a real market making
                operation? Tie this to problem 4.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- The whiteboard derivation is the single most important hour of the
  program for many students. Take your time. If you do not finish in
  thirty minutes, continue into the implementation slot --- the
  implementation can be deferred to the problem set if necessary.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        15        Complete HJB derivation,        Missing the Itô term for the
                     separation ansatz, reduction to underlying: -4. Incorrect
                     ODE system. Every step          treatment of the jump in the
                     justified.                      wealth process: -4. Wrong
                                                     sign in the cash dynamics:
                                                     -2.

  2        10        Closed-form asymptotic          Wrong limit assumption: -2.
                     solution: reservation price and Algebra errors in the
                     half-spread. Should arrive at r half-spread: -3.
                     = S − qγσ²(T−t) and δ =         
                     (1/γ)log(1+γ/κ) + (γσ²/2)(T−t). 

  3        12        Working AS engine in Python;    Symmetric baseline not
                     one-day simulation with stated  actually symmetric (drift in
                     parameters; P&L distribution    quotes): -3. Comparing wrong
                     comparing optimal vs symmetric. distributions: -3. Code does
                                                     not run: at most 4 points
                                                     for design.

  4        10        Sensitivity analysis on γ;      Only one γ value tested: -5.
                     plots of inventory variance and Wrong axis scaling (linear
                     Sharpe vs γ; identification of  when log is required): -2.
                     optimal regime.                 

  5        8         Discussion of three empirical   Listing without explanation:
                     violations of the independence  -3. Failing to discuss
                     assumption. Should engage with  consequences for the
                     phenomena like price impact,    strategy: -3.
                     adverse selection, and          
                     competitor effects.             
  -------- --------- ------------------------------- ----------------------------

Week 3. Stochastic Optimal Control in Continuous Time

**THE SPINE OF THIS WEEK**

Students should leave with the abstract template --- dynamic programming
principle, HJB equation, verification theorem --- and the ability to
recognize when a problem fits the template. The Merton problem is the
second worked example; it should reinforce, not introduce, the pattern
from week 2.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Dynamic Programming and the HJB Equation

The abstract version of last week. The mentor will derive the HJB
equation in generality, treating the previous week\'s
Avellaneda--Stoikov as a special case. Students who struggled last week
often have an epiphany here; students who breezed through last week
sometimes find this lecture unexciting. Both reactions are normal.

*Watch for student reactions at:*

- The infinitesimal generator. Students with weak stochastic-calculus
  background often need this re-explained.

- Viscosity solutions. The mentor will mention them briefly. Do not let
  students get stuck on this; viscosity solutions are not central to the
  program.

Lecture 2 --- Verification Theorems and Tractable Utility Functions

The verification theorem is the missing piece from week 2: it tells you
that the solution you find by ansatz is actually the value function. The
lecture will state the theorem precisely and sketch the proof. The
CARA-versus-CRRA discussion that closes the lecture is also important;
some students will only fully understand the choice of CARA in week 2
after seeing the comparison with CRRA in Merton\'s problem.

*Watch for student reactions at:*

- Smoothness conditions in the verification theorem. Students sometimes
  ask whether these conditions hold for the GLFT problem --- they do,
  but it takes work to show; defer.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why is the HJB equation a    The HJB encodes the dynamic programming
  necessary condition?         principle, which is necessary by
  Couldn\'t there be other     definition (any optimal policy must be
  optimal policies?            optimal at every later time conditional on
                               the current state). The verification
                               theorem provides sufficiency.

  The Merton problem under     This is exactly the point. CARA
  CRRA has wealth in the       exponential utility makes the marginal
  policy, but                  utility of wealth constant, which makes
  Avellaneda--Stoikov under    the optimal policy independent of wealth.
  CARA does not. Why?          CRRA does not have this property; the
                               optimal portfolio share is constant in
                               wealth but the dollar amount scales.
                               Encourage the student to write out both
                               derivations side by side.

  What is the difference       Verification: \"if you have a smooth
  between a verification       solution, it is the value function.\"
  theorem and an existence     Existence: \"a solution exists.\" In our
  theorem?                     program we always have a candidate
                               solution (we constructed it), so we only
                               need verification.

  Why do we ignore viscosity   Because all the problems in this program
  solutions when the textbook  have smooth value functions. Viscosity
  makes such a big deal of     solutions matter for problems with free
  them?                        boundaries or non-smooth payoffs (e.g.,
                               American options). Our problems are smooth
                               enough that classical theory suffices.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Students complete the Merton problem under CARA from scratch, then
under CRRA, and observe the structural difference between the two
solutions.

Materials needed:

- Whiteboard for the derivations.

- A short reference sheet with the Itô formula, the dynamic programming
  principle, and the HJB equation, for students to consult.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--10         Quick recap of HJB. Solicit one-sentence statements of the
                dynamic programming principle from three students.

  10--45        Group derivation of the Merton problem under CARA. The tutor
                guides; students contribute each step.

  45--75        Group derivation under CRRA. Move faster; students should be
                more confident by now.

  75--90        Side-by-side comparison of the two solutions. Explicit
                discussion: why does wealth appear in one and not the other?
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- If the cohort is strong, you can save thirty minutes by doing CARA
  quickly and spending most of recitation on Almgren--Chriss (problem 3)
  instead. Adjust based on energy level.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        12        Merton problem under CRRA, with Incorrect ansatz: -4.
                     full derivation. Optimal        Missing the HJB
                     consumption and portfolio share transversality: -3. Wealth
                     constant in wealth.             appearing in the wrong place
                                                     in the policy: -2.

  2        10        Merton problem under CARA, with Same as problem 1, plus
                     full derivation. Optimal        failure to articulate the
                     portfolio dollar amount         structural difference: -2.
                     constant in wealth.             

  3        12        Almgren--Chriss optimal         Skipping the calculus of
                     execution. Optimal trajectory   variations step: -4. Wrong
                     derived; comparison with        boundary conditions: -3.
                     discrete-time result.           

  4        10        Verification theorem in own     Restating the theorem
                     words; identification of each   verbatim: -5. Counterexample
                     assumption\'s role;             that does not actually fail
                     counterexample with one         the theorem: -3.
                     assumption failing.             

  5        6         Two-paragraph essay on          Plagiarism from the
                     viscosity solutions and the     textbook: 0. Missing the
                     obstacle problem.               obstacle problem entirely:
                                                     -3.
  -------- --------- ------------------------------- ----------------------------

Week 4. The GLFT Model, Part I --- Setup and HJB Derivation

**THE SPINE OF THIS WEEK**

GLFT is presented as Avellaneda--Stoikov with two generalizations:
arbitrary intensity functions and bounded inventory. Students should be
able to derive the GLFT HJB by analogy with week 2, identifying exactly
where the generalizations enter.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- The GLFT Setup

Conceptually a setup lecture rather than a technical one. The two key
generalizations are clearly flagged, and the mentor will discuss why
both matter in practice: arbitrary intensities because exponential
intensities are an empirical fiction, and bounded inventory because no
real market maker would tolerate unbounded position growth. Students
should leave the lecture confident that the GLFT problem is well-posed.

*Watch for student reactions at:*

- When the inventory bounds q_min, q_max are introduced. Students
  sometimes confuse these with the asymptotic limits.

- When the mentor defines admissible quote ranges (no quoting beyond the
  inventory bound). The treatment is subtle.

Lecture 2 --- HJB Derivation in the GLFT Framework

The HJB derivation is closely parallel to week 2, with two new features:
the intensity functions are general rather than exponential, and the
inventory boundary requires careful treatment. The mentor will derive
carefully but quickly, relying on the cohort\'s familiarity with the
template from week 2.

*Watch for student reactions at:*

- The boundary conditions at q_min and q_max. These are the most subtle
  part of the derivation; expect questions in the next office hour.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why not just use exponential Exponential intensities are a strong
  intensities and skip this    assumption: they imply that the
  generalization?              probability of fill drops geometrically
                               with distance from mid. Empirically (we
                               will see in week 5) the decay is often
                               slower, especially in the tails. The
                               generalization allows the model to fit
                               reality.

  What does \'arbitrary        Yes: the intensity must be positive,
  intensity function\'         decreasing in quote distance, and satisfy
  actually mean? Are there     some integrability conditions for the HJB
  restrictions?                to be well-posed. Read Section 2 of the
                               GLFT paper for the precise statement. In
                               practice, almost any reasonable parametric
                               family works.

  The boundary conditions at   No. Terminal condition: what happens at
  q_min and q_max are          time T. Boundary condition: what happens
  confusing. Are they the same at the inventory limits. They are
  as the terminal condition?   independent. The boundary conditions
                               encode that you stop quoting on the side
                               that would push you further into the
                               constraint.

  How is the asymptotic regime It is: the asymptotic regime is where T −
  defined? Just T → ∞?         t is large enough that the terminal
                               effects are negligible. We will use a
                               closed-form expression for the asymptotic
                               quotes in week 5; the technicalities of
                               the limit are sketched in the paper but
                               not central.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: The cohort re-derives the GLFT HJB step by step on the whiteboard,
with explicit attention to the points where the generalization from
Avellaneda--Stoikov enters.

Materials needed:

- Whiteboard or shared canvas.

- A copy of the week 2 whiteboard derivation, projected on a separate
  screen for side-by-side comparison.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--15         Recap of last week. Solicit a one-sentence statement of the
                difference between AS and GLFT from each student.

  15--60        Group derivation of the GLFT HJB. At each step, ask
                explicitly: \"is this step the same as Avellaneda--Stoikov,
                or different?\" When different, why?

  60--80        Discussion of intensity function choices. The tutor presents
                three families (exponential, power-law, logistic) and asks
                the cohort which they would calibrate to which kind of order
                flow.

  80--90        Wrap-up. Preview of week 5: closed-form solution in the
                asymptotic regime.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- The side-by-side comparison with week 2 is the pedagogical device that
  makes this recitation work. Students who can articulate the difference
  between AS and GLFT have understood the material; those who cannot
  have not.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        15        Complete GLFT HJB derivation    Missing boundary conditions:
                     with boundary conditions.       -5. Treating Λ as
                     Identification of the precise   exponential without
                     step where Λ regularity is      explicitly noting the
                     needed.                         generalization: -3.

  2        8         Algebraic reduction of GLFT to  Algebra errors: -2 each.
                     AS HJB under Λ(δ) = A exp(-κδ). Failure to relax the
                                                     inventory constraint: -3.

  3        10        Three intensity families        Plotting only without
                     plotted and compared, with      discussion: -4. Discussion
                     discussion of the behavioral    that does not connect to
                     assumptions each encodes.       trader behavior: -3.

  4        8         Inventory dynamics derived      Treating the jump term
                     under generic Λ; expected       incorrectly: -3. Computing
                     change computed.                variance instead of
                                                     expectation: -2.

  5        9         One-page summary of modeling    Failing to distinguish
                     differences between AS and      substantive from notational:
                     GLFT, distinguishing            -4. Going over one page: -1
                     mathematical from notational    (we are training for
                     differences.                    industry research notes).
  -------- --------- ------------------------------- ----------------------------

Week 5. The GLFT Model, Part II --- Asymptotic Solution, Implementation,
and Variants

**THE SPINE OF THIS WEEK**

Two distinct deliverables this week: students must understand the
closed-form asymptotic solution and submit Milestone 1, the linear-asset
GLFT engine. The variants survey is self-study; do not let it eat
lecture or recitation time.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- The Asymptotic Regime and Closed-Form Quotes

The technical centerpiece of the program so far. The change of variable
u(q) = θ(t, q)/θ(t, q+1) linearizes the coupled ODE system into a linear
eigenvalue problem. Students will be told this is \"the trick that makes
the paper work\" --- and it is. The mentor will derive it carefully and
may extend the lecture if students are following well.

*Watch for student reactions at:*

- The change of variable. If students do not understand why this
  particular ratio works, they will not understand the closed-form
  solution. Re-derive in office hours if needed.

- The Perron--Frobenius theorem. Some students will not have seen it
  before; the lecture will not stop to explain. Plan a five-minute aside
  in recitation.

Lecture 2 --- Numerical Implementation and Validation

The transition from theory to code. The mentor will demonstrate the
implementation live: setting up the linear system, calibrating
intensities from data, and running a simulation. This is also the
lecture where the milestone deliverable is formally announced and the
rubric is reviewed.

*Watch for student reactions at:*

- The intensity calibration step. Students often want to use a simple
  curve fit but will get poor results; maximum likelihood is required
  and the mentor will show why.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why is the change of         Because the ODE system has a
  variable u(q) = θ(t, q)/θ(t, multiplicative coupling between θ(t, q)
  q+1) and not the natural     and θ(t, q+1) that becomes linear under
  log?                         the ratio. Taking logs first does not
                               produce a linear system; taking the ratio
                               first does. This is one of those choices
                               that is hard to motivate in advance and
                               obvious in retrospect.

  My linear system is          Most likely you have not enforced the
  singular. What did I do      boundary condition properly at q_max. The
  wrong?                       asymptotic linear system needs an explicit
                               normalization (e.g., u(q_max) = 1) to
                               remove the multiplicative gauge.

  The calibrated intensity     Probably not at first. Crypto fill data is
  functions look implausible   noisy and the maximum likelihood fit on a
  --- should I be worried?     small sample can give surprising
                               parameters. Try fitting on one week, then
                               two weeks, then four. The estimates should
                               stabilize.

  My backtest P&L is negative. Possibly, but more likely: (a) the spread
  Is the model wrong?          is too tight relative to the calibrated
                               intensities, (b) the inventory penalty is
                               too small, or (c) the data window
                               contained a regime shift. Have the student
                               check all three before suspecting the
                               model.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Students complete the change-of-variable derivation, code review
one student\'s milestone-in-progress, and identify any remaining bugs
before the milestone deadline.

Materials needed:

- Whiteboard.

- A projector for live code review (one student\'s code, with their
  permission).

- A list of expected milestone bugs, prepared by the tutor in advance
  based on office hours that week.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--25         Whiteboard derivation of the change of variable, leading to
                the linear eigenvalue problem. Aside on Perron--Frobenius
                (five minutes within this block).

  25--70        Live code review. One student volunteer; their code
                projected. The cohort identifies issues. The tutor
                moderates; the volunteer should leave with a working
                implementation.

  70--85        Open Q&A on the milestone. Common questions: what counts as
                \"non-trivial fit\" for the calibration? What if my latency
                is 150µs instead of 100µs? How long should the technical
                report be?

  85--90        Wrap-up. Reminder of milestone deadline.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- The code review is the high-value activity. It will reveal common bugs
  across the cohort, which you can address in the wrap-up.

- Do not let the variants survey discussion happen in recitation. It is
  self-study. If students want to discuss it, send them to office hours.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        12        Change-of-variable derivation;  Wrong limit assumption: -3.
                     linear system in the asymptotic Algebra errors in the change
                     regime.                         of variable: -2 each.
                                                     Missing the normalization
                                                     that fixes the gauge: -2.

  2        8         Linear system solved            Singular system (no
                     numerically for stated          normalization): -3. Wrong
                     parameters; half-spread plotted sign convention on quote
                     as a function of inventory.     distance: -2.

  3        10        Reproduction of Figure 2 of     No commentary: -4.
                     GLFT (2013), with commentary on Reproducing the wrong
                     discrepancies.                  figure: -3 (read the
                                                     assignment).

  4        10        Maximum-likelihood calibration  Using OLS instead of MLE:
                     of intensities on one week of   -4. Failing to report
                     Coincall data; fitted           goodness-of-fit: -3.
                     parameters and goodness-of-fit  
                     reported.                       

  5        12        Full one-month backtest; all    Missing the symmetric
                     five performance metrics        baseline: -4. Missing one or
                     reported; comparison against    more metrics: -2 each.
                     symmetric baseline.             Reporting metrics without
                                                     time-series plots: -2.

  6        5         Two-page summary of Guéant      Going over two pages: -1.
                     (2016) Chapters 10--11;         Failing to select a specific
                     selection of one variant most   variant: -2. Summary that is
                     relevant to crypto options.     purely descriptive without
                                                     engaging with relevance: -3.
  -------- --------- ------------------------------- ----------------------------

Milestone Week Note

MILESTONE WEEK. Milestone 1 is due at the end of this week. See Part
III, Section 1 for the full evaluation rubric. As a tutor, your role
this week is heavier than usual: in addition to the recitation, you
participate in milestone code review at the end of the week. Block out
four hours of code review time in addition to your usual office hours.

Week 6. Options Pricing, the Volatility Surface, and Calibration

**THE SPINE OF THIS WEEK**

A two-track week. Conceptually: implied volatility surfaces and the
constraints they must satisfy. Practically: calibrate SVI and SABR to
Coincall data and discover how messy real crypto options data is.
Students should leave knowing that calibration is half craft and half
theory.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Greeks and the Volatility Surface

A brisk review of Greeks for students who have taken derivative pricing,
plus a careful treatment of the no-arbitrage constraints on the
volatility surface. The lecture will spend the most time on calendar and
butterfly arbitrage, because these are the constraints that get violated
by naive parameterizations. Vanna and volga are introduced; they will
not be tested for full understanding until week 8.

*Watch for student reactions at:*

- The transition from the Black--Scholes formula to the Greeks. Students
  with weak Black--Scholes background will need this revisited in office
  hours.

- The arbitrage constraints. These are presented as inequalities;
  students sometimes miss that they are necessary and not sufficient.

Lecture 2 --- Parameterization and Calibration

The lecture presents SVI and SABR as the two dominant parametric
families and walks through calibration practically. The mentor will
live-demo a calibration on a Coincall snapshot and show that the first
attempt usually has stability issues; this is intentional, to teach the
lesson that crypto calibration is hard.

*Watch for student reactions at:*

- The live calibration. Students should see it fail in interesting ways
  and watch the mentor diagnose. The diagnostic process is more valuable
  than the eventual fit.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why two parameterizations?   They encode different priors. SVI is
  Why not just one?            parameterized in implied variance and is
                               natural for arbitrage-free conditions.
                               SABR is parameterized in stochastic
                               volatility model parameters and is natural
                               when you want to extrapolate beyond the
                               observed strikes. We will use both because
                               they fail in different regimes.

  My SVI calibration has huge  Probably not. Far OTM puts in crypto have
  residuals on far OTM puts.   wide spreads and low volume; the mid-quote
  Bug?                         may be unreliable. Weighting the
                               calibration by volume or by inverse spread
                               is the standard remedy.

  The SVI parameters look very Yes and no. Day-to-day variation in market
  different from one day to    conditions causes real variation, but a
  the next. Is this normal?    well-calibrated parameter set should not
                               jump wildly. If your fits are unstable,
                               your initial guess is probably the issue;
                               try seeding from yesterday\'s fit.

  The Hagan SABR formula gives Hagan is a small-time approximation. For
  a different price than my    short maturities (under three months) it
  Monte Carlo. Which is right? is excellent; for longer maturities the
                               error grows. Monte Carlo is the truth. The
                               discrepancy is informative, not a bug.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Every student produces a working SVI and SABR calibration on a
Coincall BTC options snapshot, with diagnostic plots, by the end of the
session.

Materials needed:

- A specific Coincall BTC options chain snapshot (chosen by the tutor in
  advance, ideally one with reasonably clean data so that the
  calibration succeeds in recitation time).

- A starter notebook with the SVI and SABR pricing functions
  implemented, leaving calibration to the student.

- Reference diagnostic plots from the tutor\'s own calibration of the
  same snapshot.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--10         Recap; show the chosen snapshot; explain what \"successful\"
                calibration looks like.

  10--55        Pair programming. Each pair calibrates SVI first, then SABR.
                Tutor circulates and helps with optimizer convergence
                issues.

  55--80        Each pair presents their fit with diagnostic plots. The
                cohort discusses sources of disagreement between pairs.

  80--90        Discussion of next week\'s milestone and how the calibrated
                surface feeds into it.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- If the chosen snapshot turns out to be too clean, the lesson about
  \"crypto calibration is hard\" will not land. Have a backup snapshot
  with one or two problematic strikes ready, and switch if recitation is
  going too smoothly.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        10        Vanna and volga derivations     Algebra errors: -2 each.
                     under Black--Scholes;           Failing to verify
                     finite-difference verification. numerically: -3.

  2        10        SVI implementation with         Implementing raw SVI without
                     arbitrage-free constraints;     the constraint checks: -4.
                     explicit demonstration of which Not actually demonstrating
                     constraints fail on a           violations: -3.
                     deliberately broken             
                     parameterization.               

  3        10        SVI calibration to one          Reporting only the RMS error
                     snapshot; fitted parameters,    without per-strike
                     residuals, RMS error reported.  residuals: -3. Optimizer
                                                     failing to converge and
                                                     student not noticing: -3.

  4        10        SABR calibration to the same    Comparison that does not
                     snapshot; comparison with SVI.  engage with strengths and
                                                     weaknesses: -3. Calibration
                                                     that does not converge: -3.

  5        10        One-month daily SVI             Producing the time series
                     calibration; time series of     without commenting on
                     parameters; proposed smoothing  stability: -3. Smoothing
                     scheme.                         scheme that does not
                                                     actually address the
                                                     observed instability: -3.
  -------- --------- ------------------------------- ----------------------------

Week 7. Fast Computation of Prices, Greeks, and Surfaces

**THE SPINE OF THIS WEEK**

The week is about latency. Students must internalize that a working but
slow pricer is not enough for an options market maker. The two technical
tools --- characteristic function pricing and algorithmic
differentiation --- are the means; the end is a five-millisecond surface
revaluation.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Characteristic Function Pricing

Carr--Madan and Fang--Oosterlee are both covered, but Fang--Oosterlee
(COS) is the workhorse. The lecture spends more time on COS because it
is what students will use for the milestone. Carr--Madan is included for
historical context and because it remains common in legacy systems.

*Watch for student reactions at:*

- When the characteristic function of the Heston model is introduced.
  The expression is complex; students will not derive it themselves but
  should recognize its structure.

- The truncation interval in COS. Students sometimes choose it too
  narrow and get artifacts; the mentor will show this.

Lecture 2 --- Algorithmic Differentiation and Vectorization

The conceptual lecture of the program for systems-minded students. The
mentor will distinguish forward-mode from reverse-mode AD, demonstrate
JAX live, and show the latency impact. C++ AAD via Enzyme is mentioned
as advanced material; mentor may go deeper depending on cohort interest.

*Watch for student reactions at:*

- The complexity bound for reverse-mode AD. Students with CS background
  will get this immediately; mathematicians may need it stated twice.

- The transition from grad/jacrev to vmap. The benefit is large and
  worth dwelling on.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why are characteristic       For European options under Black--Scholes,
  function methods faster than they are not faster --- Black--Scholes is
  Black--Scholes for European  closed form and optimal. The point is that
  options? Black--Scholes is   under Heston or any model where you do not
  closed form.                 have closed-form prices, characteristic
                               function methods give you near-closed-form
                               speed (FFT in log-K, COS as a series
                               expansion).

  What is the difference       Forward-mode: O(input dim) cost per
  between forward-mode and     output. Reverse-mode: O(output dim) cost
  reverse-mode AD?             per input. For Greeks (many outputs, few
                               inputs), reverse-mode wins. Encourage
                               students to derive the complexity bounds
                               themselves.

  My JAX implementation is     Almost certainly: you are not using jit,
  slower than NumPy. Did I do  or you are recompiling on every call. JAX
  something wrong?             traces and compiles; the first call is
                               slow, subsequent calls are fast. Use
                               jax.jit and ensure the function signature
                               is static.

  I cannot get my COS pricer   Most likely the truncation interval is
  to match Monte Carlo within  wrong. Compute it from the cumulants of
  1e-4. Help?                  the characteristic function (the lecture
                               covered this) rather than guessing. Second
                               most likely: not enough COS terms; try N =
                               2\^10 or higher.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Every student profiles a naive pricer, applies AD and
vectorization, and measures at least one order of magnitude speedup.
This is the dress rehearsal for the milestone.

Materials needed:

- A naive Python implementation of the COS pricer (no JAX, no vmap, just
  a loop), provided to students.

- A standardized portfolio of fifty Heston-priced options for the
  benchmark.

- A reference implementation showing the target performance (tutor
  only).

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--10         Recap. Show the latency budget: 5ms per surface revaluation,
                200 revaluations per second, 300+ options per surface ---
                that\'s a hard problem.

  10--40        Profile the naive implementation. Each student identifies
                the bottleneck (usually the per-option price call inside a
                Python loop).

  40--70        Convert to JAX with vmap and jit. Re-benchmark. Most
                students will see 10x to 100x speedup.

  70--85        Add AAD: replace finite-difference Greeks with jax.grad.
                Re-benchmark. Most students will see another 5x to 10x.

  85--90        Discuss what is left to optimize before the milestone.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- Have the reference implementation timings ready; students need to know
  what \"good\" looks like.

- C++ via Enzyme is for the strong students. If one or two students are
  coasting, suggest the Enzyme exercise; do not require it.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        10        Carr--Madan FFT pricer for      Wrong dampening parameter
                     Heston European calls;          (α): -3. Failing to verify
                     convergence rate reported.      against Monte Carlo: -3.

  2        10        COS pricer for the same         Wrong truncation interval:
                     problem; accuracy and runtime   -3. Failing to compare
                     comparison with FFT.            runtime: -2.

  3        10        Forward-mode AD derived by hand Skipping the dual-number
                     for Black--Scholes call;        arithmetic: -4. Failing to
                     verification against analytical verify: -3.
                     Greeks.                         

  4        12        JAX-based full Greek vector for Not using jit (slow): -3.
                     fifty options; runtime          Computing only first-order
                     comparison with                 Greeks: -3.
                     finite-difference.              

  5        8         JAX vmap vectorization;         Not reporting in the
                     reported speedup in nanoseconds requested units: -2. Speedup
                     per evaluation.                 of less than 10x:
                                                     investigate, not a deduction
                                                     per se.

  6        10 (extra C++ via Enzyme: AAD performance Optional. Award up to 10
           credit)   comparison against JAX.         points of extra credit; do
                                                     not deduct from base grade.
  -------- --------- ------------------------------- ----------------------------

Milestone Week Note

MILESTONE WEEK. Milestone 2 is due at the end of this week. See Part
III, Section 2 for the full evaluation rubric. The latency target is
non-negotiable: a library that revalues the surface in 5.5ms instead of
5ms does not pass the milestone. Be prepared for student arguments on
this point; refer them to the rubric.

Week 8. Options Market Making Theory and Dynamic Hedging

**THE SPINE OF THIS WEEK**

The conceptual centerpiece of the program. Students must understand that
options market making is GLFT with a vector-valued inventory, and they
must understand how the resulting quoting strategy interacts with an
explicit hedging policy. This is the most cognitively demanding week.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Multi-Dimensional Inventory and the Multi-Greek HJB

El Aoud and Abergel\'s paper, presented carefully. The lecture builds on
GLFT by replacing the scalar inventory with a vector of Greeks and the
scalar inventory penalty with a quadratic form. The mentor will derive
the multi-Greek HJB and verify that it reduces to GLFT in the
one-dimensional case. Students who have understood weeks 2--5 will
follow; those who have not will struggle.

*Watch for student reactions at:*

- The introduction of the inventory vector. Students often need a moment
  to realize that they have been thinking of inventory as a scalar all
  program; it is.

- The penalty matrix. Some students will want to set it to the identity;
  the mentor will discourage this. Defer to office hours for the
  discussion of how to choose it.

Lecture 2 --- Dynamic Hedging and Integration with Quoting

The practitioner lecture, drawing heavily on Taleb. The
gamma--theta--variance identity is derived and forms the conceptual
core. The integration of hedging with quoting is presented as a design
choice --- external versus integrated --- with explicit pros and cons.
The Coincall perpetual futures contract is discussed as the
delta-hedging instrument.

*Watch for student reactions at:*

- The gamma--theta--variance identity. This is the conceptual key to
  options trading; students must understand it.

- The funding rate on perpetuals. Students from a traditional finance
  background may not have encountered this.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  Why is the inventory a       Because the relevant risks are aggregated
  vector and not just a list   Greeks, not individual contract positions.
  of scalar positions?         A market maker who is long one call and
                               short one call at different strikes has
                               zero contract position but non-zero gamma
                               and vega. The vector formulation captures
                               this.

  How do I choose the penalty  The identity penalizes a unit of delta
  matrix? Why not just the     exposure equally to a unit of gamma
  identity?                    exposure. But the empirical risks of unit
                               delta and unit gamma are very different.
                               Calibrate the penalty matrix to the
                               empirical covariance of the Greek
                               processes, or to the desired
                               risk-equivalence (e.g., one unit of delta
                               risk equals one unit of vega risk at some
                               volatility scale). The choice is part of
                               the model design.

  The gamma--theta--variance   Yes and no. The identity is exact under
  identity seems too simple.   Black--Scholes; in reality, additional
  Is that really all there is  terms enter for stochastic volatility,
  to it?                       jumps, and discrete hedging. But the
                               identity is the right starting point and
                               explains 80% of the daily P&L of a hedged
                               book.

  Should I delta-hedge with    Perpetual futures, for two reasons: lower
  perpetual futures or with    transaction costs (no settlement), and
  the underlying?              Coincall\'s options are quoted against the
                               perpetual price index. The funding rate is
                               a small but real cost that must be
                               accounted for; it shows up in the
                               milestone 3 backtest.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Students complete the multi-Greek HJB derivation and run a
hedged-book simulation under two hedging policies (external threshold vs
continuous), comparing the resulting P&L distributions.

Materials needed:

- Whiteboard for the derivation.

- A simulation scaffold for a hedged book under specified Heston
  dynamics.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--35         Group derivation of the multi-Greek HJB. The reduction to
                GLFT in the one-dimensional case is the verification step at
                the end.

  35--70        Pair programming. Each pair runs the hedged-book simulation
                under two policies. P&L distributions are aggregated on the
                projector.

  70--85        Discussion. Which policy wins in which regime? Why? Tie to
                the design choice for milestone 3.

  85--90        Wrap-up. Preview of milestone 3 and the role of the
                perpetual futures contract.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- This is the second-most-important whiteboard derivation in the program
  (after week 2). Move slowly enough that every student is following.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        10        Inventory dynamics for a        Missing the multi-contract
                     portfolio of options; jump      structure: -3. Wrong Greek
                     structure on fills.             aggregation: -3.

  2        15        El Aoud--Abergel HJB            Skipping the verification
                     derivation; separation ansatz;  that it reduces to GLFT: -4.
                     reduction to PDE on inventory   Algebra errors in the
                     vector; reduction to GLFT in 1D multi-dimensional case: -3
                     limit.                          each.

  3        10        Penalty matrix calibrated to    Using the identity matrix:
                     Coincall data; entries          -4. Failing to justify
                     justified from empirical Greek  entries from data: -4.
                     covariances.                    

  4        10        Gamma--theta--variance identity Wrong sign on theta: -2.
                     derived for a continuously      Missing the half-factor in
                     hedged short call.              front of gamma: -2. Failing
                                                     to identify the
                                                     realized-vs-implied variance
                                                     term: -3.

  5        10        Threshold delta-hedging policy  Missing the integration with
                     implemented on one week of      GLFT: -4. Reporting only
                     Coincall data; hedging cost and cost without risk reduction:
                     risk reduction reported;        -3.
                     integration with GLFT engine.   

  6        8         Three modeling assumptions in   Listing without proposing
                     El Aoud--Abergel critically     modifications: -3.
                     discussed for crypto.           Modifications that are not
                                                     actually implementable: -2.
  -------- --------- ------------------------------- ----------------------------

Week 9. Backtesting and Risk Analysis

**THE SPINE OF THIS WEEK**

Students assemble everything they have built into a working backtest on
three months of Coincall data. The week is more about engineering
discipline than new theory; the lecture material is necessary but not
the centerpiece.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Backtesting Architecture for Options

The lecture covers the architecture of an event-driven options backtest
and emphasizes the pitfalls. The mentor will list common bugs:
look-ahead bias, unrealistic fill assumptions, expiry handling, contract
roll. Students should leave knowing what to test for, not just what to
build.

*Watch for student reactions at:*

- The fill simulator design. Students will be tempted to assume 100%
  fill at their quoted prices; the mentor will explain why this is
  wrong.

- The contract expiry handling. Options are not perpetual; there are
  discrete events when a series expires.

Lecture 2 --- Risk Metrics and P&L Attribution

Sharpe, drawdown, Calmar, and the like are reviewed quickly. The
substantive content of the lecture is P&L attribution: decomposing daily
P&L into spread, inventory drift, gamma, vega, and hedging streams. This
decomposition is the heart of the milestone deliverable.

*Watch for student reactions at:*

- The attribution sum-to-total check. Students sometimes have
  attribution streams that do not sum to total P&L; this is always a
  bug.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  My backtest P&L is           Bug. Always bug. Common culprits:
  suspiciously high. Bug or    look-ahead in the volatility surface (you
  genuine alpha?               used today\'s surface to quote
                               yesterday\'s snapshot), 100% fill
                               assumption, missing transaction costs,
                               missing funding rate on perpetual hedges.
                               Walk through the data flow one event at a
                               time.

  How do I calibrate the fill  Use a holdout period. Calibrate the fill
  simulator? It seems          model on one month, validate on a
  circular.                    non-overlapping month. The key empirical
                               fact: fill probability is approximately
                               exponential in quote distance from mid,
                               with a parameter that depends on contract
                               liquidity.

  The P&L attribution sums to  Almost certainly: you are computing the
  a different number than the  streams using different state snapshots.
  total P&L. Where\'s the bug? The spread stream uses end-of-trade state;
                               the inventory drift stream should use
                               start-of-period state. Get the timing
                               right and they will sum.

  My Sharpe ratio is 6.0 over  No. Sharpe over a three-month window has
  three months. Is that real?  large estimation error. The deflated
                               Sharpe ratio (Bailey and López de Prado
                               2014) corrects for this; require the
                               student to report a confidence interval
                               from block bootstrap.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Each student presents a one-week regime from their backtest, walks
through the P&L attribution, and answers questions from the cohort. This
is the dress rehearsal for the milestone.

Materials needed:

- Time slot for each student to present (8 students × 10 minutes = 80
  minutes, leaving room for transitions).

- A projector for each presentation.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--5          Set the agenda. Each student gets 8 minutes (5 to present, 3
                for Q&A).

  5--85         Eight presentations, back to back.

  85--90        Wrap-up: what common issues did we see? Refer everyone to
                the milestone rubric.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- If the cohort is smaller, give more time per student. If the cohort is
  larger, do this over two sessions.

- The presentations should expose engineering bugs that students will
  then fix before the milestone. This is the entire purpose of the
  recitation.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        12        Event-driven backtest harness   Non-deterministic results:
                     with deterministic replay       -5. Code that runs but with
                     verified by bitwise-identical   floating-point drift: -2
                     re-run.                         (warn the student).

  2        12        Fill simulator calibrated on    No holdout validation: -5.
                     training period, validated on   Overfitting (training fits
                     holdout.                        great, holdout poor) without
                                                     commentary: -3.

  3        12        Full one-month backtest;        Missing block-bootstrap
                     performance metrics reported    confidence intervals: -3.
                     with appropriate caveats.       Reporting Sharpe without
                                                     context (e.g., compared to a
                                                     baseline): -2.

  4        10        P&L attribution decomposition;  Attribution that does not
                     stacked-area plot of cumulative sum to total P&L: -5 (this
                     attribution.                    is always a bug).
                                                     Aesthetics: not graded, but
                                                     flag bad plots in feedback.

  5        10        Worst-drawdown day forensic     Forensic that does not
                     analysis.                       identify specific positions:
                                                     -4. Forensic that lacks
                                                     counterfactual analysis: -3.
  -------- --------- ------------------------------- ----------------------------

Milestone Week Note

MILESTONE WEEK. Milestone 3 is due at the end of this week. See Part
III, Section 3 for the full evaluation rubric. This is the most
consequential milestone of the program and the basis for the final
report. Code review sessions should run six to eight hours total (in
addition to your usual office hours).

Week 10. Extensions, Final Report, and Presentations

**THE SPINE OF THIS WEEK**

Students choose one extension topic, implement it in a week, and present
the final report. The tutor\'s role shifts from instruction to
mentorship: helping each student scope their extension realistically and
giving feedback on the draft report.

Lecture Emphasis

Below are notes for each of the two lectures. You do not deliver these;
you attend them. Your job is to track where the cohort got lost so you
can address it in recitation.

Lecture 1 --- Extension Topics

The mentor surveys the menu of extension topics, sketches what a
credible week of work looks like for each, and answers questions.
Students choose by end of day. Tutor: pay attention to who picks what;
you will be the first line of consultation as they implement.

*Watch for student reactions at:*

- Students choosing topics that are too ambitious. The mentor will
  guide, but the tutor should reinforce: a clean partial result beats an
  incomplete grand result.

Lecture 2 --- Research Communication

The mentor walks through the structure of a quantitative research paper
using examples. The lecture is short on theory and long on examples;
encourage students to take notes on style.

*Watch for student reactions at:*

- Students from a pure-math background often resist the \"acknowledge
  limitations\" advice. Re-emphasize in feedback: this is industry
  research writing, not a theorem-proof paper.

Common Student Confusions

Confusions you should expect to see in office hours and recitation. The
right-hand column gives suggested handling.

  ---------------------------- ------------------------------------------
  **Confusion**                **How to Handle**

  My extension is not working. Probably not. The week is too short to
  Should I switch?             switch and start over. Identify the
                               smallest version of your extension that
                               does work, write that up as a partial
                               result, and acknowledge the limitations
                               honestly in the report.

  How long should my final     Maximum thirty pages excluding appendices,
  report be?                   but quality beats length. A tight
                               twenty-page report is preferable to a
                               sprawling thirty-page one. Encourage
                               students to write a short report and use
                               the appendix for supporting material.

  Can I use generated text or  Refer to the academic integrity policy in
  LLM assistance in the        Part IV. Short version: use LLMs as a
  report?                      writing tool (grammar, phrasing), not as a
                               content generator. All technical content
                               must be the student\'s own work.

  How long should my           Twenty minutes including questions.
  presentation be?             Practice it once with a tutor before the
                               final session.
  ---------------------------- ------------------------------------------

Recitation Lesson Plan

Goal: Each student delivers a fifteen-minute dry-run presentation. The
cohort provides feedback. The tutor focuses on questions an industry
audience would ask.

Materials needed:

- Projector.

- Stopwatch.

- Feedback rubric (provided in Part III, Section 4) for the cohort to
  fill in for each presenter.

Suggested timing for the ninety-minute session:

  ------------- ------------------------------------------------------------
  **Minutes**   **Activity**

  0--5          Set expectations: this is a dry run, not the final
                presentation. Tutor will be tough.

  5--85         Eight presentations, 10 minutes each (presentation + Q&A).

  85--90        Aggregate feedback: common issues, common strengths.
  ------------- ------------------------------------------------------------

Recitation-leader notes:

- Be tough but constructive. The point of the dry run is to expose
  problems while there is still time to fix them.

- Submit the feedback rubrics to the mentor; they inform the final
  presentation grade.

Problem Set Solutions and Rubric

Solution sketches with point allocations. Tutors are expected to develop
their own complete solutions before grading; the sketches below are
calibration aids, not solutions manuals.

  -------- --------- ------------------------------- ----------------------------
  **\#**   **Pts**   **Key result expected**         **Common errors and partial
                                                     credit**

  1        5         One-page extension proposal     Late submission: -3.
                     submitted by end of day one of  Proposal that does not
                     week 10.                        engage with the realistic
                                                     time budget: -2.

  2        20        Implementation of the chosen    Extension that does not
                     extension on top of milestone   actually run: at most 8
                     infrastructure.                 points for design. Partial
                                                     implementations that are
                                                     honestly reported: scaled
                                                     credit.

  3        15        Quantitative comparison of      Comparison missing baseline:
                     extension against week-9        -5. Cherry-picked metrics:
                     baseline using shared metrics.  -5.

  4        25        Final technical report (max 30  See the report rubric in
                     pp.) following the lecture\'s   Part III, Section 4.
                     structure.                      

  5        15        Final twenty-minute             See the presentation rubric
                     presentation.                   in Part III, Section 4.
  -------- --------- ------------------------------- ----------------------------

Part III. Milestone Evaluation Rubrics

Each milestone is graded out of 100 points. Final grade for the
milestone is the average of two independent evaluations: yours as the
tutor, and the mentor\'s. Significant discrepancies (more than 10
points) trigger a third reviewer.

3.1 Milestone 1 --- Linear-Asset GLFT Engine

Due: end of week 5. Evaluation criteria sum to 100 points.

  ---------------------------- ------------ ------------------------------------
  **Criterion**                **Points**   **Description**

  Correctness of GLFT          30           GLFT quote computation produces
  implementation                            results that match the closed-form
                                            asymptotic formula within numerical
                                            tolerance (1e-6). Verified by
                                            running the engine on a synthetic
                                            problem with known analytical
                                            solution.

  Intensity calibration        20           MLE-based calibration produces a
  quality                                   non-trivial fit with χ²
                                            goodness-of-fit reported. The
                                            student must demonstrate awareness
                                            of the limitations of their fit, not
                                            just produce numbers.

  Backtest reproducibility     15           Running the backtest twice with the
                                            same configuration produces
                                            bitwise-identical results. Tested by
                                            the grader; non-reproducibility is
                                            an automatic -15.

  Backtest performance match   15           P&L within ±50% of the mentor\'s
                                            reference implementation on the same
                                            data window. The 50% tolerance is
                                            generous because of legitimate
                                            implementation choices; outside this
                                            band suggests a bug.

  Latency                      10           GLFT quote computation in under
                                            100µs per update on a single CPU
                                            core. Measured by the grader using a
                                            standardized benchmark script.

  Code quality                 5            Code passes linting, includes type
                                            hints, and has unit tests covering
                                            the core quote computation.
                                            Subjective but not capricious.

  Technical report             5            Report is at most 10 pp., follows
                                            the structure of the GLFT paper, and
                                            acknowledges limitations honestly.
  ---------------------------- ------------ ------------------------------------

Common reasons for partial credit:

- Code runs but uses finite-difference Greeks (which we have not yet
  introduced): -5 from correctness, since the implementation is
  sub-optimal but not wrong.

- Reproducibility fails due to a random seed not being set: -8, with
  explicit feedback on how to fix.

- Report exceeds 10 pages: -2 per additional page, up to -5.

3.2 Milestone 2 --- Fast Pricing and Greeks Library

Due: end of week 7. Evaluation criteria sum to 100 points.

  ---------------------------- ------------ ------------------------------------
  **Criterion**                **Points**   **Description**

  Pricing accuracy             20           Maximum relative error of 1e-4
                                            against the Coincall reference
                                            prices across all contracts in the
                                            BTC surface. Measured by the grader.

  Greek accuracy               15           Finite-difference verification of
                                            all six Greeks (delta, gamma, vega,
                                            theta, vanna, volga) against the
                                            AAD-computed Greeks, with relative
                                            error below 1e-4.

  Latency --- full surface     25           Full Coincall BTC surface (300-500
  revaluation                               contracts) revalues with full Greek
                                            vector in under 5ms on a single CPU
                                            core. Measured by the grader. THIS
                                            IS A HARD GATE: failing this
                                            criterion caps the milestone grade
                                            at 70.

  Latency --- per-option       10           Per-option latency in nanoseconds
  breakdown                                 reported with distribution (mean,
                                            median, p95, p99). Bonus if students
                                            report tail latencies that are
                                            bounded.

  API design                   10           Library exposes a clean Python API.
                                            Importable as a package. Sensible
                                            function signatures. Documentation
                                            strings.

  Unit tests                   10           Tests cover all pricers, all Greeks,
                                            the calibrated surface adapter, and
                                            at least one edge case (e.g.,
                                            extreme moneyness, zero
                                            time-to-expiry).

  Technical note               10           Benchmarking results documented with
                                            latency distributions (histograms,
                                            not just means), and a clear
                                            explanation of optimization choices.
  ---------------------------- ------------ ------------------------------------

Common reasons for partial credit:

- Latency target missed by less than 1ms (i.e., 5--6ms instead of 5ms):
  -10 from the latency criterion but no hard cap. Beyond 6ms: hard cap
  applies.

- Library works in JAX but does not generalize beyond Black--Scholes: -8
  from API design.

- Vanna and volga not implemented (only first-order Greeks): -8 from
  Greek accuracy.

- C++ Enzyme exercise completed: +5 extra credit (capped at 100 total).

3.3 Milestone 3 --- Full Options Market Making Backtest

Due: end of week 9. Evaluation criteria sum to 100 points. This is the
most consequential milestone and the basis for the final report; grade
carefully.

  ---------------------------- ------------ ------------------------------------
  **Criterion**                **Points**   **Description**

  Backtest reproducibility     10           Identical replay produces
                                            bitwise-identical results. As in
                                            milestone 1, non-reproducibility is
                                            an automatic -10.

  P&L attribution correctness  20           Attribution streams (spread,
                                            inventory, gamma, vega, hedging) sum
                                            to total P&L within 1bp tolerance.
                                            Failure here usually indicates a
                                            timing bug in the attribution code.

  Risk metrics                 15           All required metrics (Sharpe, max
                                            drawdown, Calmar) reported with
                                            block-bootstrap confidence
                                            intervals. The CI requirement is
                                            non-negotiable.

  Greek exposure tracking      10           Time series of aggregated Greeks
                                            (delta, gamma, vega) plotted;
                                            exposures remain within configured
                                            position limits.

  Engine quality               15           Multi-Greek market making engine
                                            correctly integrates the calibrated
                                            volatility surface (milestone 2
                                            library) with the GLFT framework
                                            (milestone 1).

  Hedging integration          10           Dynamic hedging policy correctly
                                            integrated; hedging cost accounted
                                            for (including funding rate on
                                            perpetuals).

  Forensic analysis            10           Drawdown forensic identifies
                                            specific positions, the market
                                            environment, and at least one
                                            counterfactual.

  Technical report             10           Report is at most 20 pp., includes
                                            the forensic analysis, and
                                            acknowledges failure modes honestly.
  ---------------------------- ------------ ------------------------------------

Common reasons for partial credit:

- Look-ahead in the volatility surface: -15 from engine quality. Very
  common bug; check carefully.

- 100% fill assumption: -10 from engine quality. Almost as common.

- Funding rate ignored: -5 from hedging integration.

- Sharpe ratio reported without CI: -8 from risk metrics.

3.4 Final Report and Presentation

Final report: 25 points. Final presentation: 15 points. Total of 40
points; combined with the three milestones and the problem sets to
produce the final grade.

Report rubric:

  ---------------------- --------- -------------------------------------------
  **Criterion**          **Pts**   **Description**

  Problem motivation     3         Clearly states what the extension addresses
                                   and why it matters. A reader from industry
                                   should understand the motivation in two
                                   paragraphs.

  Methodology            6         Methodology is technically sound, builds on
                                   the milestone infrastructure, and is
                                   described at the right level of detail
                                   (enough to reproduce; not so much that it
                                   overwhelms).

  Results                6         Empirical results are reported with
                                   appropriate uncertainty quantification.
                                   Plots are clear and labeled.

  Discussion             4         Discussion engages honestly with the
                                   results. Successes are claimed without
                                   overstatement; failures are acknowledged
                                   and analyzed.

  Limitations            3         An explicit limitations section. This is
                                   required, not optional.

  Writing quality        3         Prose is clear and free of obvious errors.
                                   Citations are correct.
  ---------------------- --------- -------------------------------------------

Presentation rubric:

  ---------------------- --------- -------------------------------------------
  **Criterion**          **Pts**   **Description**

  Structure              3         Presentation follows a clear structure:
                                   motivation, methodology, results,
                                   discussion, conclusions. Time is allocated
                                   appropriately.

  Technical depth        4         Technical content is correct and at the
                                   right level for the audience. The presenter
                                   can answer follow-up questions.

  Visual aids            3         Slides are clear, uncluttered, and
                                   well-labeled. No more than one main idea
                                   per slide.

  Delivery               3         Pacing is appropriate; the presenter is
                                   audible; eye contact is maintained.

  Q&A                    2         The presenter handles questions gracefully,
                                   including questions they cannot fully
                                   answer.
  ---------------------- --------- -------------------------------------------

Part IV. Administrative Reference

4.1 Academic Integrity

The program follows the NC State Code of Student Conduct on academic
integrity. Specific guidance for this program:

- Collaboration on problem sets is encouraged but submissions must be
  each student\'s own work. Acceptable: discussing the approach.
  Unacceptable: copying code or derivations.

- Citation is required for any external source used in a problem set or
  report. \"External\" includes papers, textbooks, blog posts, and
  LLM-generated content.

- Use of LLM assistance is allowed for writing support (grammar,
  phrasing) but not for technical content generation. Students should
  disclose in the report any non-trivial LLM use.

- The mentor handles all academic integrity cases. If you suspect a
  violation, document it (specific evidence, dates) and escalate to the
  mentor within twenty-four hours. Do not confront the student yourself.

4.2 Late Work

Late submission policy for problem sets:

- Submissions are due Sunday at 11:59pm Eastern time.

- Late submissions are accepted until Tuesday 11:59pm Eastern with a 20%
  deduction.

- Submissions later than Tuesday are not accepted; the student receives
  zero for that problem set.

- Exceptions for documented medical or family emergencies are handled by
  the mentor, not the tutor. Direct the student to the mentor.

Late submission policy for milestone deliverables:

- Milestones are due Friday at 11:59pm Eastern time of the milestone
  week.

- Late milestones are not accepted. The student receives zero for that
  milestone.

- Exceptions are again handled by the mentor only.

4.3 Accommodations

Students with documented accommodations (additional time, alternative
formats, etc.) should have their accommodations on file with the NC
State Disability Resource Office. Tutors implement accommodations as
documented; do not ask the student to justify them. If you are uncertain
how to implement a specific accommodation, ask the mentor.

4.4 Crisis Escalation

Situations to escalate to the mentor immediately:

- Suspected academic integrity violation.

- Student in apparent acute distress (mental health, family emergency,
  etc.).

- Data security incident (e.g., student inadvertently exposed Coincall
  data on a public repository).

- Hostile interaction between students or between you and a student.

Use the emergency phone line for these; do not wait on Slack. The mentor
will direct next steps. Do not attempt to resolve these yourself.

4.5 Office Setup and Logistics

Each tutor is provided with:

- Access to the shared Slack workspace.

- Access to the NC State LMS for the program (for problem set submission
  and grade entry).

- Access to the Coincall data S3 endpoint (under the same NDA as
  students, plus additional credentials for the reference
  implementations).

- A laptop with the standard program environment pre-installed: Python
  3.11, JAX, NumPy, SciPy, Pandas, PyArrow, QuantLib, and the program\'s
  own internal libraries.

- A desk in the shared tutor office in SAS Hall (key issued at
  orientation).

Setup tasks for the first week:

1.  Complete the data use agreement with the program coordinator.

2.  Verify your Slack and LMS access.

3.  Run the reference Milestone 1 implementation end-to-end to confirm
    your environment is set up correctly.

4.  Attend the tutor calibration session.

4.6 Compensation and Hours

Tutors are compensated as standard graduate teaching assistants under
the NC State pay scale for the Department of Mathematics. Hours and
compensation are tracked through the standard university time-reporting
system.

4.7 Contact List

Maintained separately as a one-page reference distributed at
orientation. Includes: program mentor, program coordinator, departmental
administrator, IT support, and emergency contacts. Keep accessible
during the program.
