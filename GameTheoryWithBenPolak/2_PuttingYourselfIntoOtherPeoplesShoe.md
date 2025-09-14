# Game Theory Lecture Notes — Professor Ben Polak (Yale ECON 159)

## Recap: From Outcomes to Payoffs
- An **outcome matrix** shows what happens (e.g., grades in Game 1), but that alone is not a game.  
- To make it a game, we need **payoffs**: numerical values representing what players actually care about.  
- With players, strategies, and payoffs defined, we have a **normal-form game**.

**Lessons so far:**
1. **Do not play a strictly dominated strategy.**  
2. **Put yourself in others’ shoes** to figure out their payoffs and predict their actions.

---

## Prisoner’s Dilemma in the Real World
Examples of situations with Prisoner’s Dilemma dynamics:
- **Joint projects** → each has an incentive to shirk, leading to poor outcomes.  
- **Price competition** → undercutting prices benefits one firm in the short term but drives down industry profits.  
- **Common resources** (e.g., overfishing, carbon emissions) → individuals/countries have incentives to overuse, causing long-term harm.  

**Key Point:**  
Communication alone cannot solve a Prisoner’s Dilemma. Remedies include:
- **Contracts or treaties** (changing incentives/payoffs).  
- **Regulation** (external enforcement).  
- **Repeated interaction** (cooperation sustained over time).  
- **Education** (changing values/payoffs — “Maoist strategy”).  

---

## Formal Ingredients of a Game
1. **Players** (e.g., students, firms, countries).  
2. **Strategies**: each player’s available actions.  
   - Notation: `s_i` (specific strategy of player *i*), `S_i` (set of possible strategies).  
   - A **strategy profile** (`s`) is a list of strategies chosen by all players.  
3. **Payoffs**: each player’s utility (`U_i(s)`), determined by the strategy profile.  

---

## Strict and Weak Dominance
- **Strict Dominance:**  
  Strategy `s_i` strictly dominates `s’_i` if it always gives a strictly higher payoff, regardless of what others do.  

- **Weak Dominance:**  
  Strategy `s_i` weakly dominates `s’_i` if it always does **at least as well**, and sometimes strictly better.  

**Lesson:** Rational players should avoid both strictly and weakly dominated strategies.

---

## Example: Hannibal and the Romans
- Hannibal (attacker) chooses between an **easy pass** and a **hard pass**.  
- Romans (defenders) choose which pass to defend.  
- Payoffs depend on how many battalions Hannibal brings in versus how many Romans destroy.  

**Analysis:**  
- For Hannibal, attacking through the easy pass **weakly dominates** the hard pass.  
- Anticipating this, Romans should defend the easy pass.  
- This illustrates **Lesson Four**: predict others’ strategies by considering their payoffs.

---

## Numbers Game (2/3 of the Average)
- Each student picked a number between 1 and 100.  
- Winner = closest to **2/3 of the class average**.  

### Reasoning Process
- Random average ≈ 50 → 2/3 ≈ 33.  
- If everyone reasons that way → average 33 → 2/3 ≈ 22.  
- Iterating further pushes toward **1**.  

### Key Insights
- Numbers above **67** are dominated (cannot win).  
- Eliminating dominated strategies step by step leads eventually to **1** as the rational prediction, **if common knowledge of rationality holds**.  

### Actual Results
- Class average: **13⅓**, so 2/3 average = **9**.  
- Winning choice: **9** (several students).  
- **1 was the modal choice**, but not the winner because not all players iterated reasoning to the limit.  

---

## Rationality and Knowledge
- **Rationality alone** rules out dominated strategies.  
- To eliminate further strategies, players must assume others are rational.  
- To keep iterating, players need **knowledge of knowledge** of rationality.  

This infinite chain of mutual understanding is called **common knowledge**.

**Example:** The “pink hat” demonstration shows that **mutual knowledge** (“each knows at least one hat is pink”) is not the same as **common knowledge**.

---

## Main Lessons
1. **Do not play dominated strategies** (strict or weak).  
2. **Put yourself in others’ shoes** to anticipate their rational play.  
3. **Rational choice depends on knowledge**: outcomes hinge on how much players know about each other’s rationality.  
4. **Common knowledge** is crucial for full rational prediction (e.g., converging to 1 in the numbers game).  

---

## References
- [Game Theory](https://en.wikipedia.org/wiki/Game_theory)  
- [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)  
- [Dominant Strategy](https://en.wikipedia.org/wiki/Dominant_strategy)  
- [Common Knowledge](https://en.wikipedia.org/wiki/Common_knowledge_(logic))  
- [Overfishing](https://en.wikipedia.org/wiki/Overfishing)  
- [Climate Change Game Theory](https://en.wikipedia.org/wiki/Climate_change_mitigation#Game_theory)  

---
---

# Quiz: Short Answer Questions with Answers

### 1. What is the fundamental difference between an "outcome matrix" and a "game" in the context of Game Theory?  
An **outcome matrix** shows only the results of different choices, such as grades or payoffs without values.  
A **game** adds payoffs to these outcomes, indicating what each player values or gains, making strategic analysis possible.

---

### 2. Define a "strictly dominated strategy." Why is it a fundamental lesson in Game Theory to avoid playing such strategies?  
A **strictly dominated strategy** always yields a strictly lower payoff than another strategy, regardless of what others do.  
It should be avoided because playing it is irrational—there is always a better alternative.

---

### 3. Explain the concept of "putting yourselves in others' shoes" in Game Theory. How does it relate to predicting opponents' actions?  
It means considering other players’ payoffs and incentives to anticipate their choices.  
By understanding what they value and how they reason, one can predict their likely strategies and respond optimally.

---

### 4. Briefly describe the core dilemma of the Prisoners' Dilemma game and provide one real-world example mentioned in the text.  
The **Prisoner’s Dilemma** occurs when individually rational choices (defection) lead to a worse collective outcome than cooperation.  
A real-world example is **price competition**, where firms undercut each other and reduce industry profits.

---

### 5. What are three suggested solutions to the Prisoners' Dilemma that involve "changing the payoffs" for players?  
1. **Contracts**  
2. **Treaties between countries**  
3. **Regulation**  
Each alters incentives so that cooperation becomes individually rational.

---

### 6. In the Numbers Game (2/3 of the average), what number would be the winning choice if all players assumed the average would be around 50 (random choice)?  
If the average were around 50, then two-thirds of that would be about **33**.  
Thus, 33 would win in that case.

---

### 7. The text discusses "iterated deletion of dominated strategies." Explain how this process can reduce the set of possible strategies in a game, using the Numbers Game as an illustration.  
First, strictly dominated strategies are removed.  
Then, in the reduced game, new strategies may become dominated and are eliminated as well.  
In the **Numbers Game**, numbers above 67 are initially dominated; once deleted, numbers between 46–67 become dominated, and so on.

---

### 8. What is the difference between "mutual knowledge" and "common knowledge" according to the lecture's example with the hats?  
- **Mutual knowledge**: everyone knows the fact (e.g., both TAs see a pink hat).  
- **Common knowledge**: everyone knows it, knows that others know it, and so on infinitely.  
In the hat example, mutual knowledge existed, but not common knowledge, since each TA did not know their own hat color.

---

### 9. Why did the average number chosen in the Numbers Game typically converge downwards over multiple years, and especially after discussion in class?  
Because students became more sophisticated in reasoning, and crucially, they recognized that **others were also becoming more sophisticated**.  
This deeper knowledge of rationality led them to choose progressively lower numbers.

---

### 10. The professor mentions that assuming common knowledge of rationality would lead to an optimal choice of 1 in the Numbers Game. Why is this assumption often unrealistic in real-world scenarios or even in a classroom setting?  
Because it requires an infinite chain of reasoning: *I know that you know that I know…* everyone is rational.  
In reality, players have limited reasoning depth and uncertainty about others’ rationality, so full common knowledge rarely holds.

---

# Essay Questions (No Answers Provided)

1. Analyse the role of "payoffs" in transforming an outcome matrix into a functional game in Game Theory. Discuss how different assumptions about player payoffs (e.g., self-interest vs. altruism) could fundamentally alter the strategic analysis and predicted outcomes of a game like the Prisoners' Dilemma.

2. Compare and contrast "strictly dominated" and "weakly dominated" strategies. Explain why the decision to avoid a weakly dominated strategy is considered more "subtle" and how the process of iterated deletion of dominated strategies relies on different levels of assumptions about players' rationality and knowledge of rationality.

3. Discuss the effectiveness of various solutions to the Prisoners' Dilemma, such as contracts, treaties, regulation, and education. For each solution, explain how it attempts to "change the payoffs" or alter incentives, and consider any limitations or challenges in its real-world application, drawing on examples from the text.

4. Using the Numbers Game (2/3 of the average) as your primary example, explain the concept of "common knowledge of rationality" and its implications for strategic decision-making. Why is common knowledge so difficult to achieve, and how do varying levels of knowledge about others' rationality influence the actual outcomes of games?

5. Critically evaluate the statement, "Communication per se will not get you out of a Prisoners' Dilemma." Discuss the underlying reasons for this claim and elaborate on what additional mechanisms or changes are necessary to foster cooperation in such scenarios, providing specific examples.

---

# Glossary of Key Terms

- **Outcome Matrix**: Table of possible results of player choices, without specifying preferences.  
- **Game**: Players, strategies, and payoffs combined into a formal structure.  
- **Normal-Form Game**: Matrix representation of a game.  
- **Payoffs**: The utility or benefit players aim to maximize.  
- **Players (i, j)**: Decision-makers in the game.  
- **Strategy (s_i)**: A specific choice for a player.  
- **Strategy Set (S_i)**: All strategies available to a player.  
- **Strategy Profile (s)**: A full set of chosen strategies, one for each player.  
- **s_-i**: The strategies of all players except player *i*.  
- **Strictly Dominated Strategy (s'_i)**: Always yields a worse payoff than another strategy.  
- **Weakly Dominated Strategy (s'_i)**: Never better and sometimes worse than another strategy.  
- **Prisoners' Dilemma**: A situation where rational choices create worse outcomes than cooperation.  
- **Iterated Deletion of Dominated Strategies**: Sequentially eliminating dominated strategies to simplify analysis.  
- **Rationality**: Players maximize payoffs given beliefs about others.  
- **Knowledge of Rationality**: Awareness that other players are rational.  
- **Common Knowledge**: Everyone knows a fact, knows that others know it, infinitely.  
- **Mutual Knowledge**: Everyone knows a fact, but without infinite regress.  

---

## References
- [Game Theory](https://en.wikipedia.org/wiki/Game_theory)  
- [Prisoner’s Dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)  
- [Dominated Strategies](https://en.wikipedia.org/wiki/Dominated_strategy)  
- [Common Knowledge](https://en.wikipedia.org/wiki/Common_knowledge_(logic))  
- [Price Competition](https://en.wikipedia.org/wiki/Competition_(economics))  
