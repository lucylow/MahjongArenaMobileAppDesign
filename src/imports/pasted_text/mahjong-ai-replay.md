 Prompt 6 — “Mahjong Intelligence Replay”: Counterfactual Game Analysis

```text
Design a mobile AI analysis product called “Mahjong Intelligence Replay.” The app imports or records a completed four-player Mahjong game and lets users replay important decisions, compare alternate actions, simulate possible outcomes, and understand how a hand developed. Design a high-fidelity React Native + Expo mobile application for iPhone and Android using a 390 x 844 frame.

The visual system should feel like a sophisticated sports replay and analytics product, but still unmistakably Mahjong. Use a dark graphite background, rich teal table surface, porcelain-white tiles, amber for the selected timeline moment, cyan for alternate lines, and muted red for dangerous branches. Use clean cards, timeline markers, bottom sheets, segmented controls, and strong typography. Keep all complex information progressively disclosed so beginners are not overwhelmed.

Create these connected screens:

1. Replay dashboard. Show recently analyzed games, import options, saved moments, and a card called “Your most important decision.” Include game metadata such as date, final placement, score change, number of reviewed moments, and analysis status. Provide buttons labeled “Import Game,” “Continue Review,” and “Explore Saved Moments.”

2. Game analysis setup. Let the user select the target player, analysis depth, AI policy, and review focus. Options should include “Efficiency,” “Defense,” “Scoring,” “Opponent Reading,” “Calls and Melds,” and “All Critical Decisions.” Include a processing state with an elegant visualization of the AI scanning the game timeline. Do not imply that analysis is perfectly objective.

3. Full replay timeline. Show a horizontal hand-by-hand timeline adapted for mobile scrolling. Each decision marker should use an icon and label such as “High impact,” “Risk,” “Missed value,” “Good defense,” or “Interesting alternative.” Include filters for East, South, All hands, and Only key moments. Show a small score graph across the match, but keep it simple and readable.

4. Decision replay screen. Display the exact Mahjong state before a selected action: player hand, discards, melds, dora, scores, round, turn, and visible information. Add replay controls at the bottom: Previous decision, Play forward, Pause, Next decision, and Jump to key moment. Use a small “Original action” badge so the user always knows what actually happened.

5. Counterfactual branch screen. After the original decision is shown, allow the user to compare it with one or more alternate actions. Present a branch selector with “Original,” “AI Recommendation,” “Safer Line,” and “Higher-Value Line.” Display each branch as a visual path through the next few turns. Use language such as “estimated continuation,” “sampled outcome,” and “possible result.” Do not display counterfactual results as guaranteed outcomes.

6. Branch comparison. Show a mobile comparison card with the following sections: hand development, shanten trajectory, likely win speed, expected value range, deal-in exposure, and strategic objective. Use colored but accessible indicators and short explanations. Include a button called “Why did the branches diverge?” that opens a natural-language explanation.

7. AI reasoning layers. Create an expandable screen with three layers of explanation:

   “Visible state” — what tiles, scores, calls, and round information were available.

   “Inferred state” — what the AI estimates about opponents, danger, and likely hand direction.

   “Policy choice” — why the selected AI style preferred speed, value, defense, or score preservation.

Include an uncertainty indicator for every inferred element. Make it impossible to confuse visible facts with AI estimates.

8. Game story screen. Convert the completed match into a narrative summary with chapters such as “Fast Start,” “Turning Point,” “Defensive Recovery,” and “Final Push.” Each chapter should contain the score situation, one important decision, a small board snapshot, and a short AI explanation. Include a toggle for “Technical analysis” and “Simple explanation.”

9. Personal insights screen. Aggregate repeated patterns across analyzed games. Show insights such as “You tend to overvalue high-scoring hands when behind,” “Your defensive decisions improve after visible riichi,” or “You frequently miss low-cost fast wins.” Each insight must include sample size, confidence level, supporting moments, and a button labeled “Practice this pattern.” Avoid making psychological or permanent claims about the player.

10. Export and sharing screen. Let the player save a decision card, export a review link, or share a simplified hand explanation with friends. Include privacy controls for hiding usernames, removing scores, and excluding private game logs. Provide a clear deletion action for imported games.

Interaction requirements: prioritize the replay timeline, decision clarity, branch comparison, and uncertainty communication. Use bottom sheets for explanations and full-screen views for complex comparisons. Preserve the original game state visually while using cyan or amber overlays for alternate branches. Avoid presenting AI simulation as destiny. Avoid dense charts, unexplained model jargon, fake precision, or a single universal “correct move.”
```

## How These Three AI Directions Differ

| AI design principle | AI Copilot Table | Adaptive AI Lab | Mahjong Intelligence Replay |
|---|---|---|---|
| Primary moment | During the decision | Before and during the match | After the match |
| Main AI output | Recommendations and explanations | Opponent behavior and training scenarios | Alternate branches and game insights |
| Best user type | Players who want help while playing | Players who want targeted practice | Players who enjoy analysis and improvement |
| Key trust mechanism | Confidence ranges and visible assumptions | Configurable behavior and adaptation controls | Original-vs-counterfactual separation |
| Strongest MVP screens | Live table, AI sheet, decision detail | Opponent library, configuration, training results | Timeline, decision replay, branch comparison |

## Recommended AI Product Sequence

For the strongest initial product strategy, begin with **Prompt 4, AI Copilot Table**, because it places the AI directly inside the gameplay loop without requiring a large game-history database. Follow with **Prompt 6, Mahjong Intelligence Replay**, once game logs and decision states can be stored reliably. Add **Prompt 5, Adaptive AI Lab**, when the app has enough player behavior data to make personalization meaningful.

The most important design rule across all three concepts is to distinguish **observed facts**, **AI inferences**, and **strategic recommendations**. This is especially important in Mahjong because the game contains hidden information and multiple reasonable lines of play.[1] [2] [3]