# Study Guide: Mixed Strategies, Expected Payoffs, and Tennis Example (Polak)

---

## 1. Formal Definition of Mixed Strategies

* A **mixed strategy** for player $i$, denoted $P_i$, is a **probability distribution** over $i$’s pure strategies.
* Notation:

  * $P_i(s_i)$ = probability that player $i$ plays pure strategy $s_i$.
* Special cases:

  * If $P_i(s_i) = 1$, this reduces to a **pure strategy**.
  * If some $P_i(s_i) = 0$, those pure strategies are excluded from the mix.

Thus, pure strategies are embedded as special cases of mixed strategies.

---

## 2. Expected Payoffs of Mixed Strategies

* The **expected payoff** of a mixed strategy is the **weighted average** of the payoffs of the pure strategies being played.
* Example (Battle of the Sexes):

  * If Player I plays $P = (1/5, 4/5)$ and Player II plays $Q = (1/2, 1/2)$, compute:

    * Payoff of A vs Q = $(1/2)(2) + (1/2)(0) = 1$.
    * Payoff of B vs Q = $(1/2)(0) + (1/2)(1) = 0.5$.
    * Payoff of $P$ = $(1/5)(1) + (4/5)(0.5) = 0.6$.
* General rule:

  * Averages **always lie between** the min and max values of the included strategies.

---

## 3. Key Lesson: Equalization in Mixed Strategy Best Responses

* **Big conclusion:**
  If a mixed strategy is a best response, then every pure strategy played with positive probability must itself be a best response.
* Therefore:

  * All pure strategies in the support of a best-response mix yield the **same expected payoff**.
  * Otherwise, a player could drop the weaker strategy and improve their average.

This insight provides a **powerful tool** for finding mixed-strategy Nash equilibria.

---

## 4. Mixed Strategy Nash Equilibrium (MSNE): Formal Definition

A profile of mixed strategies $(P_1^{\ *}, P_2^{\ *}, \dots, P_N^{\ *})$ is a **Mixed Strategy Nash Equilibrium** if, for each player $i$:

$$
u_i(P_i^{\ *}, P_{-i}^{\ *}) \geq u_i(P_i, P_{-i}^{\ *}) \quad \text{for all } P_i
$$

That is, each player’s mixed strategy is a best response to the others.

---

## 5. Application: Venus vs. Serena (Tennis Passing-Shot Game)

### Setup

* **Players:** Venus (row), Serena (column).
* **Strategies:**

  * Venus: Pass left (L) or right (R).
  * Serena: Lean left (L) or right (R).
* **Payoffs (probabilities of winning the point):**

| Venus / Serena | Left (L) | Right (R) |
| -------------- | -------- | --------- |
| **Left (L)**   | (50,50)  | (80,20)   |
| **Right (R)**  | (90,10)  | (20,80)   |

---

### Step 1: No Pure Strategy Equilibrium

* Serena’s best response to Venus’ L is L.
* Serena’s best response to Venus’ R is R.
* Venus’ best response to Serena’s L is R.
* Venus’ best response to Serena’s R is L.
* **Cycle of responses → no pure-strategy NE.**

---

### Step 2: Solve for Mixed Strategy NE

* Let Venus mix: $(P, 1-P)$.
* Let Serena mix: $(Q, 1-Q)$.
* Trick: Solve Serena’s mix using **Venus’ payoffs** (equalize them).
* Calculation yields:

  * $Q = 0.6$, $P = 0.7$.

**Interpretation:**

* Venus passes left 70% of the time, right 30%.
* Serena leans left 60% of the time, right 40%.
* Each player’s randomization makes the opponent indifferent.

---

## 6. Comparative Statics: Improving Serena’s Backhand

* Suppose Serena improves her backhand volley success rate: payoff changes from (50,50) → (30,70).

### Intuition

* **Direct effect:** Stronger backhand → Serena should lean left more often.
* **Strategic effect:** Venus now avoids Serena’s left → Serena should lean left less.

### Result

* New equilibrium: $Q = 0.5$, $P = 7/12$.
* **Q decreased** → strategic effect dominates.

---

## 7. Key Takeaways

* Mixed strategies = randomization over pure strategies.
* Expected payoffs = weighted averages, lying between best and worst.
* If a mixed strategy is optimal, every included pure strategy must yield equal payoff.
* Mixed-strategy NE ensures mutual indifference.
* Comparative statics highlight **direct vs. strategic effects**:

  * Players adapt not just to their own improvements, but to opponents’ responses.

---

## References

* [Mixed strategy Nash equilibrium](https://en.wikipedia.org/wiki/Mixed_strategy)
* [Battle of the Sexes (game theory)](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29)
* [Tennis strategy](https://en.wikipedia.org/wiki/Tennis_strategy)
* [Game Theory (Yale OYC, Ben Polak)](https://oyc.yale.edu/economics/econ-159)

---
---

## 1. What is a Mixed Strategy?

* A **mixed strategy** is a probability distribution over a player’s pure strategies.
* Example: In [Rock–Paper–Scissors](https://en.wikipedia.org/wiki/Rock_paper_scissors), playing each option with probability $1/3$ is a mixed strategy.
* Denoted as $P_i(s_i)$, where $s_i$ is a pure strategy and $P_i(s_i)$ is the probability assigned.

---

## 2. Are Pure Strategies Mixed Strategies?

* Yes.
* A **pure strategy** is a **special case** of a mixed strategy where one strategy has probability 1 and all others have probability 0.
* Example: Always playing "rock" = $P(\text{rock}) = 1$, $P(\text{paper}) = 0$, $P(\text{scissors}) = 0$.

---

## 3. How Are Expected Payoffs Calculated?

* The **expected payoff** of a mixed strategy = weighted average of payoffs from pure strategies in the mix.

$$
\mathbb{E}[u] = P(A) \cdot E(A) + P(B) \cdot E(B) + \dots
$$

* Example: If a player mixes 50% A and 50% B, and $E(A) = 2$, $E(B) = 4$:
  $\mathbb{E}[u] = 0.5 \cdot 2 + 0.5 \cdot 4 = 3$.

---

## 4. Key Principle of Best Response in Mixed Strategies

* If a **mixed strategy is a best response**, every pure strategy used with positive probability in the mix must:

  1. Be a **best response** itself.
  2. Yield the **same expected payoff** as the others in the mix.
* Otherwise, the player could shift probability toward the higher-yielding strategy.

---

## 5. Mixed vs. Pure Strategy Nash Equilibria

* **Pure Strategy Nash Equilibrium (PSNE):** Each player’s pure strategy is a best response to the other players’ strategies.
* **Mixed Strategy Nash Equilibrium (MSNE):** Same definition, but players may use **probability distributions** over strategies.
* Implication: If a mixed strategy is part of an equilibrium, every pure strategy played with positive probability is also a best response.

---

## 6. Why Mixed Strategies Are Needed

* Some games (e.g., tennis passing-shot game, Rock–Paper–Scissors) have **no pure strategy equilibrium**.
* Without mixing, players cycle endlessly between strategies.
* Mixed strategies create **stable equilibria**, where randomisation prevents exploitation.

---

## 7. The Trick for Finding a Mixed Strategy NE

* To find **Player 2’s mix**, look at **Player 1’s payoffs**:

  * If Player 1 is mixing, then each pure strategy in their mix must yield the **same expected payoff**.
  * Equating those payoffs gives Player 2’s equilibrium probabilities.
* Repeat symmetrically for Player 1’s mix.

This is the main computational shortcut.

---

## 8. Comparative Statics in Mixed Strategy Equilibria

* **Comparative statics** = studying how equilibria change when payoffs change.
* Example: If Serena’s backhand improves in the tennis game:

  * **Direct effect:** Serena should lean left more (better backhand).
  * **Strategic effect:** Venus will avoid her left more, so Serena should actually lean left less.
* Often, **strategic effects outweigh direct effects**, leading to counterintuitive results.

---

## References

* [Mixed Strategy Nash Equilibrium – Wikipedia](https://en.wikipedia.org/wiki/Mixed_strategy)
* [Nash Equilibrium – Wikipedia](https://en.wikipedia.org/wiki/Nash_equilibrium)
* [Comparative Statics – Wikipedia](https://en.wikipedia.org/wiki/Comparative_statics)
* [Game Theory (Yale OYC, Ben Polak)](https://oyc.yale.edu/economics/econ-159)

---
