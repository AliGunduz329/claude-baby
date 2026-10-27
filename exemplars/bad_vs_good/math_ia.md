# Exemplars: Mathematics IA (AA/AI HL) — Criterion C, D & E

## 1. Rationale & Problem Formulation (Criterion C & A)

- **Weak / Flawed (Example 47 — 13/20):**
  > "My investigation was inspired when I was travelling in the front seat of my parent's car. There are situations when sunlight shines directly into my eyes... Personally, this posed great danger to my mom as she got into an accident when she couldn't see the streetlight color due to sunlight. Since then, one problem was given — whether to use sun visors or tint the front face of the car..."
  - **Why it Fails:** Emotional melodrama substituted for mathematical purpose. The author introduces an arbitrary threshold ("efficient when at least 70% is blocked") without mathematical or physical justification.

- **Strong / Rigorous (Example 48 — 17/20):**
  > "Usually, when violinists play music, they hold the bow frog, slide the bow on one string and rotate the bow about the string at the same time if they need to shift strings. If one traces the bow frog, one can see it gives a curved path... As an amateur violinist, I always find it hard to understand intuitively, so I want to see the effect of bow length on its path in a more concrete way through mathematics. The aim of this investigation is to model the path of the violin bow frog depending on the length of bow section used ($L$)..."
  - **Why it Succeeds:** The personal context directly informs the coordinate setup. The mathematical goal is explicit, bounded ($s \le L \le L_0$), and cleanly decoupled from emotional narrative.

---

## 2. Model Construction vs. Mathematical Mechanics (Criterion B & E)

- **Weak / Flawed (Example 47):**
  > Pulls out heavy multivariable calculus machinery ($\iint r^2 \sin\phi \, d\phi \, d\theta$) to calculate spherical cap surface area, but relies on flawed modeling: treats the flat, rectangular visor as if it stretched across the entire car windshield like a curved dome element. Mathematical notation slips (omitting differentials $d\phi$, unannotated vector steps).
  - **Takeaway:** Advanced mathematics outside the syllabus earns zero credit if the underlying physical geometry is divorced from reality or poorly justified.

- **Strong / Rigorous (Example 48):**
  > Uses syllabus-level parametric equations and basic trigonometry:
  > $$x(t) = \frac{L + 3s}{4}t \cos(2\theta_s - \theta_s t), \quad y(t) = \frac{L + 3s}{4}t \sin(2\theta_s - \theta_s t)$$
  > Follows with explicit definitions of domain ($0 \le t \le 1$), linear speed $v$, and angular velocity $\omega$. Explains piecewise discontinuities at string shifts with a clean $l-t$ graph.
  - **Takeaway:** Elegant application of syllabus mathematics with sound logic, clear domain boundaries, and explicit parameter definitions consistently outperforms misunderstood out-of-syllabus calculus.

---

## 3. Reflection, Limitations & Model Testing (Criterion D)

- **Weak / Flawed (Example 47 — Criterion D: 1/3):**
  > "The method used to determine the efficiency of sun visors can be said to be accurate to some extent. The limitations of my result includes the facts that there are certain assumptions... Other minor limitations could have been that when measuring the real values... the measuring tape had an uncertainty of $\pm 0.5\text{ cm}$... Also, when I was measuring the values, there would have been human errors involved."
  - **Why it Fails:**
git add exemplars/bad_vs_good/math_ia.md
git commit -m "feat: add Math IA 4 vs 7 bad-vs-good exemplar analysis"
git push
cat << 'EOF' > system_prompts/academic_writer.md
# Academic & Technical Paper Writer

You are an academic researcher and mathematical author. Your goal is to draft formal investigations, internal assessments, and technical papers with mathematical rigor, economy of language, and clear logic.

## Structural & Voice Directives

1. **Introduction & Rationale (Criterion A & C):**
   - Anchor the personal engagement strictly in physical, geometric, or algorithmic mechanics.
   - Ban melodramatic storytelling, emotional stakes, or moral justifications.
   - Define the explicit aim, parameter boundaries, and constraints in the opening section.

2. **Mathematical Formulation (Criterion B & E):**
   - Use standard LaTeX notation ($inline$ and $$display$$).
   - Define every variable immediately after its introduction.
   - Explicitly justify all assumptions (e.g., planar reduction, symmetry, boundary limits) based on physical or mathematical properties.
   - Never skip derivation steps without stating the mathematical axiom or rule used.
   - Prefer elegant syllabus-appropriate models over superficial, advanced mathematical tools that do not fit the underlying geometry.

3. **In-Line Reflection & Critical Evaluation (Criterion D):**
   - Embed reflection directly after each mathematical decision: explain why a specific function, coordinate system, or regression was chosen over an alternative.
   - Analyze error and fit using quantitative metrics (residuals, percentage deviation, goodness-of-fit) rather than qualitative impressions.
   - Never use cliché evaluation boilerplate ("human error", "measuring tape inaccuracies"). Discuss structural model limitations, edge cases, and domain discontinuities.

4. **Tone & Word Economy:**
   - Write in direct, formal prose.
   - Eliminate filler adverbs (*arguably, truly, intricately, essentially*).
   - Use diagrams and tables to carry structural descriptions rather than long descriptive paragraphs.
