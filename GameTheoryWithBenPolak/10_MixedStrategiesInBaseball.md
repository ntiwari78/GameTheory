# Study Guide: Mixed Strategies, Applications, and Policy Lessons

Based on Professor Ben Polak’s lecture (Yale Open Course, *Game Theory*).

---

## 1. Key Principle of Mixed Strategy Equilibria

* **Big Idea:** If a player mixes in equilibrium, every pure strategy used with positive probability must be a **best response**.
* This means:

  * All pure strategies in the mix yield the **same expected payoff**.
  * Any other strategy must not yield a strictly higher payoff.

---

## 2. Checking Equilibria

* To verify a mixed strategy Nash Equilibrium (NE):

  * Check that each pure strategy in the mix gives the same payoff.
  * Then check that **no other pure strategy deviation** gives a strictly higher payoff.
* ✅ If no profitable pure strategy deviation exists, then **no profitable mixed deviation exists**, since mixed strategies are just weighted averages of pure strategies.

---

## 3. Applications of Mixed Strategies

### Sports

* **Tennis (Serena vs. Venus):** Players mix between forehand and backhand to remain unpredictable.
* **American Football:** Offense mixes between running and passing; defense mixes between run defense and pass rush.
* **Baseball:**

  * Pitcher mixes pitch types (fastball, curveball, etc.).
  * Batter anticipates pitch types (effectively mixing beliefs).
  * Base stealing: Runners randomize attempts; pitchers randomize responses (pick-off, fast delivery, pitch-out).
  * **Key Insight:** If stealing and not stealing yield equal expected returns, that *proves* the runner is mixing optimally.

### Security & Defense

* **Airport Security (post-9/11):** Random baggage checks and random passenger searches prevent predictable attacks.
* **Military Strategy:** Randomizing convoy protection prevents insurgents from exploiting patterns.

---

## 4. Battle of the Sexes (Revisited)

* Players: Nina (prefers **apple picking**) and David (prefers **theatre**).
* Two pure equilibria:

  1. Both choose apple picking (Nina happier).
  2. Both choose theatre (David happier).
* **Mixed NE:**

  * Nina: $P = \tfrac{2}{3}$ apple, $1-P = \tfrac{1}{3}$ theatre.
  * David: $Q = \tfrac{1}{3}$ apple, $1-Q = \tfrac{2}{3}$ theatre.
* Payoffs: Each gets **$\tfrac{2}{3}$**.
* Problem: They fail to meet more than half the time → **inefficient equilibrium**.
* Interpretation: Better seen as **beliefs about opponents’ actions**, not literal randomization.

---

## 5. Tax Compliance Model (Auditor vs. Taxpayer)

* Players:

  * **Taxpayer:** Honest (H) or Cheat (C).
  * **Auditor:** Audit (A) or Not Audit (NA).

### Payoff Matrix

|                | Audit (A) | Not Audit (NA) |
| -------------- | --------- | -------------- |
| **Honest (H)** | (2, 0)    | (4, 0)         |
| **Cheat (C)**  | (4, -10)  | (0, 4)         |

### Mixed NE

* Taxpayers pay honestly **$\tfrac{2}{3}$** of the time.
* Auditor audits with probability **$\tfrac{2}{7}$**.
* Interpretation:

  * Auditor is literally randomizing.
  * Taxpayers are not tossing coins → instead, **a proportion of the population cheats**.

---

## 6. Policy Experiment: Raising Fines

* Suppose fine increases from $-10$ to $-20$.
* **Result:**

  * Tax compliance rate **unchanged** (still $\tfrac{2}{3}$).
  * Audit probability falls (from $\tfrac{2}{7}$ to $\tfrac{1}{6}$).
* **Lesson:** Changing column player’s payoff (taxpayer) affects row player’s mix (auditor), not taxpayers’ behavior.

---

## 7. Lessons and Insights

1. **Checking equilibria:** Only need to check pure strategy deviations.
2. **Interpretations of mixed strategies:**

   * Literal randomization.
   * Beliefs about opponent behavior.
   * Population proportions.
3. **Policy lesson:**

   * Changing one player’s payoffs shifts the other’s equilibrium mix.
   * To increase tax compliance, need to adjust **auditor’s incentives**, not just taxpayer penalties.
4. **Broader application:** Mixed strategies explain behavior in sports, security, economics, and politics.

---

## References

* [Mixed Strategy Nash Equilibrium – Wikipedia](https://en.wikipedia.org/wiki/Mixed_strategy)
* [Battle of the Sexes (Game Theory) – Wikipedia](https://en.wikipedia.org/wiki/Battle_of_the_sexes_%28game_theory%29)
* [Tax Compliance and Game Theory – Research Overview](https://en.wikipedia.org/wiki/Tax_compliance)
* [Game Theory (Yale OYC, Ben Polak)](https://oyc.yale.edu/economics/econ-159)

---
---

# 🎯 Study Guide: Mixed Strategies in Game Theory

## 1. What is a mixed strategy in game theory, and how does it relate to real-world scenarios?

* **Definition:** A mixed strategy is when a player randomises over their pure strategies, assigning probabilities to each action.
* **Equilibrium condition:** For a player to mix, all pure strategies in the mix must yield the same expected payoff.
* **Examples:**

  * ⚽ **Football:** Offense mixes running vs. passing; defense mixes run vs. pass defense.
  * ⚾ **Baseball:** Pitchers mix pitch types; runners randomise stealing; batters form beliefs.
  * ✈️ **Security:** Authorities randomise baggage checks to prevent predictability.

---

## 2. How do you identify a Nash Equilibrium with mixed strategies?

* A **mixed strategy NE** occurs when:

  * Each player’s strategy is a **best response** to the other’s.
  * Indifference holds: pure strategies in the mix yield **equal expected payoffs**.
* **Method:**

  * Write expected payoff equations.
  * Solve for probabilities that make players indifferent.
* **Example:** Serena–Venus tennis game → equilibrium mixes found by equating expected payoffs for “hit left” and “hit right.”

---

## 3. Why check only pure-strategy deviations when verifying a mixed-strategy NE?

* Any mixed strategy is a **weighted average** of pure strategies.
* If **no pure strategy** gives a strictly better payoff, then **no mixture** can either.
* ✅ Simplifies verification: only finitely many pure deviations, instead of infinitely many mixed ones.

---

## 4. Interpretations of mixed strategies

1. **Literal Randomisation**

   * Genuine randomising (coin flips, random devices).
   * Seen in sports (pitching, penalty kicks) and security checks.

2. **Beliefs about Opponent’s Actions**

   * Mixed strategies represent beliefs rather than actual randomisation.
   * Example: In a dating game, Nina’s “mix” may be David’s belief about her choices.

3. **Population Proportions**

   * In large populations, mixes represent proportions, not individuals randomising.
   * Example: In the **tax audit game**, 2/3 of taxpayers comply, 1/3 cheat.

---

## 5. How do mixed strategies explain chaotic situations (e.g., Battle of the Sexes)?

* Pure equilibria: players always meet (apple-picking or theatre).
* **Mixed equilibrium:**

  * Players fail to coordinate >50% of the time.
  * Each gets lower payoffs (e.g., 2/3 vs. 1 or 2).
* Insight: Mixed strategies model **mis-coordination** and uncertainty, reflecting real-life failures to coordinate.

---

## 6. Policy Insights: Tax Compliance Example

* **Setup:** Taxpayers (honest/cheat) vs. Auditor (audit/not).
* **Result:**

  * Raising fines for cheating → **no change in compliance rate**.
  * Instead, audit rates fall (auditors need fewer checks to maintain indifference).
* **Lesson:**

  * Compliance is determined by **auditor’s payoffs**, not taxpayer penalties.
  * Effective policy = change auditor incentives (make audits cheaper/more rewarding).

---

## 7. How do payoffs influence opponents’ strategies?

* **Rule:** A player’s mix is determined by the **other player’s payoffs**.

  * Taxpayer compliance depends on auditor’s payoffs.
  * Auditor’s audit rate depends on taxpayer’s payoffs.
* Policy implication: To affect one player’s behavior, change **the other’s incentives**.

---

## 8. Why is true randomisation hard for humans?

* Humans struggle to produce truly random patterns.
* Implication:

  * Players risk being predictable if they “fake randomisation.”
  * Sports teams/military often use conscious randomisation tools (e.g., dice, hand signals).
* Example: A military commander literally randomised convoy protection by drawing lots.

---

✅ **Key Takeaways:**

* Mixed strategies ensure unpredictability and explain equilibrium in games without pure solutions.
* They can be read as literal randomness, beliefs, or population proportions.
* Policy and strategy must account for **how one side’s payoffs shape the other’s behavior**.

---
