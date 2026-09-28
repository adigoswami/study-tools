# Session M1 — From Exponents to Factoring Quadratics (Grade 9 Foundation)

**Subject:** Mathematics
**Duration:** ~75 minutes (flexible 60–90 min)
**Student:** Grade 9, concurrently taking an accelerated Grade 11 Math course
**Topic:** Quadratic equations — building the Grade-9 foundation (exponents → polynomial factorization → factoring & solving quadratics)

**Source material used tonight:** R.D. Sharma *Mathematics – IX*, Chapter 2 "Exponents of Real Numbers" and Chapter 6 "Factorization of Polynomials" (the two excerpts provided).

**Grade-10 / Grade-11 material:** Not yet provided. This session deliberately stops at the *factorization method* for solving quadratic equations. Completing the square, the quadratic formula (and its derivation), the discriminant/nature of roots, and any Grade-11-level extensions (complex roots, sum & product of roots, forming equations from roots) belong in the **next** session once the Grade-10 and Grade-11 PDFs are available — see "Notes for Next Session" at the end.

**Why this scope, tonight:** The school's accelerated course has reached quadratic equations. Before he can follow that at grade-11 depth, he needs to be completely fluent in two grade-9 building blocks: (1) the laws of exponents (so algebraic manipulation doesn't slow him down), and (2) factoring a quadratic trinomial by splitting the middle term (the method almost every "solve the quadratic" problem starts with). This session builds both, then fuses them into "solve a quadratic equation by factorization."

---

## Lesson Plan

| Segment | Time | Focus |
|---|---|---|
| Warm-up | 10 min | Recall laws of exponents; hook problem that hides a quadratic equation inside an exponential equation |
| Concept Notes — Part A | 10 min | Polynomials refresher: definition, degree, zero/root of a polynomial |
| Concept Notes — Part B | 10 min | Remainder Theorem and Factor Theorem (statement + proof of each) |
| Concept Notes — Part C | 15 min | Splitting the middle term — full derivation of *why* the method works |
| Concept Notes — Part D | 5 min | Zero Product Property; definition of a quadratic equation; solving by factorization |
| Worked Examples | 10 min | 3 fully solved examples, increasing in difficulty |
| Practice Problems | 15 min (in-class) / homework | 13 problems across 4 tiers |
| Wrap-up | 5 min | Answer key walkthrough, preview of next session |

**Learning objectives — by the end of this session the student will be able to:**

1. State and correctly apply all the laws of exponents.
2. State the Remainder Theorem and Factor Theorem, and explain *why* each is true (not just recite it).
3. Factor any quadratic trinomial $ax^2+bx+c$ by splitting the middle term, and explain why the method works.
4. Solve a quadratic equation $ax^2+bx+c=0$ by factorization, using the Zero Product Property.
5. Recognize and solve an exponential equation that is secretly a quadratic equation in disguise (via substitution).

---

## Warm-up (10 min)

### Quick recall: Laws of Exponents

Before we start, run through these out loud — for each one, be ready to say *why* it's true, not just what it says (we derive all of them in the notes below):

$$a^m \times a^n = a^{m+n} \qquad a^m \div a^n = a^{m-n} \qquad (a^m)^n = a^{mn}$$
$$(ab)^m = a^m b^m \qquad \left(\frac{a}{b}\right)^m = \frac{a^m}{b^m} \qquad a^0 = 1 \qquad a^{-n} = \frac{1}{a^n}$$

**Quick fire (answer out loud, 2 min):**

- $2^3 \times 2^4 = ?$ → $2^7 = 128$
- $5^0 = ?$ → $1$
- $3^{-2} = ?$ → $\dfrac{1}{9}$

### Hook problem

Solve for $x$: $\quad 2^{2x+1} = 17\cdot 2^x - 8$

This doesn't look like anything we've solved before — there's an $x$ in the exponent *and* the equation isn't linear. Watch what happens if we let $y = 2^x$:

$$2\cdot(2^x)^2 = 17\cdot 2^x - 8 \;\;\Longrightarrow\;\; 2y^2 - 17y + 8 = 0$$

That's a **quadratic equation** in $y$. We don't yet have a general, reliable way to solve *any* quadratic equation — that's exactly what tonight builds. We'll come back and finish this exact problem in Worked Example 3.

---

## Concept Notes

### Part A — Polynomials Refresher (10 min)

> **Definition (Polynomial).** An algebraic expression of the form
> $$f(x) = a_nx^n + a_{n-1}x^{n-1} + \cdots + a_1x + a_0$$
> where $n$ is a non-negative integer and the coefficients $a_n, a_{n-1}, \dots, a_0$ are real numbers with $a_n \neq 0$, is called a **polynomial in $x$ of degree $n$**.

Degree names you'll see constantly: degree 1 → *linear*, degree 2 → *quadratic*, degree 3 → *cubic*, degree 4 → *biquadratic (quartic)*.

> **Definition (Quadratic polynomial).** A polynomial of degree 2: $\;ax^2+bx+c$, where $a,b,c$ are real numbers and $a \neq 0$.
> (Why $a\neq 0$? If $a=0$ the $x^2$ term vanishes and it's just a linear expression $bx+c$ — not degree 2 anymore.)

> **Definition (Zero / Root of a polynomial).** A real number $k$ is called a **zero** (or **root**) of a polynomial $f(x)$ if $f(k) = 0$.

This is the idea we'll use constantly tonight: "finding where a polynomial equals zero" and "finding its factors" turn out to be the same question — that's exactly what the next two theorems formalize.

### Part B — Remainder Theorem & Factor Theorem (10 min)

> **Remainder Theorem.** If a polynomial $f(x)$ is divided by a linear polynomial $(x-a)$, the remainder is $f(a)$.
>
> Mathematically: $\;f(x) = (x-a)\cdot q(x) + f(a)$, for some polynomial $q(x)$ (the quotient).

**Derivation (why this is true):** When you divide any polynomial $f(x)$ by a linear divisor $(x-a)$, the division algorithm guarantees
$$f(x) = (x-a)\cdot q(x) + r$$
where $r$ is the remainder. Since the divisor $(x-a)$ has degree 1, the remainder must have degree *less than* 1 — i.e., $r$ is just a constant number (not an expression in $x$).

Now substitute $x = a$ into both sides:
$$f(a) = (a-a)\cdot q(a) + r = 0\cdot q(a) + r = r$$

So $r = f(a)$. That's the whole proof — the remainder is literally just "plug $a$ into $f$." $\blacksquare$

> **Factor Theorem.** $(x-a)$ is a factor of a polynomial $f(x)$ **if and only if** $f(a) = 0$.

**Derivation (this follows directly from the Remainder Theorem):**

- ($\Leftarrow$) Suppose $f(a) = 0$. From the Remainder Theorem, $f(x) = (x-a)q(x) + f(a) = (x-a)q(x) + 0 = (x-a)q(x)$. Since $f(x)$ divides evenly by $(x-a)$ with nothing left over, $(x-a)$ is a factor of $f(x)$.
- ($\Rightarrow$) Suppose $(x-a)$ is a factor of $f(x)$. Then $f(x) = (x-a)q(x)$ for some $q(x)$. Substituting $x=a$: $f(a) = (a-a)q(a) = 0$.

Both directions hold, so it's an "if and only if." $\blacksquare$

**Quick example:** Is $(x-2)$ a factor of $f(x) = x^3 - 6x^2 + 11x - 6$?
$f(2) = 8 - 24 + 22 - 6 = 0$ → yes, by the Factor Theorem, $(x-2)$ is a factor.

### Part C — Splitting the Middle Term: the full derivation (15 min)

This is the core technique tonight, and the standing rule in this course is: never memorize a method without knowing why it works. So here's where "find two numbers whose sum is $b$ and product is $ac$" actually comes from.

**Goal:** factor a quadratic trinomial $ax^2+bx+c$ (with $a,b,c$ real, $a\neq 0$) into two linear factors $(px+q)(rx+s)$.

**Derivation:**

Step 1 — Expand the general product of two linear factors:
$$(px+q)(rx+s) = prx^2 + (ps+qr)x + qs$$

Step 2 — Match coefficients with $ax^2+bx+c$:
$$pr = a \qquad qs = c \qquad ps+qr = b$$

Step 3 — Here's the key trick. Let $m = ps$ and $n = qr$, so that $m+n = b$ (matches the middle coefficient, by the third equation above). Now look at the *product* $m \cdot n$:
$$m \cdot n = (ps)(qr) = (pr)(qs) = a \cdot c$$

So $m$ and $n$ are two numbers whose **sum is $b$** and whose **product is $ac$**. That's exactly the rule — and now you can see it isn't an arbitrary trick, it falls straight out of matching coefficients.

Step 4 — Once such $m, n$ are found, rewrite the middle term $bx$ as $mx + nx$:
$$ax^2 + bx + c = ax^2 + mx + nx + c$$

Step 5 — Factor by grouping: pull the common factor out of the first pair of terms, and out of the second pair, and you'll always be left with the *same* binomial factor in both — that's what lets you finish the factoring.

**Worked derivation example:** Factor $6x^2+7x-3$.

- $a=6, b=7, c=-3 \Rightarrow ac = -18$.
- Need two numbers with sum $7$ and product $-18$: try $9$ and $-2$ ($9\times(-2)=-18$, $9+(-2)=7$). ✓
- Split: $6x^2 + 9x - 2x - 3$
- Group: $3x(2x+3) - 1(2x+3)$
- Common factor: $(2x+3)(3x-1)$

Check by expanding: $(2x+3)(3x-1) = 6x^2 - 2x + 9x - 3 = 6x^2+7x-3$ ✓.

**This is exactly the technique the textbook uses to finish factoring higher-degree polynomials too** — e.g. after using the Factor Theorem to strip a linear factor off a cubic like $2x^3-3x^2-17x+30$, you're left with a quadratic quotient ($2x^2+x-15$), and splitting the middle term finishes the job. We'll solve that exact quotient as an equation in Worked Example 2.

### Part D — Zero Product Property & Solving Quadratic Equations (5 min)

> **Zero Product Property.** For real numbers $p$ and $q$: if $p \cdot q = 0$, then $p = 0$ or $q = 0$ (or both).
>
> Mathematically: $\;pq = 0 \iff p=0 \;\lor\; q=0$

**Reasoning:** Suppose $p \neq 0$. Then we're allowed to divide both sides of $pq=0$ by $p$: $q = \dfrac{0}{p} = 0$. So if $p$ isn't zero, $q$ is forced to be zero — meaning at least one of the two factors must be zero. This is the property that lets us turn a *factored* equation into two simple linear equations.

> **Definition (Quadratic equation).** An equation of the form $ax^2+bx+c=0$, where $a,b,c$ are real numbers and $a \neq 0$.

**Solving by factorization — putting it all together:**

1. Factor $ax^2+bx+c$ into $(px+q)(rx+s)$ by splitting the middle term (Part C).
2. Set the factored equation to zero: $(px+q)(rx+s) = 0$.
3. Apply the Zero Product Property: $px+q=0$ **or** $rx+s=0$.
4. Solve each linear equation: $x = -\dfrac{q}{p}$ or $x = -\dfrac{s}{r}$.

**Note for next session:** factorization only works cleanly when the quadratic splits into nice integer/rational factors. When it doesn't, we need the completing-the-square method and the quadratic formula — that's Grade-10 territory, coming once that material is available.

---

## Worked Examples (10 min)

**Worked Example 1 — Factor a quadratic trinomial**

Factor: $2x^2+5x-3$

$a=2, b=5, c=-3 \Rightarrow ac=-6$. Need two numbers with sum $5$, product $-6$: $6$ and $-1$ ($6\times(-1)=-6$, $6+(-1)=5$). ✓

$2x^2+6x-x-3 = 2x(x+3) - 1(x+3) = (x+3)(2x-1)$

Check: $(x+3)(2x-1) = 2x^2-x+6x-3 = 2x^2+5x-3$ ✓

**Worked Example 2 — Solve a quadratic equation by factorization**

Solve: $2x^2+x-15=0$

*(This is the exact quadratic quotient that appears inside the textbook's Example 1 of §6.5, when factoring $2x^3-3x^2-17x+30$ — now we solve it as an equation in its own right.)*

$a=2,b=1,c=-15 \Rightarrow ac=-30$. Need sum $1$, product $-30$: $6$ and $-5$ ($6\times(-5)=-30$, $6+(-5)=1$). ✓

$2x^2+6x-5x-15 = 2x(x+3) - 5(x+3) = (x+3)(2x-5)$

Set to zero: $(x+3)(2x-5)=0 \Rightarrow x+3=0 \text{ or } 2x-5=0 \Rightarrow x=-3 \text{ or } x=\dfrac{5}{2}$

Check $x=-3$: $2(9)+(-3)-15 = 18-3-15=0$ ✓
Check $x=\frac{5}{2}$: $2\left(\frac{25}{4}\right)+\frac{5}{2}-15 = \frac{25}{2}+\frac{5}{2}-15 = \frac{30}{2}-15 = 15-15=0$ ✓

**Worked Example 3 — Finishing the warm-up hook**

Solve: $2^{2x+1} = 17\cdot 2^x - 8$

Rewrite $2^{2x+1} = 2\cdot(2^x)^2$. Let $y = 2^x$:
$$2y^2 = 17y - 8 \;\Longrightarrow\; 2y^2-17y+8=0$$

$a=2,b=-17,c=8 \Rightarrow ac=16$. Need sum $-17$, product $16$: $-16$ and $-1$ ($-16\times-1=16$, $-16+(-1)=-17$). ✓

$2y^2-16y-y+8 = 2y(y-8)-1(y-8)=(y-8)(2y-1)$

$(y-8)(2y-1)=0 \Rightarrow y=8 \text{ or } y=\dfrac{1}{2}$

Back-substitute $y=2^x$:

- $2^x = 8 = 2^3 \Rightarrow x=3$
- $2^x = \dfrac12 = 2^{-1} \Rightarrow x=-1$

Check $x=3$: LHS $=2^7=128$. RHS $=17(8)-8=136-8=128$ ✓
Check $x=-1$: LHS $=2^{-1}=0.5$. RHS $=17(0.5)-8=8.5-8=0.5$ ✓

$$x = 3 \;\text{ or }\; x=-1$$

---

## Practice Problems

### Tier 1 — Laws of Exponents (warm-up level)

1. Simplify: $\dfrac{2^5 \times 2^{-2}}{2^{-3}}$
2. Solve for $x$: $3^{x+2} = 81$
3. Simplify: $(a^3b^{-2})^2 \times (a^{-1}b)^3$

### Tier 2 — Factor by splitting the middle term

4. Factor: $4x^2-4x-15$
5. Factor: $3x^2-5x-12$
6. Factor: $5x^2+13x-6$

### Tier 3 — Solve quadratic equations by factorization

7. Solve: $x^2-7x+12=0$
8. Solve: $2x^2-x-6=0$
9. Solve: $3x^2+14x-5=0$
10. Solve: $6x^2-x-15=0$

### Tier 4 — Challenge: exponential equations hiding a quadratic

11. Solve for $x$: $2^{2x}-9(2^x)+8=0$
12. Solve for $x$: $3^{2x+1}-10(3^x)+3=0$

### Tier 5 — Apply the Factor Theorem (quick check, ties Part B back in)

13. Without dividing, determine whether $(x-1)$ is a factor of $f(x)=x^3+2x^2-x-2$. If it is, use the Factor Theorem's logic plus splitting the middle term (after dividing out the known factor) to fully factor $f(x)$.

---

## Answer Key — Full Step-by-Step Solutions

**1.** $\dfrac{2^5\times2^{-2}}{2^{-3}} = 2^{5+(-2)-(-3)} = 2^{5-2+3}=2^6=64$

**2.** $3^{x+2}=81=3^4 \Rightarrow x+2=4 \Rightarrow x=2$

**3.** $(a^3b^{-2})^2\times(a^{-1}b)^3 = a^6b^{-4}\times a^{-3}b^3 = a^{6-3}b^{-4+3}=a^3b^{-1}=\dfrac{a^3}{b}$

**4.** Factor $4x^2-4x-15$: $a=4,c=-15\Rightarrow ac=-60$. Need sum $-4$, product $-60$: $6,-10$ ($6\times-10=-60$, $6-10=-4$). ✓
$4x^2+6x-10x-15 = 2x(2x+3)-5(2x+3)=(2x+3)(2x-5)$
Check: $4x^2-10x+6x-15=4x^2-4x-15$ ✓

**5.** Factor $3x^2-5x-12$: $ac=-36$. Need sum $-5$, product $-36$: $4,-9$ ($4\times-9=-36$, $4-9=-5$). ✓
$3x^2+4x-9x-12=x(3x+4)-3(3x+4)=(3x+4)(x-3)$
Check: $3x^2-9x+4x-12=3x^2-5x-12$ ✓

**6.** Factor $5x^2+13x-6$: $ac=-30$. Need sum $13$, product $-30$: $15,-2$ ($15\times-2=-30$, $15-2=13$). ✓
$5x^2+15x-2x-6=5x(x+3)-2(x+3)=(x+3)(5x-2)$
Check: $5x^2-2x+15x-6=5x^2+13x-6$ ✓

**7.** Solve $x^2-7x+12=0$: need sum $-7$, product $12$: $-3,-4$.
$(x-3)(x-4)=0 \Rightarrow x=3 \text{ or } x=4$
Check: $x=3$: $9-21+12=0$ ✓. $x=4$: $16-28+12=0$ ✓

**8.** Solve $2x^2-x-6=0$: $ac=-12$. Need sum $-1$, product $-12$: $3,-4$.
$2x^2+3x-4x-6=x(2x+3)-2(2x+3)=(2x+3)(x-2)$
$(2x+3)(x-2)=0 \Rightarrow x=-\dfrac32 \text{ or } x=2$
Check: $x=2$: $8-2-6=0$ ✓. $x=-\frac32$: $2\left(\frac94\right)+\frac32-6=4.5+1.5-6=0$ ✓

**9.** Solve $3x^2+14x-5=0$: $ac=-15$. Need sum $14$, product $-15$: $15,-1$.
$3x^2+15x-x-5=3x(x+5)-1(x+5)=(x+5)(3x-1)$
$(x+5)(3x-1)=0 \Rightarrow x=-5 \text{ or } x=\dfrac13$
Check: $x=-5$: $75-70-5=0$ ✓. $x=\frac13$: $3\left(\frac19\right)+\frac{14}{3}-5=\frac13+\frac{14}{3}-5=\frac{15}{3}-5=0$ ✓

**10.** Solve $6x^2-x-15=0$: $ac=-90$. Need sum $-1$, product $-90$: $9,-10$.
$6x^2+9x-10x-15=3x(2x+3)-5(2x+3)=(2x+3)(3x-5)$
$(2x+3)(3x-5)=0 \Rightarrow x=-\dfrac32 \text{ or } x=\dfrac53$
Check: $x=\frac53$: $6\left(\frac{25}9\right)-\frac53-15=\frac{50}3-\frac53-15=\frac{45}3-15=15-15=0$ ✓. $x=-\frac32$: $6\left(\frac94\right)+\frac32-15=13.5+1.5-15=0$ ✓

**11.** Solve $2^{2x}-9(2^x)+8=0$: let $y=2^x$: $y^2-9y+8=0 \Rightarrow (y-1)(y-8)=0 \Rightarrow y=1 \text{ or } y=8$
$2^x=1=2^0 \Rightarrow x=0$
$2^x=8=2^3 \Rightarrow x=3$
Check $x=0$: $2^0-9(2^0)+8=1-9+8=0$ ✓. Check $x=3$: $2^6-9(2^3)+8=64-72+8=0$ ✓

**12.** Solve $3^{2x+1}-10(3^x)+3=0$: rewrite $3^{2x+1}=3\cdot(3^x)^2$. Let $y=3^x$:
$3y^2-10y+3=0$. $ac=9$. Need sum $-10$, product $9$: $-9,-1$.
$3y^2-9y-y+3=3y(y-3)-1(y-3)=(y-3)(3y-1)=0 \Rightarrow y=3 \text{ or } y=\dfrac13$
$3^x=3=3^1 \Rightarrow x=1$
$3^x=\dfrac13=3^{-1} \Rightarrow x=-1$
Check $x=1$: $3^3-10(3)+3=27-30+3=0$ ✓. Check $x=-1$: $3^{-1}-10(3^{-1})+3=\frac13-\frac{10}3+3=-\frac93+3=-3+3=0$ ✓

**13.** Is $(x-1)$ a factor of $f(x)=x^3+2x^2-x-2$?
By the Factor Theorem, check $f(1)$: $f(1)=1+2-1-2=0$. Since $f(1)=0$, yes — $(x-1)$ is a factor.

Divide $f(x)$ by $(x-1)$ (long division) to get the quadratic quotient:
$x^3+2x^2-x-2 \div (x-1) = x^2+3x+2$

So $f(x) = (x-1)(x^2+3x+2)$.

Now factor $x^2+3x+2$ by splitting the middle term: need sum $3$, product $2$: $1,2$.
$x^2+x+2x+2 = x(x+1)+2(x+1)=(x+1)(x+2)$

Therefore: $f(x) = (x-1)(x+1)(x+2)$

Check by expanding $(x-1)(x+1)(x+2)$: $(x-1)(x+1)=x^2-1$, then $(x^2-1)(x+2)=x^3+2x^2-x-2$ ✓

---

## Notes for Next Session

Tonight covered the complete grade-9 foundation: laws of exponents, the Remainder/Factor Theorems, and factoring & solving quadratic equations by splitting the middle term — matched to what his accelerated course is currently doing.

**Still pending (once the grade-10 and grade-11 R.D. Sharma PDFs are available):**

- **Grade 10 — Quadratic Equations chapter:** the completing-the-square method (with full derivation), the quadratic formula (derived from completing the square, not just stated), and the discriminant $b^2-4ac$ for determining the nature of roots (real & distinct, real & equal, no real roots).
- **Grade 11 — accelerated depth:** likely complex/imaginary roots when the discriminant is negative, sum and product of roots ($\alpha+\beta = -b/a$, $\alpha\beta = c/a$) and forming a quadratic from given roots, and possibly quadratic inequalities.

Once those two chapters are shared, the plan is to build the continuation session(s) picking up exactly where tonight left off — same 9→10→11 interleaved structure used for the Physics track.
