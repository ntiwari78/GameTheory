

# Study Guide: Candidate–Voter Model, Schelling Segregation, and Mixed Strategies

---

## 1. Candidate–Voter Model: Key Lessons

* **Fixed Positions:** Unlike the [Downs median-voter model](https://en.wikipedia.org/wiki/Median_voter_theorem), candidates cannot choose their positions; they inherit them from their ideology/voter identity.
* **Multiple Equilibria:**

  * Candidates do not always crowd the center.
  * Entry from one side (left or right) can shift the outcome in favor of the **opposite side**.
  * If candidates are too extreme, centrist entry is likely to win.

📌 **Real-world examples:** Ralph Nader in 2000 (left entry aiding the right), third-party threats in Republican primaries, UK politics during Thatcher’s era.

---

## 2. Schelling Segregation Model

Developed by [Thomas Schelling](https://en.wikipedia.org/wiki/Thomas_Schelling), this model explains how **segregation emerges even when individuals prefer integration.**

### Setup

* Two towns: East and West.
* Two types of people: tall vs short (a stand-in for social categories, e.g., ethnicity).
* Preferences:

  * Prefer **mixed towns** (highest utility).
  * If not mixed, prefer being in the **majority**.

### Equilibria

* **Two segregated equilibria:** all tall in one town, all short in the other.

  * **Strict and stable** (no incentive to deviate).
* **One integrated equilibrium (50/50 split):**

  * **Weak and unstable.** Any small deviation tips the outcome toward segregation.

### Key Insights

* **Segregation without preference for segregation.**
* **Tipping points:** Once imbalance crosses a threshold, the system moves toward segregation.
* **Policy implications:**

  * **Randomization** (e.g., bussing, randomized housing/school assignments) can sustain integration.
  * Examples: [school bussing](https://en.wikipedia.org/wiki/Desegregation_busing), Harvard/Yale randomization into houses/colleges.

---

## 3. Mixed Strategies in Game Theory

So far, strategies were **pure** (e.g., invest/not invest, choose left/right).
Now, we expand to **mixed strategies** — randomizing over pure strategies.

### Example: Rock–Paper–Scissors

* Payoff matrix cycles: Rock beats Scissors, Scissors beats Paper, Paper beats Rock.
* **No pure strategy Nash Equilibrium.**
* **Unique mixed strategy equilibrium:** each player plays Rock, Paper, Scissors with equal probability:

$$
\left(\tfrac{1}{3}, \tfrac{1}{3}, \tfrac{1}{3}\right)
$$

* Expected payoff = **0** for each player.

📌 **Implication:** Mixed strategies are essential in games without stable pure-strategy equilibria.

---

## 4. Key Takeaways

* **Candidate–Voter model:** Multiplicity of equilibria, strategic entry can backfire.
* **Schelling model:** Segregation can emerge endogenously, even if individuals prefer integration.
* **Mixed strategies:** Broaden the concept of equilibrium; critical in competitive and cyclical games.

---

## References

* [Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)
* [Thomas Schelling](https://en.wikipedia.org/wiki/Thomas_Schelling)
* [Schelling’s Segregation Model](https://en.wikipedia.org/wiki/Schelling%27s_model_of_segregation)
* [Desegregation Busing](https://en.wikipedia.org/wiki/Desegregation_busing)
* [Hotelling’s Law](https://en.wikipedia.org/wiki/Hotelling%27s_law)
* [Mixed Strategy Nash Equilibrium](https://en.wikipedia.org/wiki/Mixed_strategy)
* [Rock–Paper–Scissors](https://en.wikipedia.org/wiki/Rock_paper_scissors)

---
---

## 1) Candidate–Voter Model: definition & political equilibria

**What it is:** A model where *any voter can enter as a candidate* and each candidate’s ideological position is **fixed** (can’t be repositioned). Voters choose the closest running candidate; the number of entrants is endogenous.

**Key lessons**

* **Multiple equilibria:** Not all equilibria feature candidates at the center (unlike Downs/median-voter).
* **Entry can backfire:** A same-side entrant (e.g., left) can split that side and help the other side win.
* **Limits to extremism:** If two candidates are too far apart (e.g., beyond **1/6** and **5/6** on the line), a centrist can profitably enter and win.

---

## 2) How segregation emerges despite a preference for integration

Two towns (East/West), two types (Tall/Short). Everyone prefers a **50/50 mix** most; otherwise they prefer being in their **own majority** over being a minority.

**Mechanism:** Any slight imbalance makes majority towns more attractive to that type → more migration toward the majority → **cascade** → ends in **segregated** towns (all Tall in one, all Short in the other), even though everyone would have preferred integration.

---

## 3) Nash equilibria in the segregation model

* **Two segregated equilibria (strict & stable):**

  * All Tall in A, all Short in B (or vice versa).
  * Any deviator strictly worse (½ → 0).
* **One integrated equilibrium (weak & unstable):**

  * Exactly 50/50 in each town.
  * Tiny perturbations tip the system toward segregation.
* **“Silly” equilibria (all choose the same town → random rationing):**

  * If overcrowded, random assignment splits residents \~50/50.
  * Existence hinges on the *rationing rule*—a modeling detail, not a preference.

---

## 4) Tipping points

A **tipping point** is a threshold where small deviations trigger a big shift. Here, being even slightly off 50/50 pushes dynamics toward **complete segregation**—illustrating how small shocks can produce large, persistent social changes.

---

## 5) Mixed strategies & why RPS needs them

**Mixed strategy:** Randomize over pure actions (e.g., Rock, Paper, Scissors each with probability **1/3**).

**Why needed in RPS:** No pure-strategy NE (Rock → Paper → Scissors → Rock). The unique NE is both players mixing **(1/3, 1/3, 1/3)**, yielding **expected payoff 0**—and making play unexploitable.

---

## 6) Sociological lesson from segregation

Do **not** infer preferences from outcomes. Widespread segregation can arise from benign individual motives (majority preference when not perfectly mixed), so observed patterns need not reflect a desire for segregation.

---

## 7) Policy links: bussing & random allocation

Centralized randomization (e.g., **school bussing**, **random house assignments**) can **bypass coordination cascades** that produce segregation and steer the system toward integrated allocations—mirroring the model’s random-rationing “silly” equilibria.

---

## 8) Game-theory lesson on “irrelevant details”

Seemingly minor modeling choices (e.g., **how overcrowding is rationed**) can **create equilibria** and shape predictions. Always audit such assumptions; they can drive results as much as core preferences or payoffs.

---

### Key takeaways

* Entry and strategic positioning can overturn median-voter intuitions.
* Small shocks around unstable equilibria can have outsized social effects.
* Mixed strategies are essential whenever pure strategies cycle.
* Modeling plumbing (allocation/rationing rules) can be outcome-determinative.
