
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
---

# Game Theory: Iterative Deletion & Median-Voter Theorem Study Guide

---

## I. Iterative Deletion of Dominated Strategies

### A. Definition and Process

* **[Dominated Strategy](https://en.wikipedia.org/wiki/Strategic_dominance)**: A strategy that always yields a lower payoff than another, regardless of opponents' choices.
* **Strictly Dominated Strategy**: Always yields a strictly lower payoff than another.
* **Iterative Deletion**:

  1. Identify all dominated strategies for all players.
  2. Delete these strategies from the game.
  3. Re-evaluate the simplified game for newly dominated strategies.
  4. Repeat until no further deletions are possible.

### B. Key Concepts and Considerations

* **[Rationality](https://en.wikipedia.org/wiki/Rational_choice_theory)**: Assumes players act to maximize their own payoff.
* **Common Knowledge of Rationality**: Players believe all others are also rational and apply the same logic.
* **Convergence**: The process can converge to a unique solution.
* **Limitations**:

  * Can lead to excessive complexity ("over-thinking").
  * Cannot proceed if no dominated strategies exist.

---

## II. Application: The Median-Voter Theorem in Politics

### A. Model Setup

* **Players**: Two political candidates.
* **Strategies**: Positions on a 1–10 political spectrum.
* **Voters**:

  * Uniformly distributed (10% at each point).
  * Vote for the candidate closest to their position.
* **Tie-Breaking**: Voters split evenly if candidates are equidistant.
* **Payoffs**: Candidates aim to maximize their vote share.

### B. Applying Iterative Deletion

* **Round 1**:

  * Strategy 1 is dominated by 2.
  * Strategy 10 is dominated by 9.
* **Subsequent Rounds**:

  * 2 and 9 become dominated by 3 and 8, and so on.
* **Convergence**: Ends at positions **5 and 6**, representing the political center.

### C. Median-Voter Theorem

* **Prediction**: Candidates converge near the **[median voter](https://en.wikipedia.org/wiki/Median_voter_theorem)**.
* **Real-World Examples**:

  * [Kennedy–Nixon elections](https://en.wikipedia.org/wiki/1960_United_States_presidential_election)
  * [Clinton (1992)](https://en.wikipedia.org/wiki/Bill_Clinton_presidential_campaign,_1992)
* **Economic Analogy**:

  * **[Hotelling's Model](https://en.wikipedia.org/wiki/Hotelling%27s_law)**: Firms cluster to maximize consumer base, similar to politicians clustering at the center.

### D. Strengths and Weaknesses

#### Criticisms:

* **Uniform Distribution**: Real voter preferences are not evenly spread.
* **Voter Turnout**: Not all voters vote.
* **Election Stages**: Ignores primaries and runoffs.
* **Multidimensional Politics**: Ignores issues beyond left–right spectrum.
* **Number of Candidates**: Only two candidates assumed.
* **Candidate Commitment**: Ignores credibility and past record.

#### Importance of Modelling

* **Abstraction**: Models simplify reality to test core intuitions.
* **Enrichment**: Starting with simple models helps build towards more complex and realistic ones.

---

## III. Introduction to Best Response Strategies

### A. Definition

* **[Best Response](https://en.wikipedia.org/wiki/Best_response)**: The strategy that maximizes a player's payoff given the opponent's action.

### B. Limitations of Iterative Deletion

* Some games lack dominated strategies, making iterative deletion inapplicable.

### C. Best Response with Uncertainty

* **Expected Payoff**:

$$
  \text{Expected Payoff} = \sum (\text{Payoff}) \times (\text{Probability})
$$

* **Graphical Tool**: Plot expected payoffs vs. probability of opponent's strategy to find the **best response**.
* **Rationalization**: Players justify choices based on beliefs about opponent actions.

### D. Next Steps

* Best response logic applies to more complex strategic scenarios like **[penalty kicks in soccer](https://en.wikipedia.org/wiki/Game_theory_in_football_%28soccer%29)**.

---

## Quiz

### Short Answer Questions

1. **Define "iterative deletion of dominated strategies."**
   Progressive elimination of inferior strategies to simplify and solve a game.

2. **Assumption about rationality in iterative deletion?**
   All players are rational and aware that others are rational too.

3. **Why are positions 1 and 10 dominated in the political model?**
   They consistently yield worse outcomes than choosing positions closer to the center.

4. **Core prediction of the Median Voter Theorem?**
   Candidates move toward the center to capture the largest voter share.

5. **Historical example of the theorem in practice?**
   Kennedy–Nixon elections or Clinton’s 1992 campaign.

6. **Hotelling's model analogy?**
   Firms cluster in the middle to maximize consumer base — like politicians vying for the median voter.

7. **Two criticisms of the basic political model?**
   Assumes uniform voter distribution and a two-candidate race.

8. **Why is lack of commitment a problem in the model?**
   Candidates may not be trusted; voters consider credibility.

9. **What is a "best response" in game theory?**
   The optimal strategy given opponents' choices.

10. **Why is iterative deletion insufficient in some games?**
    If no strategies are dominated, the method cannot proceed.

---

## Essay Questions

1. Evaluate the use of iterative deletion in elections using the Median Voter Theorem.
2. Discuss the educational benefit of starting with simplified models in game theory.
3. Compare iterative deletion in abstract vs. political games. What makes political models uniquely suited or ill-suited?
4. Identify other limiting assumptions in the Median Voter Theorem for modern politics.
5. Explain how best response strategies offer more flexibility in uncertain games.

---

## Glossary of Key Terms

| Term                                                                           | Definition                                                                     |
| ------------------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| **Best Response**                                                              | A strategy that maximizes a player's payoff given opponents' choices.          |
| **Dominated Strategy**                                                         | Yields lower payoffs than another strategy regardless of others’ moves.        |
| **Expected Payoff**                                                            | Weighted average of possible payoffs based on opponents’ action probabilities. |
| **[Game Theory](https://en.wikipedia.org/wiki/Game_theory)**                   | Mathematical study of strategic interactions.                                  |
| **[Hotelling's Model](https://en.wikipedia.org/wiki/Hotelling%27s_law)**       | Firms locate centrally to maximize market capture.                             |
| **Iterative Deletion**                                                         | Repeatedly removing dominated strategies from a game.                          |
| **[Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)** | Candidates converge toward the median voter’s position.                        |
| **Payoffs**                                                                    | The numerical representation of outcomes in a game.                            |
| **[Political Spectrum](https://en.wikipedia.org/wiki/Political_spectrum)**     | A range representing political ideologies from left to right.                  |
| **Rationality**                                                                | Assumes players act to maximize their utility.                                 |
| **Strictly Dominated Strategy**                                                | Always yields strictly lower payoffs than another.                             |
| **Strategies**                                                                 | Complete action plans specifying a player's moves.                             |
| **Uniform Distribution**                                                       | Equal probability or voter share across spectrum positions.                    |

---
---

# Game Theory: Iterative Deletion, Median Voter Theorem & Best Response – Q\&A Summary

---

## What is *iterative deletion of dominated strategies*?

**Iterative deletion of dominated strategies** is a predictive method in [game theory](https://en.wikipedia.org/wiki/Game_theory). It involves:

* **Eliminating dominated strategies** — strategies that are always worse than another strategy, regardless of what opponents do.
* **Re-evaluating the game** after each deletion to find new dominated strategies in the reduced game.
* **Repeating this process** until no more strategies can be deleted.

The goal is to isolate rational strategies that players are expected to choose, assuming all players are rational and know others are too.

[Learn more →](https://en.wikipedia.org/wiki/Strategic_dominance)

---

## How does *iterative deletion* apply to the political model?

In a simplified political election model:

* **Candidates** choose positions on a 1–10 spectrum (left to right).
* **Voters** are uniformly distributed and vote for the closest candidate.
* **Payoffs**: candidates want to maximize their vote share.

**Process**:

1. **Round 1**:

   * Position 1 is strictly dominated by 2.
   * Position 10 is dominated by 9.
2. **Round 2**:

   * After removing 1 and 10, position 2 is now dominated by 3, and 9 by 8.
3. **Subsequent rounds**:

   * Iterative deletion continues until only positions **5 and 6** remain.

**Conclusion**: Candidates converge near the center of the spectrum.

---

## What is the *Median Voter Theorem* and its significance?

The **[Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)** predicts:

> In a two-candidate election with voters on a spectrum, candidates will position themselves near the median voter's preferences to win.

**Significance**:

* Explains why centrist policies dominate in two-party systems.
* Suggests that **median voters** (those in the middle) decide elections.
* Seen in U.S. history (e.g., Kennedy-Nixon, Clinton 1992 campaigns).

---

## What are some economic applications of the Median Voter Theorem?

The same logic applies to economics, specifically in **[Hotelling’s model](https://en.wikipedia.org/wiki/Hotelling%27s_law)**:

* **Firms (e.g., gas stations)** tend to cluster in central locations to maximize customer capture.
* **Clustering** prevents competitors from out-positioning them, just like political candidates crowding the center.

---

## What are the main criticisms or limitations of the Median Voter Theorem?

### Limitations include:

* **Non-uniform voter distribution**: Real voters aren’t evenly spread.
* **Voter turnout**: Model assumes everyone votes.
* **Election stages**: Ignores primary elections.
* **Multidimensional issues**: Politics isn't just left vs. right.
* **More than two candidates**: Third-party options change dynamics.
* **Commitment issues**: Candidates may not be believed if their declared position doesn’t match their track record.

---

## How are simplified models like the Median Voter Theorem useful despite their limitations?

Simplified models serve to:

* Capture **core intuitions** (e.g., convergence to the center).
* Provide a foundation for **building more complex models**.
* Allow analysts to **test the robustness** of conclusions under changing assumptions.
* Promote a **deeper understanding** by analyzing why and when deviations occur.

---

## What is a *best response* in game theory?

A **[best response](https://en.wikipedia.org/wiki/Best_response)** is:

> The strategy that maximizes a player's payoff given the strategies chosen (or believed to be chosen) by other players.

Unlike dominated strategies, best responses depend on specific beliefs or actions of the opponent.

Example:

* If your opponent chooses Left, your best response might be "Up."
* If they choose Right, your best response might be "Middle."

---

## How can *best response* analysis be visualized and used?

### Visualization:

1. **Expected payoff graph**: Plot expected payoffs for each strategy against the probability of an opponent choosing a certain move.
2. **Highest line wins**: For any belief about opponent behavior, the strategy with the highest payoff line is the best response.

### Justification:

Players can rationalize their choice by stating:

> “I believed the opponent was equally likely to choose Left or Right, and under that belief, 'Down' was my best response.”

### Example:

* Probability opponent chooses Right = ½
* Compute expected payoffs:

  * Up: 0.5×Payoff1 + 0.5×Payoff2
  * Middle: same
  * Down: same
* Compare and choose the best.

---

## References

* [Game Theory](https://en.wikipedia.org/wiki/Game_theory)
* [Strategic Dominance](https://en.wikipedia.org/wiki/Strategic_dominance)
* [Median Voter Theorem](https://en.wikipedia.org/wiki/Median_voter_theorem)
* [Hotelling's Law](https://en.wikipedia.org/wiki/Hotelling%27s_law)
* [Best Response](https://en.wikipedia.org/wiki/Best_response)

---
