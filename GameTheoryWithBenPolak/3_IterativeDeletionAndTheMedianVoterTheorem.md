
# Iterative Deletion of Dominated Strategies (IDDS)

## Concept Overview

**Iterative Deletion of Dominated Strategies (IDDS)** is a fundamental method in [game theory](https://en.wikipedia.org/wiki/Game_theory). It involves successively removing strategies that are inferior (dominated) for each player, based on rational expectations about opponents' behavior.

* **Strictly dominated strategy**: A strategy is strictly dominated if another strategy yields a better outcome regardless of what opponents do.
* **Iterative process**: Once a dominated strategy is deleted, it may cause other strategies to become dominated in subsequent rounds.

## Example: Political Spectrum Game

A classic example used in political science involves two candidates choosing positions on a political spectrum (from 1 to 10):

* **Players**: Two political candidates.
* **Strategies**: Positions 1 to 10 on the spectrum.
* **Assumptions**:

  * 10% of voters are located at each position.
  * Voters choose the closest candidate.
  * If equidistant, they split their votes evenly.
  * Candidates aim to **maximize their vote share**.

### Analysis of Dominated Strategies

1. **Initial dominance**:

   * Strategy 1 is strictly dominated by 2.
   * Strategy 10 is strictly dominated by 9.
   * These are symmetric arguments.

2. **Iterative Deletion**:

   * Once 1 and 10 are removed, 2 is dominated by 3, and 9 by 8.
   * This process continues until only strategies **5 and 6 remain**.

### Implication: Median Voter Theorem

This process leads to the **Median Voter Theorem**, which states that:

> Political candidates tend to converge toward the median voter’s position to capture the majority of votes.

This behavior is observed in:

* [1960 Kennedy vs. Nixon election](https://en.wikipedia.org/wiki/1960_United_States_presidential_election)
* [1992 Bill Clinton campaign](https://en.wikipedia.org/wiki/Bill_Clinton_presidential_campaign,_1992)

The same concept applies in **economics**:

* Firms may cluster products (e.g. gas stations) to attract the largest segment of customers, known as [Hotelling's Law](https://en.wikipedia.org/wiki/Hotelling%27s_law).

---

## Limitations of the Model

### Key Assumptions That May Not Hold in Reality:

* **Uniform voter distribution** — Voters aren't evenly spread.
* **Single-issue spectrum** — Real issues are multidimensional (economy, healthcare, foreign policy).
* **Two-candidate system** — Real elections often include third-party candidates.
* **Perfect commitment** — Candidates might not be trusted to stick to their declared position.
* **Voter turnout** — Model assumes all voters vote.
* **No primaries considered** — In reality, primary elections shift candidate positions.
* **Non-policy factors** — Charisma, reputation, and media influence matter too.

---

# Transition: From Deletion to Best Response

To analyze more complex games, we introduce **Best Response Analysis**:

* The best response is the strategy that yields the highest payoff, given a belief about the opponent's choice.
* If no strategies are dominated, this method allows us to still make predictions about behavior.

---

## Example: Best Response in a Payoff Matrix

Two-player matrix game:

| Player I | Left   | Right  |
| -------- | ------ | ------ |
| Up       | (5, 1) | (0, 2) |
| Middle   | (1, 3) | (4, 1) |
| Down     | (4, 2) | (2, 3) |

### Expected Payoff Analysis

Assuming Player I believes Player II will choose:

* **Left with 100% probability** → Best response: **Up**
* **Right with 100% probability** → Best response: **Middle**
* **Equal probability (½ Left, ½ Right)** → Best response: **Down**

This leads to plotting **expected payoffs** as a function of the probability Player II chooses "Right".

---

## Visual Tool: Best Response Diagram

* **X-axis**: Probability that Player II chooses "Right".
* **Y-axis**: Expected payoff for Player I.
* Each strategy’s expected payoff is plotted as a line.
* The **upper envelope** of these lines determines the **best response** at each belief level.

---

# Applications and Future Topics

* **Penalty kicks in soccer**: The best response framework helps understand mixed strategy equilibria.
* **Model refinement**: Add complexity (e.g., voter turnout, multidimensional policy issues) to test robustness.

---

## References

* [Game Theory](https://en.wikipedia.org/wiki/Game_theory)
* [Dominated Strategies](https://en.wikipedia.org/wiki/Strategic_dominance)
* [Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)
* [Hotelling's Law](https://en.wikipedia.org/wiki/Hotelling%27s_law)
* [Expected Value](https://en.wikipedia.org/wiki/Expected_value)
* [Anthony Downs (1957)](https://en.wikipedia.org/wiki/Anthony_Downs)
* [Harold Hotelling (1929)](https://en.wikipedia.org/wiki/Harold_Hotelling)

---
