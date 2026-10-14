# Notes on the solutions

Stochastic Processes (1060429), Technion, Spring 2026. Nawar Sgier, 326586047.

| Sheet | Solutions |
|---|---|
| `Exercise01_2026.pdf` (Exercise 1) | `Exercise01_2026_solutions.tex` / `.pdf` |
| `Exercise02_2026.pdf` (Exercise 2) | `Exercise02_2026_solutions.tex` / `.pdf` |
| `Exercise03_2026.pdf` (titled "Exercise 4" on the sheet) | `Exercise03_2026_solutions.tex` / `.pdf` |

`solutions.tex` / `solutions.pdf` hold all three sheets in one document. "Not for submission" sections are skipped.

## References
The Moodle lecture notes were not available, so the proofs use the standard course tools listed in the syllabus: Doob's theorems for discrete-time martingales (optional stopping, the upcrossing inequality), the reflection principle, Itô's isometry and Itô's formula.

## Problems in the questions (flagged in the PDFs as well)
**Exercise 1**
- BM Q1: the condition should hold for all t, s ∈ [0,T]. In (c) the bound is 2^{-γn}, not 2^{-m}. In (e)–(f) the index set is [0,1].

**Exercise 2**
- Cond. exp. Q4: Y must be allowed to take the value +∞. With the trivial σ-algebra and E[X] = ∞ no finite Y works.
- Martingales Q2: the index "t ∈ X" should be "t ∈ T".
- Martingales Q3: (a) should read E|X_{τ₂}| < ∞.
- Martingales Q4(b): X_τ needs a definition on {τ = ∞}. It is taken as lim X_{t∧τ}, which exists by Q5(a).
- Martingales Q5(b): right-continuity must be assumed. A counterexample without it is given.
- Martingales Q6: (a) holds for every σ ∈ ℝ, which (b) needs (derivatives at σ = 0).

**Exercise 4 (file Exercise03)**
- Q1(a)ii and (b)i: the right side should be ⅓B_t³ − ∫B ds, not ⅓B_t².
- Q2: L²_loc is read as E∫₀ᵀ f² < ∞ for every T. Under only ∫f² < ∞ a.s. the claim fails in general.
- Q5: the recursion holds for k ≥ 1 but fails for k = 0 (β₀ = 1).
- Q6: g_ε is C¹ but not C², so Itô's formula is justified by an approximation argument.
- Q7: T_x should be inf{t : X_t^x = 0} with x > 0. In (b) the claim is Y =ᵈ X¹. All X^x are driven by the same B.

## Facts used from outside the course
- Ex 1, Relations Q2(b): the subsets of the Cantor set outnumber the Borel sets (2^𝔠 > 𝔠).
- Ex 4, Q7: B_t/t → 0 a.s.
- Ex 2, Martingales Q4(a): a uniform-integrability lemma for backward supermartingale sequences, proved inside the solution. Your notes may already contain it.

## Parts to read most carefully
- Ex 4, Q7(c)(v)–(vi) on Bessel processes: complete proofs are given, but they are the least standard arguments in the set.
