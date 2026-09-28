# Hypothesis Testing: Choosing the Cutoff

**In class** we used the simulation method: reject the hypothesis if a result as extreme as yours shows up in **about 5% or less** of the simulated samples. **If your teacher uses a different cutoff, go with your teacher's.**

---

## What the cutoff is called

In statistics, that 5% cutoff is called the **significance level**, written **α = 0.05** (α is the Greek letter "alpha").

The claim you are testing (e.g. "the coin is fair") is called the **null hypothesis**.

## How the decision changes with the cutoff

| Teacher's cutoff | Reject the null hypothesis if the result shows up in… | What it means |
| --- | --- | --- |
| **1%** (α = 0.01) | 1% or less of the simulated samples | **Stricter**: needs stronger evidence to reject |
| **5%** (α = 0.05) | 5% or less of the simulated samples | The usual standard |
| **10%** (α = 0.10) | 10% or less of the simulated samples | **More lenient**: easier to reject |

## The core decision rule (the same for every cutoff)

<div class="rule">
If &nbsp;<b>P</b>(simulated outcome ≥ observed outcome) &nbsp;≤&nbsp; teacher's cutoff<br>
&nbsp;&nbsp;&nbsp;&nbsp;→ &nbsp;<b>Reject the null hypothesis.</b><br><br>
Otherwise &nbsp;→ &nbsp;<b>Do not reject</b> it. The data doesn't give enough evidence against the claim, but that does <i>not</i> prove the claim is true.
</div>

## Quick check with our coin examples

- **36 heads in 50 flips:** 0 of 200 fair-coin samples were that high, which is **0%**. That is below every cutoff (1%, 5% or 10%), so **reject** in all three cases.
- **29 heads in 50 flips:** 39 of 200 samples were that high, which is **19.5%**. That is above every cutoff, so **do not reject** in all three cases.
