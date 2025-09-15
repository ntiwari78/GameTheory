
# Game Theory Lecture: Best Response and the Penalty Kick Game

## Introduction to Best Response

**Best Response** refers to a strategy that maximizes a player’s payoff given their beliefs about what other players are doing.

- **Example scenario**: If your boss asks why you chose an action, a valid answer is "I believed others would do X, and this was my best response."
- This idea helps justify decision-making in strategic environments.

---

## Case Study: The Penalty Kick Game

### Game Setup

- A common scenario in soccer, such as a **World Cup penalty shootout**.
- **Shooter’s options**: Left, Middle, Right
- **Goalkeeper’s options**: Dive Left or Right (initially ignoring Middle)

### Payoffs

| Shooter \ Goalkeeper | Left (GK) | Right (GK) |
|----------------------|-----------|------------|
| Left                 | (4, -4)   | (9, -9)    |
| Middle               | (6, -6)   | (6, -6)    |
| Right                | (9, -9)   | (4, -4)    |

- Payoffs represent **probability of scoring**, scaled (e.g., 4 = 40%).
- Goalkeeper’s payoff is the negative of the shooter’s.

### Dominated Strategies?

- No strategy is **strictly dominated**.
- But: Shooting to the middle is **never a best response** to any belief about the goalkeeper’s action.

### Visualizing Best Response

- Plotted expected payoffs against the probability the goalkeeper dives right.
- The Middle strategy is always strictly worse than Left or Right, regardless of goalkeeper behavior.
  
**Key Lesson**:
> Do **not** choose a strategy that is **never** a best response to any belief.

---

## Real-World Accuracy

### What’s Missing?

- **Player asymmetry**: Right-footed vs. left-footed preferences.
- **Goalkeeper staying in the middle**.
- **Shooter’s accuracy & power trade-off**.
- **Strategic variability**: Players may change decision mid-run-up.

### Real Data (Chiappori et al.)

| Shooter \ GK         | Natural Side | Unnatural Side |
|----------------------|--------------|----------------|
| Goalkeeper Natural   | 63.6%        | 94.4%          |
| Goalkeeper Unnatural | 89.3%        | 43.7%          |

- **Natural side**: Easier to kick across body (for right-footed players, this is left).
- **Middle strategy** becomes viable for powerful but less accurate shooters.

---

## Formal Definition of Best Response

### To a Strategy

Let `ŝᵢ` be player *i*'s strategy. It's a best response to opponent strategy `s₋ᵢ` if:

```

uᵢ(ŝᵢ, s₋ᵢ) ≥ uᵢ(sᵢ′, s₋ᵢ) ∀ sᵢ′

```

### To a Belief

Let `P` be a belief over opponents’ strategies. Then `ŝᵢ` is a best response if:

```

E\[uᵢ(ŝᵢ, s₋ᵢ) | P] ≥ E\[uᵢ(sᵢ′, s₋ᵢ) | P] ∀ sᵢ′

```

---

## Application: The Partnership Game

### Setup

- Two players in a firm choose **effort levels** `s₁` and `s₂` in [0, 4].
- **Profit function**:  
  `π = 4(s₁ + s₂) + B·s₁·s₂`
- **Payoffs**:
  - Player i gets:  
    `½π - sᵢ²`

### Best Response Functions

Solving:
```

∂u₁/∂s₁ = 2 + B·s₂ - 2s₁ = 0
⇒ s₁ = 1 + ½B·s₂

```
Symmetric for Player 2:
```

s₂ = 1 + ½B·s₁

```

### Solving for Equilibrium

By substitution:
```

s₁ = s₂ = 1 / (1 - B)

```

- **Nash Equilibrium**: The point where both best response functions intersect.

---

## Efficiency & Externalities

- **Is the equilibrium efficient?** No.
- **Why?** Each player bears the full cost of effort but only receives **half the benefit**—a classic **externality**.
- Leads to **under-provision of effort**.

---

## Conclusions

- **Never play strategies that are not best responses to any belief.**
- **Best responses** lead naturally to **Nash Equilibrium**.
- Nash Equilibrium can emerge from **iterative elimination of non-best responses**.
- In **partnerships**, profit-sharing leads to **suboptimal effort** due to externalities.

---

## References

1. [Best Response (Game Theory) - Wikipedia](https://en.wikipedia.org/wiki/Best_response)
2. [Penalty Kick (Soccer) - Wikipedia](https://en.wikipedia.org/wiki/Penalty_kick_(association_football))
3. [Nash Equilibrium - Wikipedia](https://en.wikipedia.org/wiki/Nash_equilibrium)
4. [Chiappori et al. (2002) AER paper on Penalty Kicks - JSTOR](https://www.jstor.org/stable/3083304) *(Yale access)*
5. [Externality - Wikipedia](https://en.wikipedia.org/wiki/Externality)
6. [Microeconomic Theory, Mas-Colell et al. (for Partnership Game model)](https://global.oup.com/ushe/product/microeconomic-theory-9780195073409)

---
---

# Understanding Game Theory: Best Responses, Dominated Strategies, and Nash Equilibrium

This study guide summarizes core game theory concepts with practical applications such as penalty kicks in soccer and collaborative partnerships in business.

---

## I. Core Concepts

### Best Response (BR)

* **Definition**: A strategy that maximizes a player's payoff, given their belief about what other players are doing.
* **Rationalisation**: Used to justify choices as optimal responses to others' actions.
* **Formal Definitions**:

  * To a strategy $s_{-i}$:
    $\hat{s}_i$ is a best response if:

$$
    u_i(\hat{s}_i, s_{-i}) \geq u_i(s'_i, s_{-i}) \quad \forall s'_i
$$

  * To a belief $P$:

$$
    E[u_i(\hat{s}_i, s_{-i})|P] \geq E[u_i(s'_i, s_{-i})|P] \quad \forall s'_i
$$

### Dominated Strategies

* **Definition**: A strategy always yielding strictly worse payoffs than another, no matter what opponents do.
* **Use**: Can be eliminated to simplify game analysis.
* **Limitation**: Not all games contain dominated strategies.

### Strategies that are Never a Best Response

* **Definition**: Strategies that are never optimal for any belief a player could hold about opponents.
* **Elimination**: These can be iteratively removed from the game, even if they’re not strictly dominated.

### Nash Equilibrium

* **Definition**: A strategy profile where no player has an incentive to deviate unilaterally.
* **Stability**: Each player's strategy is a best response to others’.
* **Graphical Representation**: Intersection of players’ best response functions (for continuous strategies).

---

## II. Applications and Examples

### The Penalty Kick Game (Soccer)

* **Players**: Kicker and Goalkeeper.
* **Kicker’s Strategies**: Shoot Left, Middle, or Right.
* **Goalkeeper’s Strategies**: Dive Left or Right.
* **Payoffs**: Represent scoring probabilities (e.g., 4 = 40%) and their negatives for the goalie.

#### Key Takeaways

* **No dominated strategies**.
* **"Shoot Middle"** is **never a best response** under any belief.
* **Advice**: Do not shoot middle unless under special conditions (e.g., highly skilled).
* **Model limitations**:

  * Ignores footedness, vertical placement, and goalie behavior like staying in the center.
  * Data quality issues (e.g., mixed league sources).

### The Partnership Game (Business/Study Groups)

* **Players**: Two agents (e.g., law firm partners).
* **Strategies**: Choose effort $s_1, s_2 \in [0,4]$
* **Profit Function**:

$$
  \pi = 4(s_1 + s_2) + B \cdot s_1 \cdot s_2
$$

* **Payoff Function for player i**:

$$
  u_i = \frac{1}{2}\pi - s_i^2
$$

* $B$: synergy/complementarity factor (0 ≤ B ≤ 1/4)

#### Key Takeaways

* **Best Response Functions**:

$$
  \hat{s}_1 = 1 + \frac{B}{2}s_2 \quad \text{and} \quad \hat{s}_2 = 1 + \frac{B}{2}s_1
$$

* **Nash Equilibrium**:

$$
  s_1^* = s_2^* = \frac{1}{1 - B}
$$

* **Efficiency**:

  * The equilibrium is inefficient due to **externalities**.
  * Each player under-contributes since they don’t internalize the full benefit.
* **Impact of B**: Lower B → lower equilibrium efforts (due to weaker synergy).

---

## III. Analytical Tools

### Graphical Analysis

* Used for discrete strategy games (e.g., penalty kick).
* Plot expected payoffs vs. belief probabilities to identify non-optimal strategies.

### Calculus for Continuous Strategies

* **Used in**: Games like the partnership model.
* **Steps**:

  * Apply **First Order Condition (FOC)**: Set derivative to zero.
  * Apply **Second Order Condition (SOC)**: Confirm maximum (negative second derivative).

---

## Quiz: Game Theory Applications

> *Answer in 2–3 sentences.*

1. **Define the concept of a "best response" in game theory.**
   A strategy that maximizes a player’s payoff given their belief about other players' strategies.

2. **Why is "shooting to the middle" never a best response?**
   Its expected payoff is always lower than Left or Right across all possible goalie behaviors.

3. **Main limitation of dominated strategies in the penalty kick game?**
   No strategy is strictly dominated, so the concept cannot simplify or solve the game.

4. **How does a payoff graph identify strategies that are never best responses?**
   If the expected payoff line is always below others, that strategy can never be optimal.

5. **Why use calculus in the partnership game?**
   Strategy choices are continuous; graphical analysis isn’t feasible for infinite options.

6. **What does parameter 'B' represent?**
   The degree of synergy—how joint effort boosts overall profit.

7. **Significance of best response intersection in the partnership game?**
   It's the **Nash Equilibrium**, where both players are simultaneously playing optimally.

8. **Why is effort inefficient at equilibrium?**
   Players don’t fully internalize the benefit of their effort due to shared profits.

9. **Effect of a decrease in B?**
   Lower synergy reduces the benefit of joint effort, leading to lower optimal contributions.

10. **Meaning of “playing a best response to each other”?**
    Each player is choosing their optimal strategy, assuming the other’s strategy remains fixed.

---

## Essay Questions

1. **Dominated vs. Never Best Response**:
   Compare these concepts and explain why “never best response” is more flexible analytically.

2. **Penalty Kick Game Analysis**:
   Describe players, strategies, and model insights. Evaluate limitations for real-world use.

3. **Calculus in the Partnership Game**:
   Explain the mathematical process for finding best responses and equilibrium.

4. **Efficiency in the Partnership Game**:
   Discuss the externality problem and how B affects efficiency.

5. **Game Structure and Tools**:
   Contrast analytical methods used for discrete (graphical) vs. continuous (calculus) games.

---

## Glossary of Key Terms

| Term                                                                   | Definition                                                             |
| ---------------------------------------------------------------------- | ---------------------------------------------------------------------- |
| **Best Response**                                                      | A strategy that maximizes payoff given a belief about other players.   |
| **Best Response Function**                                             | Shows optimal strategy for each possible action of opponents.          |
| **Complementarity**                                                    | Synergy from combined efforts in the partnership game.                 |
| **Continuum of Strategies**                                            | Infinite options over a range (e.g., effort level from 0 to 4).        |
| **Dominant Strategy**                                                  | Always strictly better, no matter what others do.                      |
| **Dominated Strategy**                                                 | Always strictly worse than another strategy.                           |
| **Expected Payoff**                                                    | Weighted average of payoffs based on opponent strategy probabilities.  |
| **Externality**                                                        | Benefit or cost affecting others not fully accounted for by the actor. |
| **First Order Condition (FOC)**                                        | Derivative equals zero; used to find extrema.                          |
| **[Game Theory](https://en.wikipedia.org/wiki/Game_theory)**           | Study of strategic decision-making.                                    |
| **Iterated Elimination of Never-Best-Response Strategies**             | Removing implausible strategies through successive logic.              |
| **[Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium)** | No player benefits from changing strategy unilaterally.                |
| **Payoff Function**                                                    | Describes the utility a player receives from the outcome.              |
| **Penalty Kick Game**                                                  | Model illustrating discrete strategic choices.                         |
| **Partnership Game**                                                   | Model of shared effort and profit with continuous strategy space.      |
| **Second Order Condition (SOC)**                                       | Sign of second derivative determines max or min.                       |
| **Strategy**                                                           | A complete action plan in a game.                                      |
| **Strategies that are Never a Best Response**                          | Cannot be optimal under any belief.                                    |
| **Synergy**                                                            | Additional value from joint effort. See: Complementarity.              |

---

## References

* [Best Response - Wikipedia](https://en.wikipedia.org/wiki/Best_response)
* [Dominated Strategies - Wikipedia](https://en.wikipedia.org/wiki/Strategic_dominance)
* [Nash Equilibrium - Wikipedia](https://en.wikipedia.org/wiki/Nash_equilibrium)
* [Penalty Kick in Football - Wikipedia](https://en.wikipedia.org/wiki/Penalty_kick_%28association_football%29)
* [Externality - Wikipedia](https://en.wikipedia.org/wiki/Externality)
* [Game Theory (Stanford Encyclopedia)](https://plato.stanford.edu/entries/game-theory/)

---
---

# Game Theory Q\&A: Best Response, Penalty Kicks, Partnership Game, and Nash Equilibrium

---

## 1. What is the fundamental concept of "best response" in game theory?

**Best response** is the strategy that maximizes a player's payoff given their beliefs about other players' strategies. These beliefs can be about a specific opponent action or a **probabilistic distribution** over possible actions. For example, in a [penalty kick](https://en.wikipedia.org/wiki/Penalty_kick_%28association_football%29) scenario, a kicker chooses the direction that best responds to the goalkeeper's expected dive direction to maximize the scoring chance.

[More on best response →](https://en.wikipedia.org/wiki/Best_response)

---

## 2. How does the penalty kick game illustrate best response and the elimination of non-optimal strategies?

In the penalty kick game:

* **Players**: Shooter and Goalkeeper.
* **Strategies**:

  * Shooter: Left, Middle, Right.
  * Goalkeeper: Left, Right.
* **Observation**: Shooting **Middle** is **never** a best response.

  * For any belief about the goalkeeper's dive, shooting Left or Right yields a higher expected payoff.
* **Conclusion**: Even though “Middle” is **not strictly dominated**, it can be eliminated using the concept of **never-best-response**, narrowing the game's strategy space.

---

## 3. What are the limitations of the initial penalty kick model?

### Simplifying assumptions:

* **Player asymmetry**: Ignores footedness (e.g., right-footed players prefer shooting left).
* **Goalkeeper behavior**: Assumes the goalie always dives, ignoring the option of staying in the center.
* **Kick characteristics**: Does not model trade-offs between power and placement.

### With real data and complexity:

* Shooting to the **Middle** might become viable for players with **powerful but less accurate kicks**.
* This changes the conclusion from “never shoot middle” to “consider context.”

---

## 4. How is best response applied in the "partnership game"?

In the **partnership game**:

* **Players**: Two individuals (e.g., law partners).
* **Strategy**: Choose effort $S_1$, $S_2 \in [0, 4]$.
* **Payoff**:

$$
  u_i = \frac{1}{2} [4(S_1 + S_2) + B \cdot S_1 \cdot S_2] - S_i^2
$$

### Best response analysis:

* Use **calculus** to differentiate and solve:

$$
  \hat{S}_1 = 1 + B \cdot S_2 \quad \text{and} \quad \hat{S}_2 = 1 + B \cdot S_1
$$

* These are each player’s **best response functions** showing how one’s optimal effort depends on the other’s effort.

---

## 5. What is the significance of the "synergy" term (B)?

* **B** represents **synergy** (also called **complementarity**) between partners’ efforts.
* When **B > 0**, joint efforts produce more profit than the sum of individual efforts.
* A **higher B**:

  * Steepens the best response curve.
  * Increases mutual responsiveness in effort decisions.
  * Encourages higher equilibrium efforts.

[More on synergy →](https://en.wikipedia.org/wiki/Complementarity_%28economics%29)

---

## 6. Explain the iterative elimination of non-best response strategies in the partnership game.

* Start with a **range of effort levels**.
* Eliminate levels that are **never a best response** to any strategy in the current set.
* Redefine the strategy space (the "box").
* Repeat: further eliminate strategies that are not best responses in the reduced box.
* **Result**: Converges to the **intersection of best response functions**, i.e., the **Nash Equilibrium**.

---

## 7. What is a Nash Equilibrium, and how is it identified in the partnership and number-choosing games?

### Definition:

A **[Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium)** is a set of strategies where each player’s choice is a **best response** to the others’. No one gains by deviating unilaterally.

### Partnership Game:

* Nash Equilibrium is at the **intersection** of the best response curves.
* $S_1^* = S_2^* = \frac{1}{1 - B}$

### Number-Choosing Game:

* Goal: Choose a number closest to **2/3 of the average**.
* Equilibrium: Everyone chooses **1**.

  * If all pick 1, average is 1 → 2/3 of average is 2/3 → 1 is the closest number.

---

## 8. Why do players in the partnership game exert inefficiently low effort at equilibrium?

### Key concept: **[Externality](https://en.wikipedia.org/wiki/Externality)**

* Each partner bears **full cost** of their own effort but gets only **half the benefit** (due to profit-sharing).
* Result: They **under-contribute** relative to the socially optimal effort level.
* **Inefficiency** arises even when **B > 0**, because private incentives do not align with collective welfare.

---

## References

1. [Best Response – Wikipedia](https://en.wikipedia.org/wiki/Best_response)
2. [Penalty Kick – Wikipedia](https://en.wikipedia.org/wiki/Penalty_kick_%28association_football%29)
3. [Nash Equilibrium – Wikipedia](https://en.wikipedia.org/wiki/Nash_equilibrium)
4. [Complementarity in Economics](https://en.wikipedia.org/wiki/Complementarity_%28economics%29)
5. [Externality – Wikipedia](https://en.wikipedia.org/wiki/Externality)

---
