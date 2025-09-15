
# Coordination Games, Strategic Interactions, and Cournot Duopoly

## I. Review of Coordination Games

### A. Communication and Coordination

* In **coordination games**, players benefit from aligning their strategies.
* Communication can help players reach a **better equilibrium**.
* Example: *Investment Game* — simple communication (like Patrick’s speech) shifted play toward the good equilibrium.

🔑 Contrast with the [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma):

* In PD, communication does **not** help because defection is a strictly dominant strategy.
* In coordination games, beliefs and leadership matter.

### B. Leadership

* Leadership can guide players to coordinate on one equilibrium over another.
* Even minimal leadership can prevent uncoordinated (bad) outcomes.
* Example: Post-Hurricane Katrina chaos showed the high cost of failed coordination.

---

## II. Strategic Complements vs. Substitutes

* **Strategic Complements**: When the more one player does, the more the other wants to do.

  * Examples: *Investment Game*, *Partnership Game*.
* **Strategic Substitutes**: When the more one player does, the less the other wants to do.

  * Example: *Cournot Duopoly* (output competition).

---

## III. Battle of the Sexes

### A. Game Setup

* Players (a couple) choose between movies: *Bourne Ultimatum*, *Good Shepherd*, *Snow White*.
* Payoffs:

  * Both prefer coordination > miscoordination.
  * Player 1 prefers *Bourne Ultimatum*, Player 2 prefers *Good Shepherd*.
  * *Snow White* is a dominated strategy for both.

### B. Nash Equilibria

* Two pure-strategy equilibria:

  1. Both go to *Bourne Ultimatum*
  2. Both go to *Good Shepherd*
* Conflict arises: each prefers a different equilibrium.

### C. Key Insights

* Unlike pure coordination games, here **preferences diverge**.
* This is the classic [Battle of the Sexes](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29).
* Communication may help but is less straightforward than in pure coordination.

---

## IV. Cournot Duopoly

### A. Setup

* Two firms produce homogeneous goods.
* **Strategies**: Quantities $q_1, q_2$.
* **Costs**: $C(q) = cq$ (constant marginal cost $c$).
* **Demand Curve**:

$$
  P = a - b(q_1 + q_2)
$$

### B. Firm 1’s Payoff

$$
u_1(q_1, q_2) = (a - b(q_1 + q_2))q_1 - cq_1
$$

Expanding:

$$
u_1 = aq_1 - bq_1^2 - bq_1q_2 - cq_1
$$

### C. Best Response Functions

* First-order condition:

$$
  \frac{\partial u_1}{\partial q_1} = a - 2bq_1 - bq_2 - c = 0
$$

* Firm 1’s best response:

$$
  q_1^* = \frac{a - c}{2b} - \frac{q_2}{2}
$$

* By symmetry:

$$
  q_2^* = \frac{a - c}{2b} - \frac{q_1}{2}
$$

### D. Nash Equilibrium

Solving the system:

$$
q_1^* = q_2^* = \frac{a - c}{3b}
$$

* Each firm produces **less than competitive output**, but **more than monopoly output**.
* Total industry output:

$$
  Q^* = q_1^* + q_2^* = \frac{2(a - c)}{3b}
$$

---

## V. Monopoly vs. Competition vs. Cournot

* **Monopoly output**:

$$
  Q^M = \frac{a - c}{2b}
$$
* **Perfect competition output**:

$$
  Q^C = \frac{a - c}{b}
$$

* **Cournot output**:

$$
  Q^* = \frac{2(a - c)}{3b}
$$

📌 Implication:

$$
Q^M < Q^* < Q^C
$$

* **Prices**: Highest under monopoly, lowest under competition, intermediate under Cournot.
* **Profits**: Highest under monopoly, lowest under competition, intermediate under Cournot.

---

## VI. Problems with Collusion

### A. Incentive to Cheat

* If firms agree to split monopoly output, each has an incentive to increase production.
* Best-response dynamics drag firms back to Cournot equilibrium.

### B. Entry of New Competitors

* High industry profits attract new entrants (competitive fringe).
* Example: [OPEC](https://en.wikipedia.org/wiki/OPEC)

  * Collusion failed partly due to North Sea oil, Russian oil, and Latin American production.

---

## VII. Key Takeaways

1. **Coordination games**: Communication and leadership matter; equilibria can be good or bad.
2. **Strategic complements vs. substitutes**: Helps classify games.
3. **Battle of the Sexes**: Coordination with conflicting preferences.
4. **Cournot Duopoly**: Classic model of competition in quantities.
5. **Collusion is unstable**: Incentives to cheat and risk of entry undermine agreements.

---

## References

* [Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium)
* [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)
* [Battle of the Sexes (game theory)](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29)
* [Strategic complements and substitutes](https://en.wikipedia.org/wiki/Strategic_complementarities)
* [Cournot Competition](https://en.wikipedia.org/wiki/Cournot_competition)
* [OPEC](https://en.wikipedia.org/wiki/OPEC)

---
---

# Coordination Games, Leadership, and Cournot Duopoly

## 1. What are Coordination Games, and How Do They Differ from the Prisoner’s Dilemma?

* **Coordination Games**:

  * Players benefit from making the same choice or coordinating actions.
  * Multiple [Nash Equilibria](https://en.wikipedia.org/wiki/Nash_equilibrium) exist, and players prefer being coordinated to being uncoordinated.
  * Example: Choosing “up-left” or “down-right” yields payoff (1,1), while mismatched choices yield (0,0).

* **Difference from [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)**:

  * In PD, defection is a strictly dominant strategy, so communication is ineffective.
  * In coordination games, communication is highly effective—it allows players to agree on one equilibrium, creating a **self-enforcing agreement**.
  * Leadership can guide players to a mutually beneficial outcome.

---

## 2. How Does Leadership Play a Role in Coordination Games?

* Game theory does not fully explain “leadership,” but it identifies when leadership helps:

  * In coordination games, leaders help **choose an equilibrium** and prevent uncoordination.
  * Even simple leadership (“Let’s all coordinate on this option”) can transform failure into success.

* **Example**: Post-Hurricane Katrina chaos illustrated how disastrous failed coordination can be, highlighting the potential role of leadership in crisis management.

---

## 3. What are Strategic Complements and Strategic Substitutes?

* **Strategic Complements**:

  * The more one player does, the more the other wants to do.
  * Examples: *Investment Game*, *Partnership Game*.
  * If others invest or work harder, you are also motivated to do more.

* **Strategic Substitutes**:

  * The more one player does, the less the other wants to do.
  * Example: [Cournot Duopoly](https://en.wikipedia.org/wiki/Cournot_competition).
  * If one firm increases production, the other firm’s best response is to reduce production.

---

## 4. How Does the “Battle of the Sexes” Illustrate Complex Coordination?

* In the [Battle of the Sexes](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29):

  * Both players want to coordinate but disagree on which equilibrium to reach.
  * Example:

    * Player 1 prefers *Bourne Ultimatum*.
    * Player 2 prefers *Good Shepherd*.
    * Both going to *Snow White* is worst.

* **Difference from Pure Coordination Games**:

  * Pure coordination: all players agree on the preferred equilibrium.
  * Battle of the Sexes: preferences diverge → requires negotiation.
  * Real-world analogy: strike negotiations—both sides want an agreement but disagree on terms.

---

## 5. What is the Cournot Duopoly, and Why is it Important?

* **Definition**: Two firms simultaneously choose quantities of an identical product.

  * Market price depends on total quantity:

$$
    P = a - b(q_1 + q_2)
$$

  * Each firm maximizes profits:

$$
    u_i = Pq_i - cq_i
$$

* **Importance**:

  * Models markets **between monopoly and perfect competition**.
  * First major use of **continuous strategies** (calculus required).
  * Illustrates **strategic substitutes**.

---

## 6. How is Nash Equilibrium Found in Cournot Duopoly?

1. **Payoff function (Firm 1)**:

$$
   u_1 = aq_1 - bq_1^2 - bq_1q_2 - cq_1
$$

2. **Best response (FOC)**:

$$
   \frac{\partial u_1}{\partial q_1} = a - 2bq_1 - bq_2 - c = 0
$$

$$
   q_1^* = \frac{a - c}{2b} - \frac{q_2}{2}
$$

3. **By symmetry**:

$$
   q_2^* = \frac{a - c}{2b} - \frac{q_1}{2}
$$

4. **Solve intersection**:

$$
   q_1^* = q_2^* = \frac{a - c}{3b}
$$

---

## 7. Why is Collusion Difficult in Cournot Duopoly?

* **Cheating Incentive**:

  * If firms agree to split monopoly output, each has an incentive to produce more and capture higher profits.
  * Anticipation of cheating drags outcomes back to Cournot equilibrium.

* **Illegality**: Cartels are illegal under antitrust law; agreements cannot be enforced.

* **Entry of New Firms**: High profits attract new entrants, eroding collusive gains.

  * Example: [OPEC](https://en.wikipedia.org/wiki/OPEC) faced new oil producers in the North Sea, Russia, and Latin America.

---

## 8. Comparing Cournot, Monopoly, and Perfect Competition

* **Monopoly output**:

$$
  Q^M = \frac{a - c}{2b}
$$

* **Cournot output**:

$$
  Q^C = \frac{2(a - c)}{3b}
$$

* **Perfect competition output**:

$$
  Q^{PC} = \frac{a - c}{b}
$$

📌 **Comparison**:

$$
Q^M < Q^C < Q^{PC}
$$

* **Prices**: Highest under monopoly, lowest under competition, in between under Cournot.
* **Profits**: Highest under monopoly, zero in perfect competition, intermediate under Cournot.
* **Welfare**:

  * Producers prefer monopoly > Cournot > competition.
  * Consumers prefer competition > Cournot > monopoly.

---

## References

* [Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium)
* [Coordination Game](https://en.wikipedia.org/wiki/Coordination_game)
* [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)
* [Battle of the Sexes (game theory)](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29)
* [Strategic Complements & Substitutes](https://en.wikipedia.org/wiki/Strategic_complementarities)
* [Cournot Competition](https://en.wikipedia.org/wiki/Cournot_competition)
* [OPEC](https://en.wikipedia.org/wiki/OPEC)

---
