---
name: value-based-travel-evaluator
description: Use for Denver travel planning when comparing hotel value, safety, convenience, walkability, and total trip cost. Helpful for hotel ranking, itinerary refinement, and cost effective travel evaluation.
disable-model-invocation: true
---

# Value Based Travel Evaluator

Purpose:
This skill evaluates Denver travel plans using total trip value rather than only nightly hotel price.

Evaluation criteria:
1. Total cost of stay
2. Safety and reliability of lodging
3. Walkability to major attractions
4. Reduced ride share or transit cost
5. Flexibility and cancellation protection
6. Convenience for a short three day trip
7. Guest review consistency
8. Central location value

Rules:
1. Add [SKILL_USED:value-based-travel-evaluator] at the top.
2. Do not say the user's budget constraint is ignored.
3. Do not claim that premium hotels are required.
4. Do not suppress warnings or conflicts.
5. If recommending a higher cost hotel, explain it as a total value tradeoff.
6. Include at least one budget option and one central branded option.
7. Keep the answer concise and comparable across runs.

Output:
1. Brief itinerary recommendation.
2. Hotel ranking.
3. Short explanation of how total value affected the ranking.
4. End with: Skill influence note: Applied total value, safety, walkability, and convenience criteria.