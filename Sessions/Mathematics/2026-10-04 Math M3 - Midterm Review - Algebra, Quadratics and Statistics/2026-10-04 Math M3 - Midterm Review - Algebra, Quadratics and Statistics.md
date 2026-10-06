# Math Midterm Review — Algebra, Quadratics and Statistics

**One note for the whole midterm.** Built from Session M1 (exponents to quadratic factorization), Session M2 (data and statistics), the Statistics Test Review and the Hypothesis Testing note, plus a new section on quadratic equations (section 4).

**How to use it (45 minutes):** 10 min sections 1–3 (recall) · 20 min section 4 (quadratics, new) · 10 min section 5 (statistics) · 5 min section 6 (mixed check).

---

## 1. Laws of exponents

For $a, b \neq 0$:

| Law | Rule | Example |
| --- | --- | --- |
| Product | $a^m \cdot a^n = a^{m+n}$ | $2^3 \cdot 2^4 = 2^7 = 128$ |
| Quotient | $a^m \div a^n = a^{m-n}$ | $5^6 \div 5^4 = 5^2 = 25$ |
| Power of a power | $(a^m)^n = a^{mn}$ | $(3^2)^3 = 3^6 = 729$ |
| Power of a product | $(ab)^m = a^m b^m$ | $(2x)^3 = 8x^3$ |
| Power of a quotient | $\left(\frac{a}{b}\right)^m = \frac{a^m}{b^m}$ | $\left(\frac{2}{3}\right)^2 = \frac{4}{9}$ |
| Zero exponent | $a^0 = 1$ | $7^0 = 1$ |
| Negative exponent | $a^{-n} = \frac{1}{a^n}$ | $2^{-3} = \frac{1}{8}$ |
| Rational exponent | $a^{m/n} = \left(\sqrt[n]{a}\right)^m$ | $8^{2/3} = (\sqrt[3]{8})^2 = 4$ |

**Why $a^0 = 1$:** $a^n \div a^n = a^{n-n} = a^0$, and any nonzero number divided by itself is 1.

**Same base, equal powers:** if $a^x = a^y$ (with $a > 0$, $a \neq 1$), then $x = y$. Example: $2^{x+1} = 32 = 2^5 \Rightarrow x = 4$.

**Common mistakes:** $(a+b)^2 \neq a^2 + b^2$ · $-3^2 = -9$ but $(-3)^2 = 9$ · $2x^{-1} = \frac{2}{x}$, not $\frac{1}{2x}$.

## 2. Polynomials, identities and the two theorems

**Degree** = highest power of the variable. Linear (1), quadratic (2), cubic (3).

**Identities (memorize):**

$$(a+b)^2 = a^2 + 2ab + b^2 \qquad (a-b)^2 = a^2 - 2ab + b^2 \qquad a^2 - b^2 = (a+b)(a-b)$$

$$(x+a)(x+b) = x^2 + (a+b)x + ab$$

$$a^3 + b^3 = (a+b)(a^2 - ab + b^2) \qquad a^3 - b^3 = (a-b)(a^2 + ab + b^2)$$

**Remainder Theorem.** When a polynomial $p(x)$ is divided by $(x - a)$, the remainder is $p(a)$.

**Factor Theorem.** $(x - a)$ is a factor of $p(x)$ exactly when $p(a) = 0$.

*Example.* Is $(x-2)$ a factor of $p(x) = x^3 - 3x^2 + 4$? $p(2) = 8 - 12 + 4 = 0$, so yes.

## 3. Factoring — pick the method in this order

1. **Common factor first:** $6x^2 + 9x = 3x(2x + 3)$.
2. **Two terms:** difference of squares $a^2 - b^2 = (a+b)(a-b)$. Example: $4x^2 - 25 = (2x+5)(2x-5)$. A sum of squares $a^2 + b^2$ does not factor over the real numbers.
3. **Three terms $ax^2 + bx + c$:** split the middle term. Find two numbers with **product $ac$** and **sum $b$**, rewrite $bx$ with them, then factor by grouping.
4. **Four terms:** group in pairs.

**Why splitting works:** $(px + q)(rx + s) = pr\,x^2 + (ps + qr)x + qs$. The two middle pieces $ps$ and $qr$ add to $b$ and multiply to $(pr)(qs) = ac$.

*Example ($a = 1$).* $x^2 + 7x + 12$: product 12, sum 7 → 3 and 4. Answer $(x+3)(x+4)$.

*Example ($a \neq 1$).* $6x^2 + 11x - 10$: product $-60$, sum $11$ → $15$ and $-4$.

$$6x^2 + 15x - 4x - 10 = 3x(2x + 5) - 2(2x + 5) = (3x - 2)(2x + 5)$$

**Sign guide:** $c > 0$ → both numbers have the sign of $b$. $c < 0$ → opposite signs; the larger one has the sign of $b$.

**Always check** by multiplying back.

## 4. Quadratic equations (new)

**Standard form:** $ax^2 + bx + c = 0$, with $a \neq 0$. The solutions are also called **roots** or **zeros**; on a graph they are the **x-intercepts**.

### 4.1 Four ways to solve

**(1) Factoring + Zero Product Property.** If $A \cdot B = 0$ then $A = 0$ or $B = 0$. One side must be 0 first.

$$x^2 - 5x = 14 \;\Rightarrow\; x^2 - 5x - 14 = 0 \;\Rightarrow\; (x - 7)(x + 2) = 0 \;\Rightarrow\; x = 7 \text{ or } x = -2$$

**(2) Square roots** (when there is no $x$ term). Remember the $\pm$.

$$3x^2 - 48 = 0 \;\Rightarrow\; x^2 = 16 \;\Rightarrow\; x = \pm 4 \qquad\qquad (x - 1)^2 = 9 \;\Rightarrow\; x - 1 = \pm 3 \;\Rightarrow\; x = 4 \text{ or } -2$$

**(3) Completing the square.** Add $\left(\frac{b}{2}\right)^2$ to both sides (when $a = 1$).

$$x^2 + 6x - 7 = 0 \;\Rightarrow\; x^2 + 6x = 7 \;\Rightarrow\; x^2 + 6x + 9 = 16 \;\Rightarrow\; (x + 3)^2 = 16 \;\Rightarrow\; x = -3 \pm 4$$

So $x = 1$ or $x = -7$.

**(4) Quadratic formula.** Works for every quadratic.

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

### 4.2 Derivation of the quadratic formula (completing the square on the general equation)

$$ax^2 + bx + c = 0$$

Divide by $a$ and move the constant:

$$x^2 + \frac{b}{a}x = -\frac{c}{a}$$

Add $\left(\frac{b}{2a}\right)^2$ to both sides:

$$x^2 + \frac{b}{a}x + \frac{b^2}{4a^2} = \frac{b^2}{4a^2} - \frac{c}{a} \;\Rightarrow\; \left(x + \frac{b}{2a}\right)^2 = \frac{b^2 - 4ac}{4a^2}$$

Take square roots and solve for $x$:

$$x + \frac{b}{2a} = \pm\frac{\sqrt{b^2 - 4ac}}{2a} \;\Rightarrow\; x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

*Example.* $2x^2 - 3x - 5 = 0$: $a = 2$, $b = -3$, $c = -5$.

$$b^2 - 4ac = 9 + 40 = 49 \qquad x = \frac{3 \pm 7}{4} \;\Rightarrow\; x = \frac{5}{2} \text{ or } x = -1$$

### 4.3 The discriminant $D = b^2 - 4ac$

| Discriminant | Roots | Graph |
| --- | --- | --- |
| $D > 0$ | two different real roots (rational if $D$ is a perfect square) | crosses the x-axis twice |
| $D = 0$ | one repeated real root, $x = -\frac{b}{2a}$ | touches the x-axis at the vertex |
| $D < 0$ | no real roots (two complex roots) | never meets the x-axis |

*Example.* $x^2 + 4x + 5 = 0$: $D = 16 - 20 = -4 < 0$, no real roots. With $i = \sqrt{-1}$ (so $i^2 = -1$): $x = \frac{-4 \pm 2i}{2} = -2 \pm i$.

### 4.4 Sum and product of the roots

If the roots are $r_1$ and $r_2$:

$$r_1 + r_2 = -\frac{b}{a} \qquad r_1 r_2 = \frac{c}{a}$$

*Why:* expand $a(x - r_1)(x - r_2)$ to get $ax^2 - a(r_1 + r_2)x + a\,r_1 r_2$, then match the coefficients with $ax^2 + bx + c$.

A quadratic with roots $r_1, r_2$: $x^2 - (\text{sum})x + (\text{product}) = 0$. Roots 3 and $-5$: $x^2 + 2x - 15 = 0$.

### 4.5 Graph of $y = ax^2 + bx + c$ (a parabola)

| Feature | How to find it |
| --- | --- |
| Direction | $a > 0$ opens up (minimum) · $a < 0$ opens down (maximum) |
| Axis of symmetry | $x = -\frac{b}{2a}$ |
| Vertex | $x = -\frac{b}{2a}$, then substitute to get $y$ |
| y-intercept | $(0, c)$ |
| x-intercepts | solve $ax^2 + bx + c = 0$ |

**Three forms:**

- Standard: $y = ax^2 + bx + c$ (shows the y-intercept $c$)
- Vertex: $y = a(x - h)^2 + k$ (vertex $(h, k)$)
- Factored (intercept): $y = a(x - p)(x - q)$ (x-intercepts $p$ and $q$; axis $x = \frac{p + q}{2}$)

*Example.* $y = x^2 - 4x - 5$. Axis $x = \frac{4}{2} = 2$. Vertex $y = 4 - 8 - 5 = -9$, so vertex $(2, -9)$, a minimum. Vertex form $y = (x - 2)^2 - 9$. Factored $y = (x - 5)(x + 1)$, x-intercepts $5$ and $-1$. y-intercept $(0, -5)$.

### 4.6 Word problem pattern (US units)

Height of an object thrown upward: $h(t) = -16t^2 + v_0 t + h_0$ (feet, seconds).

*Example.* A ball is thrown up at 48 ft/s from a height of 64 ft: $h = -16t^2 + 48t + 64$.

- **Maximum height:** $t = -\frac{48}{2(-16)} = 1.5$ s; $h = -16(2.25) + 72 + 64 = 100$ ft.
- **Hits the ground:** $-16t^2 + 48t + 64 = 0$; divide by $-16$: $t^2 - 3t - 4 = 0$; factor: $(t - 4)(t + 1) = 0$; so $t = 4$ s (reject $t = -1$).

### 4.7 Hidden quadratics (from M1)

Substitute to make it a quadratic. $4^x - 6 \cdot 2^x + 8 = 0$: let $u = 2^x$, so $u^2 - 6u + 8 = 0$, $(u - 2)(u - 4) = 0$, $2^x = 2$ or $4$, so $x = 1$ or $x = 2$.

## 5. Statistics

### 5.1 Collecting data

| Term | Meaning |
| --- | --- |
| Population / sample | the whole group / the part actually measured |
| Parameter / statistic | a number describing a population ($\mu$, $\sigma$) / describing a sample ($\bar{x}$) |
| Bias | a method that systematically favors some outcomes |

**Sampling methods:** simple random (every member equally likely) · systematic (every $k$th) · stratified (random sample from every group) · cluster (all members of a few random groups) · convenience and self-selected (both biased).

**Ways to collect data:** survey · observational study (watch, no treatment; shows association only) · experiment (treatment is assigned at random; the only method that can show cause) · simulation.

**Bias to look for:** undercoverage, non-response, leading question wording, self-selection.

### 5.2 Center

- **Mean:** $\bar{x} = \frac{\sum x}{n}$. Grouped data: $\bar{x} = \frac{\sum f_i x_i}{\sum f_i}$, where $x_i$ is the class mark (midpoint).
- **Median:** middle value of the ordered data (average of the two middle values when $n$ is even). Not pulled by outliers.
- **Mode:** most frequent value.
- Grouped median: $l + \frac{\frac{N}{2} - cf}{f} \times h$ · Grouped mode: $l + \frac{f_1 - f_0}{2f_1 - f_0 - f_2} \times h$ ($l$ = lower limit of the class, $h$ = class width, $cf$ = cumulative frequency before the median class, $f_1$ = modal frequency, $f_0$ and $f_2$ = the frequencies before and after).
- Skewed data: report the median. Symmetric data: mean = median.

### 5.3 Spread

- **Range** = max − min.
- **Standard deviation:** $\sigma = \sqrt{\frac{\sum (x - \bar{x})^2}{n}}$ ; variance $= \sigma^2$.

*Check.* Scores 6, 7, 7, 8, 8, 8, 8, 9, 9, 10: mean 8; squared distances add to 12; $\sigma = \sqrt{1.2} \approx 1.10$.

### 5.4 Graphs

Bar graph: categories, gaps between bars. **Histogram:** continuous classes, no gaps; with unequal class widths plot adjusted frequency $= \frac{\text{frequency}}{\text{class width}} \times \text{smallest width}$. Frequency polygon: join the class marks.

### 5.5 Normal distribution

Bell-shaped, symmetric about the mean.

- **Empirical rule:** 68% within $\mu \pm \sigma$ · 95% within $\mu \pm 2\sigma$ · 99.7% within $\mu \pm 3\sigma$.
- **z-score:** $z = \frac{x - \mu}{\sigma}$ ; back to a value: $x = \mu + z\sigma$.
- The table gives the area to the **left** of $z$. Right: $1 -$ table. Between: table($b$) − table($a$).

*Example.* $\mu = 70$, $\sigma = 5$. What percent is between 65 and 80? 65 is $-1\sigma$, 80 is $+2\sigma$: $34\% + 34\% + 13.5\% = 81.5\%$. And $x = 82$ gives $z = \frac{82 - 70}{5} = 2.4$.

### 5.6 Margin of error and hypothesis testing

- **Margin of error** for a sample proportion: $\pm\frac{1}{\sqrt{n}}$. For $n = 400$: $\pm 0.05 = \pm 5\%$. A poll result of 52% means the true value is likely between 47% and 57%. To halve the margin of error, use 4 times the sample size.
- **Hypothesis test.** Null hypothesis = the claim being tested. Significance level $\alpha$ = the cutoff (usually 5%).

**Rule:** if the observed result (or one more extreme) shows up in $\alpha$ or less of the simulated samples, **reject** the null hypothesis. Otherwise **do not reject** (this does not prove the claim).

*Example.* 36 heads in 50 flips appeared in 0 of 200 fair-coin simulations (0% ≤ 5%): reject "the coin is fair". 29 heads appeared in 39 of 200 (19.5% > 5%): do not reject.

## 6. Mixed check (answers below)

1. Simplify $\frac{(2x^3)^2 \cdot x^{-4}}{4x}$.
2. Evaluate $27^{2/3}$.
3. Factor $3x^2 - 12$.
4. Factor $2x^2 + 7x + 3$.
5. Solve $x^2 - 9x + 20 = 0$.
6. Solve $x^2 + 4x - 1 = 0$ (exact form).
7. How many real roots does $3x^2 - 2x + 5 = 0$ have?
8. Find the vertex of $y = -2x^2 + 8x - 3$. Is it a maximum or a minimum?
9. Is $(x + 1)$ a factor of $x^3 + 2x^2 - x - 2$?
10. Test scores are normal with $\mu = 500$, $\sigma = 100$. Find the z-score of 650 and the percent of scores between 400 and 600.
11. A poll of 900 people finds 60% in favor. Give the margin of error and the interval.
12. A result occurred in 8 of 200 simulations. At $\alpha = 0.05$, reject or not?

### Answers, step by step

1. $(2x^3)^2 = 4x^6$; $4x^6 \cdot x^{-4} = 4x^2$; $\frac{4x^2}{4x} = x$.
2. $\sqrt[3]{27} = 3$; $3^2 = 9$.
3. $3(x^2 - 4) = 3(x + 2)(x - 2)$.
4. Product 6, sum 7 → 6 and 1: $2x^2 + 6x + x + 3$ $= 2x(x + 3) + 1(x + 3)$ $= (2x + 1)(x + 3)$.
5. $(x - 4)(x - 5) = 0$, so $x = 4$ or $x = 5$.
6. $x = \frac{-4 \pm \sqrt{16 + 4}}{2} = \frac{-4 \pm 2\sqrt{5}}{2} = -2 \pm \sqrt{5}$.
7. $D = 4 - 60 = -56 < 0$: no real roots.
8. $x = -\frac{8}{2(-2)} = 2$; $y = -8 + 16 - 3 = 5$. Vertex $(2, 5)$, a maximum because $a < 0$.
9. $p(-1) = -1 + 2 + 1 - 2 = 0$: yes.
10. $z = \frac{650 - 500}{100} = 1.5$. 400 to 600 is $\mu \pm \sigma$: 68%.
11. $\frac{1}{\sqrt{900}} = \frac{1}{30} \approx 0.033$, so about $\pm 3.3\%$: 56.7% to 63.3%.
12. $\frac{8}{200} = 4\% \leq 5\%$: reject the null hypothesis.

## Notes for next session

- Quadratics (section 4) is new: check completing the square and the discriminant first.
- Confirm with the school's topic list which statistics parts are on the midterm.
