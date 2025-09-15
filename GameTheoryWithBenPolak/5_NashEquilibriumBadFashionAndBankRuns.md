
## Key Ideas from Polak’s Lecture

### Formal Definition of Nash Equilibrium (NE)

* A strategy profile
  
$$
 (S_1^{\ *}, S_2^{\ *}, \dots, S_M^{\ *})
$$ 

(i.e. one strategy for each player) is a **Nash Equilibrium** if for *every player* $i$, their strategy

$$
S_i^{\ *}
$$ 

is a *best response* to the other players’ strategies 

$$
    S_{-i}^{\ *}
$$

.

* Equivalently: given what everyone else is doing, no player can unilaterally deviate and get a strictly better payoff.

### Motivations / Why NE matters

1. **No regrets**: If the profile is NE, once you observe what others did, you can look back and say “I couldn’t have done better, given what they did.”
2. **Self-fulfilling beliefs**: If everyone believes “everyone else will play according to this NE”, then best responses lead them to actually play that NE.
3. Under repeated play or learning, people often move toward an equilibrium in coordination settings (as observed in experiments).

He emphasizes that NE is *not* a guarantee of what will actually happen in every one-shot game among humans. People sometimes deviate, have incorrect beliefs, or are influenced by fairness, risk, etc.

---

## Example 1: 2-player 3×3 Game

* Players: P1 (Up / Middle / Down), P2 (Left / Center / Right).
* Payoffs given in a matrix.
* Method: Find P1’s best response to each strategy of P2; find P2’s best response to each of P1’s; then look for where best responses coincide.
* NE found: **(Down, Right)** is the unique Nash Equilibrium in that game.

Observation: All strategies are best responses *to something*, so no dominated or never-best-response strategies can be eliminated in that game — yet NE still narrows things further.

---

## Example 2: Another 3×3 Game

* Similar setup, but different payoffs.
* Again, find best responses for each side.
* NE found: **(Middle, Center)** is a Nash Equilibrium.

Important note: Best responses need not be unique — there can be ties.

---

## Relating NE to Dominance

* Example: Prisoner’s Dilemma. The “defect” strategy (call it β) is *strictly dominated* by “cooperate” (call it α).

* In PD, the unique NE is (α, α) — same as you’d get by deleting strictly dominated strategies.

* **Key point**: Any *strictly dominated* strategy **cannot** be part of a Nash Equilibrium (because a strictly dominated strategy is never a best response).

* However, *weak domination* is trickier: deleting weakly dominated strategies can sometimes lead you to throw away equilibria or get odd predictions.

Example shown: a 2×2 game where one player has up/down, the other left/right with payoffs such that some strategies are weakly dominated (or at least weakly worse), yet there are multiple Nash Equilibria, including ones that look “silly” or less plausible.

---

## Example 3: The Investment Game (Many Players; Simple Strategies)

* Each player (in class) chooses: **Invest** \$10 or **Don’t Invest**.
* Payoffs: If you invest, you get net +\$5 *only if* at least **90%** of the class invests; otherwise you lose your investment (i.e. negative payoff). If you don’t invest, you get 0.
* No communication allowed (cheap talk in some rounds later, but that comes after initial play).

**Nash Equilibria** in this game:

* *Everyone invests.* If everyone invests, then each is a best response: as everyone else is investing, investing nets \$5, which is better than not investing (0).
* *No one invests.* If no one invests, then investing is bad (you'd almost certainly fail to reach 90%), so no one investing is also a best response for each individual, given the others.

So there are **two pure-strategy Nash equilibria**: “all invest” and “none invest.”

**Observed behavior in class**:

* In early rounds, many people did not invest.
* Over repeated play, behavior converged toward the “none invest” equilibrium (the “bad” equilibrium), even though “all invest” is strictly better for everyone.

This illustrates a coordination problem: multiple equilibria, where only one is good in the Pareto-sense, but the group ends up at the worse equilibrium due to beliefs, risk, or lack of confidence that others will invest.

---

## Concepts & Terminology Introduced / Emphasized

* **Coordination Game**: Games in which players benefit from choosing the same or matching strategies, and where there can be multiple Nash equilibria. (“Invest / Not Invest” is one.)
* **Pareto dominance**: One equilibrium is strictly better for all players than another equilibrium.
* Example of **focal point / communication / beliefs** helping to select one equilibrium over another. Patrick’s speech in class helped shift expectations and raise investment levels.

---

## Some Clarifications / Additional Thoughts

* **Strict vs Weak Dominance**: Strictly dominated strategies can *never* be in a NE; weakly dominated might sometimes be part of a NE because they might still be a best response in some beliefs (even if weakly).

* **Multiple Nash Equilibria**: Having more than one possible equilibrium means we often need extra structure (beliefs, focal points, risk dominance, communication) to predict which equilibrium players “choose”.

* **Risk dominance** vs **payoff dominance**: In coordination games, one equilibrium may yield higher payoffs, but another may be safer (less risky if you’re unsure about others). People sometimes gravitate to the less risky even if payoff is lower, especially without communication.

* **Pre-play communication (“cheap talk”)** can help choose the “better” equilibrium in coordination games, even without enforceable commitments. This was illustrated in class when Patrick’s speech shifted many toward “invest.”

---

## Connection with Academic Literature

* Coordination games are a classic concept in game theory. They involve multiple Nash Equilibria and the importance of how players form expectations. ([Wikipedia][1])
* The role of **communication** before play is well studied: “cheap talk” can help select favorable equilibria. One well-known paper is *“Communication, coordination, and Nash equilibrium”* by Joseph Farrell (1988). ([ScienceDirect][2])
* Other ideas: focal points (Schelling), risk dominance, payoff dominance. ([Wikipedia][1])

---

- https://en.wikipedia.org/wiki/Coordination_game "Coordination game"
- https://www.sciencedirect.com/science/article/pii/0165176588901723 "Communication, coordination and Nash equilibrium"
---
---

# Nash Equilibrium and Coordination Games: Study Guide

---

## I. Core Concepts of Nash Equilibrium

### A. Definition and Identification

* **Formal Definition**
  A strategy profile $(S_1^*, S_2^*, \dots, S_M^*)$ for $M$ players is a **Nash Equilibrium (NE)** if for every player $i$, $S_i^*$ is a best response to the strategies chosen by all the other players $S_{-i}^*$. In other words, no player can improve their payoff by unilaterally deviating.

* **Best Response**
  A strategy for player $i$ that maximises their payoff, given a fixed strategy profile of the other players.

* **How to Find Nash Equilibria in Simple Games**

  1. For each possible strategy of the other player(s), find each player’s best responses.
  2. Mark or identify where the best responses of all players coincide. Those coincide‐points are NE.
  3. Use “guess and check” when there are many players but few strategy options per player. You guess a profile, then check whether anyone would want to deviate.

### B. Motivations and Interpretations of Nash Equilibrium

* **No Regrets**
  Once the game is played and you see what the others did, you don’t look back and wish you had chosen something else—given what others did, you couldn’t have done better.

* **Self‑Fulfilling Beliefs**
  If every player believes the others will play some NE profile, then each’s best response is to play their part of that profile. Thus beliefs that everyone expects that NE lead to that NE being played.

* **Convergence of Play**
  Repeated play, experiments, or dynamics often cause behavior to move toward a Nash Equilibrium over time—even if initial choices are off the equilibrium.

### C. Relationship with Dominance

* **Strictly Dominated Strategies**
  A strictly dominated strategy is one that is worse than another strategy for every possible combination of other players’ strategies. Such a strategy *cannot* be part of a Nash Equilibrium, since a NE requires that each strategy be a best response to something.

* **Weakly Dominated Strategies**
  These are more subtle. A weakly dominated strategy can sometimes still be part of a NE (because “weak” dominance allows equality in some cases). Eliminating weakly dominated strategies can lead to losing some equilibria or retaining "silly" equilibria; thus, it is less secure to rely on weak domination than strict domination.

---

## II. The Investment Game: Application of Nash Equilibrium

### A. Game Structure and Payoffs

* Players: Many (e.g., a class of students).

* Strategies: Each player chooses either **Invest** (\$10) or **Don’t Invest** (\$0).

* Payoffs:

  * If you don’t invest: payoff = \$0.
  * If you invest:
      • If **≥ 90%** of players invest → net profit \$5 (gross \$15 minus the \$10 cost).
      • If **< 90%** invest → you lose your \$10.

* Key rule: No communication (initially), so players don’t know what fraction will invest except by beliefs or observations in repeated rounds.

### B. Identifying Nash Equilibria in the Investment Game

There are **two pure‐strategy Nash Equilibria**:

1. *Everyone Invests.*
   If every other player invests (so you believe ≥ 90% will), then investing yields +\$5 vs 0 if you don’t – so the best response is to invest. No one wants to deviate.

2. *No One Invests.*
   If everyone expects fewer than 90% to invest (or sees nobody investing), then investing would lead to a loss, so the best response is to **not invest**. Again, no one wants to deviate.

### C. Bad Equilibria & Coordination Problems

* **Pareto Dominance**
  The “Everyone Invests” equilibrium strictly Pareto dominates “No One Invests”—everyone is better off in “Everyone Invests.”

* **Convergence to Bad Equilibrium**
  In practice (class experiments), behavior tends to converge toward “No One Invests” if initial investment levels are below the 90% threshold. Once people believe fewer will invest, it becomes safer not to invest, and the bad equilibrium becomes a self‐fulfilling outcome.

* **Coordination Game** vs **Prisoner’s Dilemma**

  * In coordination games, there are multiple equilibria; players benefit if they coordinate on certain strategies. The “good” strategy (invest) is only a best response if enough others choose it.
  * This differs from Prisoner’s Dilemma, where there is a single strictly dominant strategy for each player (defect) regardless of what others do.

* **Role of Communication**
  Even cheap, non‐binding communication (Patrick’s speech, discussions) can shift beliefs and help everyone coordinate on a more desirable equilibrium. This is something you often cannot do in Prisoner’s Dilemma to achieve better outcomes, because the dominant strategy structure locks players into defection.

---

## III. Real‑World Examples of Coordination Games

* Choosing where to meet: which party, which bar, or what location.
* Technology / industry standards: software platforms, TV standards, network compatibility.
* Fashion / popular culture: trends, what’s “in.”
* Economic systems: stock exchanges, network effects (e.g., everyone using one software so it's useful).
* Bank runs: confidence vs panic equilibria.
* Political bandwagons: candidate selection in primaries.

---

## IV. Quiz Questions

Here are some useful questions (with answers hidden) to test understanding. Try to answer in 2–3 sentences each.

1. Define Nash Equilibrium formally, including the concept of a "best response."
2. Explain the “no regrets” motivation for Nash Equilibrium. Why is it significant?
3. How do “self‑fulfilling beliefs” relate to Nash Equilibrium?
4. Distinguish between strictly dominated and weakly dominated strategies. How do they each relate to Nash Equilibrium?
5. In the Investment Game, describe the two main Nash Equilibria.
6. Why is the “No One Invests” equilibrium considered “bad” even though it is a Nash Equilibrium?
7. Why is the Investment Game a coordination game, and not a Prisoner’s Dilemma?
8. What role can communication play in a coordination game, and how does this differ from a Prisoner’s Dilemma?
9. Give a real‑world problem involving coordination (in technology or standards). Identify players, strategies, and possible equilibria.
10. Describe a “bank run” as a coordination game, including its equilibria, and discuss what might move people from a bad to a good equilibrium.

---

## V. Additional Notes & Tips

* **Equilibrium Selection**: When there are multiple Nash equilibria, additional criteria may help pick which one is “likely” (e.g., risk dominance, payoff dominance, focal points, convention, communication).

* **Repeated Play & Learning**: Many games, when repeated, allow players to observe outcomes, adjust beliefs, and tend to move toward equilibria. But the path (initial conditions, beliefs) matters a lot.

* **Expectations / Beliefs**: Much of coordination depends on what you believe others will do. Even if the better equilibrium exists, if your beliefs are misaligned, you may settle into a worse one.

* **Dominance arguments** are powerful, especially strict dominance, but note their limitations. Weak dominance and never‐best‐response arguments can help, but must be used carefully.

---
---


### 1. What is a Nash Equilibrium, and how is it formally defined?

A **Nash Equilibrium (NE)** is a strategy profile — that is, one strategy chosen for each player in a game — such that no single player can improve her payoff by unilaterally changing her strategy, given that all the other players stick to their strategies in that profile.

Formally: A profile 
A strategy profile

$$
(S_1^{\ *}, S_2^{\ *}, \dots, S_M^{\ *})
$$

is a **Nash Equilibrium** if, for every player \( i \),

$$
u_i(S_i^*, S_{-i}^{\ *}) \ge u_i(s_i, S_{-i}^{\ *}) \quad \text{for all strategies } s_i \text{ of player } i.
$$



Here $S_{-i}^*$ denotes the strategies chosen by all players *other than* $i$.

---

### 2. What are the primary motivations for studying Nash Equilibrium?

* **No Regrets**: If the profile is a NE, then after play, no player wishes they had deviated — given what others did, they did as well as possible. This gives the outcome a sense of stability and rational justification.

* **Self‑fulfilling Beliefs**: If each player believes that all others will play their part of a particular NE, then each has an incentive to play their part (because it is a best response to that belief). Thus beliefs about others can lead to NE being realized.

* **Predictive Power / Convergence**: In many settings (experiments, repeated play, learning dynamics), behavior tends to gravitate toward Nash Equilibria. So even if players don’t compute NE explicitly, their actions often end up close to it.

* **Self‑enforcing Agreements**: In coordination or social interaction games, a NE often serves as a kind of “agreement” that does not require external enforcement: everyone’s interest is aligned with sticking to the equilibrium once they expect it.

---

### 3. How does Nash Equilibrium relate to the concept of dominant strategies?

* A **strictly dominant strategy** is one that yields a strictly higher payoff than any other strategy for a player, *no matter what* the other players do.

* If a player has a strictly dominated strategy, that strategy *can never* be part of a Nash Equilibrium, because in equilibrium each player’s strategy must be a best response to others’ strategies.

* **Weakly dominated strategies** are more subtle: a weakly dominated strategy does not always give strictly lower payoff (sometimes it gives equal payoff). Such strategies *can* appear in Nash Equilibria. Deleting weakly dominated strategies can sometimes remove potential equilibria or lead to losing plausible outcomes.

So: strict dominance → safe to eliminate; weak dominance → more care needed.

---

### 4. How are Nash Equilibria found in games?

* **Small, discrete games**:

  1. For each possible strategy of the other players, compute each player’s best response(s).
  2. Mark (or circle / highlight) those best responses in the payoff matrix.
  3. The cells where *all* players are playing their best responses are Nash Equilibria.

* **Larger/multi‑player games with few strategies**:
  Use guess-and-check: pick a candidate profile, check whether any player can profitably deviate. If none can, it’s a NE. If someone can, discard it.

* In continuous strategy games, often best response functions are derived (via calculus or optimization) and you look for intersections of those functions.

---

### 5. Can a game have more than one Nash Equilibrium? If so, what are the implications?

Yes, many games admit multiple Nash Equilibria.

**Implications:**

* **Predictive Ambiguity**: Which equilibrium will actually be played may depend on beliefs, expectations, history, focal points, or conventions, rather than just payoffs.

* **Coordination Problems**: Players must coordinate not just on what to do, but on what *others believe* they will do. If beliefs are misaligned, they might coordinate on a suboptimal equilibrium.

* **Pareto Ranking**: Some equilibria may be strictly better for all players (Pareto dominant) than others, yet the game might end up in a worse equilibrium because players do not coordinate or have incorrect beliefs.

* **Equilibrium Selection**: Additional criteria (risk dominance, payoff dominance, evolutionary stability, etc.) are often introduced in literature to suggest which equilibrium seems more plausible in practice.

---

### 6. What is a "coordination game," and what makes it distinct from a Prisoner’s Dilemma?

* A **coordination game** is one where:

  1. Players benefit if they coordinate their strategies (e.g. many prefer to choose the same action or complementary actions).
  2. There are typically *multiple Nash Equilibria*, and some of them are better for everyone than others.
  3. Which equilibrium is played often depends on beliefs, expectations, communications, or conventions.

* Distinction from **Prisoner’s Dilemma**:

  * In a Prisoner’s Dilemma, each player has a *strictly dominant strategy* (e.g. defect) that does better regardless of what the opponent does. The unique NE is the suboptimal outcome that arises from both playing their dominant strategy.

  * In coordination games, there is *no* strictly dominant strategy. What is best for you depends on what you expect others to do. So coordination games allow for the possibility of better outcomes if players can align their beliefs.

---

### 7. What are some real-world examples of coordination problems and their consequences?

* **Technology / Industry Standards**: E.g. different software platforms, or TV standards (HDTV). If people pick incompatible standards, the product is less useful. Might end up with a standard that everyone uses, but possibly one that’s not the best technically.

* **Bank Runs**: Two equilibria — one “good” where everyone trusts the bank and keeps deposits, one “bad” where panic leads everyone to withdraw, potentially causing a collapse.

* **Stock Exchanges / Networks**: Which platform to use, which communication protocol, which social media network, etc. The more people adopt a platform/protocol, the more valuable it is.

* **Social Gatherings / Party Locations**: If people don’t coordinate, very few attend; if everyone believes many will come, it can be a big success.

* **Fashion Trends / Popular Culture**: What becomes “in” often depends on what people believe others will do; can lead to widespread adoption of a trend whether or not it is “objectively good.”

---

### 8. Why is communication more effective in coordination games than in Prisoner’s Dilemma situations?

* In coordination games, communication can align beliefs: letting everyone know “I expect you to play X” can shift expectations so that playing X becomes a best response. Because outcomes depend heavily on beliefs about others, communication helps pick among equilibria.

* In Prisoner’s Dilemma, communication alone typically *cannot* overcome the incentive to defect, because defecting is a strictly dominant strategy: regardless of what you believe the other will do, defecting yields a better payoff. So even if everyone agrees verbally, each has an individual incentive to deviate. Thus, contracts, enforcement, or changing payoff structure are needed to escape the suboptimal outcome.

---

## Additional Notes & Reminders

* **Risk Dominance vs Payoff Dominance**: Sometimes players prefer an equilibrium that is “safer” (less risky given uncertainty in others’ actions) even if it yields lower payoff. This may explain why “bad” equilibria are often chosen in practice.

* **Initial Conditions / Beliefs Matter**: In many coordination games, how the game starts (initial beliefs, past rounds, cues, focal points) plays a big role in which equilibrium is selected.

* **Multiple Equilibria is not “bad” in theory**, but it means predictions need more structure (e.g. norms, communication, focal points) to be precise in practice.

---
