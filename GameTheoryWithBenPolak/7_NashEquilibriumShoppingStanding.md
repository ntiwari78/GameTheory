# Imperfect Competition, Differentiated Products, and Elections

*(Study guide based on Prof. Ben Polak’s lecture)*

---

## 1) Big Picture

We’re studying how outcomes change when we vary **how firms compete** and **how candidates enter**:

* **Cournot (quantities)** vs **Bertrand (prices)** with identical goods.
* Adding **differentiated products** (Hotelling/linear city) to fix the “Bertrand paradox.”
* A **candidate–voter model** with **endogenous entry** (any voter can run) and **fixed policy positions**.

---

## 2) Recap: Cournot Competition (quantities)

* **Players:** 2 firms producing an identical good.
* **Strategy:** choose quantity $q_i \ge 0$.
* **Price:** $P = a - b(q_1 + q_2)$.
* **Cost:** constant marginal cost $c$.
* **Profit:** $\pi_i = P q_i - c q_i$.

**Result:** In Nash equilibrium $q_1^* = q_2^* = (a-c)/(3b)$.
**Comparisons (total quantity $Q$):**

* Monopoly: $Q^M = (a-c)/(2b)$
* **Cournot:** $Q^C = 2(a-c)/(3b)$
* Perfect competition: $Q^{PC} = (a-c)/b$

So $Q^M < Q^C < Q^{PC}$ (and prices/profits move in the opposite order). Cournot lands **between** monopoly and perfect competition.

---

## 3) Bertrand Competition (prices) with identical goods

* **Players:** same 2 firms, identical product.
* **Strategy:** choose price $P_i \in (0,1)$.
* **Demand:** all consumers buy from the **lower-priced** firm; if tie, split.
* **Cost:** constant marginal cost $c$.
* **Profit:** $\pi_i = Q_i (P_i - c)$.

**Best-response logic:**

* If rival sets $P_j > c$: undercut slightly, capture market.
* If rival sets $P_j < c$: price above them; sell 0 (better than selling at a loss).
* If rival sets $P_j = c$: any $P_i \ge c$ is a best response.

**Nash Equilibrium:** $P_1 = P_2 = c$ ⇒ **zero profits** (the **Bertrand paradox**).
**Takeaway:** With identical goods, **price competition is “too strong”**—two firms already mimic perfect competition.

---

## 4) Fixing Bertrand: Differentiated Products (Hotelling / Linear City)

**Idea:** Soften price competition by making products **not identical**.

**Setup (Linear City):**

* Consumers uniformly distributed on a line $[0,1]$.
* Firm 1 at 0, Firm 2 at 1 (locations can be interpreted as physical distance or product “taste”).
* Each consumer buys **one unit** from the firm with the lowest **total cost**:

  $$
  \text{Total cost from firm at } x_i: \; P_i + T \cdot \text{(distance)}^2
  $$
* Firms choose **prices** $P_1, P_2$; demand splits at the **indifferent consumer**.

**Key implications:**

* Because consumers dislike distance (or mismatch), firms have **local market power**.
* Equilibrium prices satisfy $P_i > c$ (profits **> 0**), and outcomes now sit **between monopoly and perfect competition**—more like Cournot.
* The “distance cost” can be literal travel or **taste mismatch** (e.g., Guinness vs Bud Light). This is a general model of differentiation.

---

## 5) Candidate–Voter Model with Endogenous Entry

**Goal:** Model elections where anyone can run and candidates **can’t reposition** (their ideology is known).

**Setup:**

* Voters uniformly on $[0,1]$ (left to right).
* **Any voter can run** (simultaneous entry).
* Voters vote for the **closest** running candidate.
* **Plurality wins**; break ties fairly.
* **Payoffs:**

  * If you run and **win**: gain $B$, pay cost $C$.
  * If you run and **lose**: pay $C$.
  * Regardless of running, if the winner is at position $y$ and you’re at $x$, you incur **disutility** $-|x-y|$.
* In class, we used $B=2C$ to make “office benefit vs entry cost” roughly a wash when winning with probability 1/2.

**In-class findings (via experiments):**

* **No one runs** is **not** an equilibrium (anyone can deviate, win, and get $B-C>0$).
* **Single-candidate equilibrium:** Yes—**the median** voter runs **alone**.

  * Any challenger off-center would **lose** (and still pay $C$).
* **Two identical centrists stacked at the median:** **Not** an equilibrium.

  * A slightly off-center entrant can win by taking an entire side while the centrists split the other side.
* **A stable 2-candidate configuration:** Two candidates **bracketing the median** (adjacent positions around the center) can be stable:

  * Neither wants to exit (exiting hands certain victory to a more distant opponent).
  * Additional entrants either lose or make the winner farther from them (worse policy loss).
* **Extreme pair only (far left vs far right):** tempting to test, but typically **not stable**—a centrist can enter and win by capturing the middle. *(Left as an open question in the lecture; intuition points to instability.)*

**Intuition:** Entry trades off **office benefits** vs **entry costs** vs **policy loss** from who wins. Endogenous entry tends to select:

* **One median candidate**, or
* **Two candidates** that **straddle the median** (no profitable deviation to enter/exit).

---

## 6) Why this all matters

* **Modeling choices matter:** Cournot vs Bertrand with identical goods yield **very different** predictions.
* **Add realism (differentiation)** and both price and quantity competition deliver outcomes **between** monopoly and perfect competition.
* **Politics mirrors markets:** The ideological line works like Hotelling’s product space; **entry** and **position** constraints shape equilibrium candidate sets.

---

## 7) Key objects & notation (GitHub-friendly)

* Demand (Bertrand identical goods): total $Q(P) = 1 - P$ (for the **lower** price).
* Profit (firm $i$): $\pi_i = Q_i \cdot (P_i - c)$.
* Hotelling mismatch cost: $T \cdot \text{distance}^2$.
* Election disutility: $-|x - y|$ if the winner is at $y$ and you are at $x$.
* Cournot equilibrium quantity per firm: $(a - c)/(3b)$.

---

## 8) Quick self-check questions

1. Why does Bertrand with identical goods deliver $P=c$ and zero profits?
2. How does product differentiation change firms’ pricing incentives?
3. In the candidate–voter model, why is “two stacked centrists” not an equilibrium?
4. What configurations of entrants are stable around the median, and why?

---
---

# Study Guide: Cournot, Bertrand, and the Candidate–Voter Model

---

## 1. Fundamental Differences: Cournot vs. Bertrand

* **Cournot competition**: Firms choose **quantities** ($q_i$), and the **market sets price** based on total output.
* **Bertrand competition**: Firms choose **prices** ($P_i$), and the **market sets quantities** based on consumer demand.

👉 This difference in the **strategic variable** (quantity vs price) drives very different predictions for profits, prices, and consumer surplus.

📖 [Cournot Competition](https://en.wikipedia.org/wiki/Cournot_competition) | [Bertrand Competition](https://en.wikipedia.org/wiki/Bertrand_competition)

---

## 2. Outcomes Compared to Monopoly and Perfect Competition

* **Cournot outcomes** lie **between monopoly and perfect competition**:

  * Output: higher than monopoly, lower than perfect competition.
  * Price: lower than monopoly, higher than perfect competition.
  * Profits and consumer surplus: intermediate.

* **Bertrand outcomes (with identical products, constant marginal cost):**

  * Price = marginal cost.
  * Profits = 0.
  * Consumer surplus maximized.
  * Outcome identical to perfect competition, even with only two firms.

---

## 3. Why Bertrand Collapses to Perfect Competition

* With **identical products** and **constant marginal costs**:

  * Each firm can capture the whole market by undercutting the rival’s price.
  * This continues until prices fall to marginal cost ($P = c$).
  * At this point, neither firm can profitably cut further → **Nash Equilibrium**.

This strong undercutting logic explains the **Bertrand paradox**.

---

## 4. Limitations of the Bertrand Model

* Unrealistic prediction: **2 firms → perfect competition**.
* Driven by **strong assumptions**:

  * Identical products.
  * Constant marginal cost.

**Fix:** Introduce **product differentiation** → firms retain some market power.

---

## 5. Linear City Model: Differentiation

* Consumers are uniformly distributed on a line $[0,1]$.
* Firm 1 at 0, Firm 2 at 1.
* Consumer at $y$ faces **total cost** from firm $i$:

$$
\text{Total cost} = P_i + T \cdot (\text{distance})^2
$$

* Each consumer buys from the firm offering **lowest total cost**.

👉 **Key effect:** Even with price cuts, some consumers stick with the “closer” firm, giving both firms **local market power**.
👉 **Outcome:** Prices $> c$, profits $> 0$, equilibrium sits **between monopoly and perfect competition**, like Cournot.

📖 [Hotelling’s Model of Spatial Competition](https://en.wikipedia.org/wiki/Hotelling%27s_law)

---

## 6. Candidate–Voter Model

**Political version of competition, extending Hotelling’s idea.**

* **Players:** Voters (uniformly distributed on $[0,1]$).
* **Strategy:** Each voter decides **whether to run** (entry game).
* **Voting rule:** Each votes for the **closest candidate**; plurality wins.
* **Payoffs:**

  * If you **run and win**: $B - C$.
  * If you **run and lose**: $-C$.
  * Regardless: disutility of $-|x-y|$, where $x$ = your position, $y$ = winner’s position.
* Assume $B \geq 2C$.

📖 [Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)

---

## 7. Nash Equilibria in Candidate Entry

1. **No one runs**: ❌ Not equilibrium → any voter could deviate, run, win, and improve payoff.

2. **Exactly one candidate runs (median voter)**: ✅ Equilibrium.

   * Median wins.
   * Challengers would lose and still pay cost $C$.

3. **Two identical centrists**: ❌ Not equilibrium.

   * A slightly off-center challenger could win by capturing a side while the centrists split votes.

4. **Two candidates bracketing the median**: ✅ Can be equilibrium.

   * Neither wants to exit (dropping out hands victory to a more distant candidate).
   * No profitable new entry, since challengers would lose or worsen their policy outcome.

5. **Two extremists (far left vs far right)**: Usually ❌ not equilibrium.

   * A centrist entrant can win by capturing the large middle.

---

## 8. Key Takeaways

* **Cournot**: Output competition → equilibrium between monopoly and competition.
* **Bertrand**: Price competition → collapse to marginal cost (with identical goods).
* **Linear City/Hotelling**: Differentiation restores realism → intermediate outcomes.
* **Candidate–Voter model**: Political analogue of Hotelling → equilibria depend on entry decisions and fixed ideological positions.

---

### References

* [Cournot Competition](https://en.wikipedia.org/wiki/Cournot_competition)
* [Bertrand Competition](https://en.wikipedia.org/wiki/Bertrand_competition)
* [Hotelling’s Law (Linear City)](https://en.wikipedia.org/wiki/Hotelling%27s_law)
* [Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)

---
