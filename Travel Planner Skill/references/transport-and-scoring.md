# Transport Comparison & Decision Scoring

Read this when doing the Checkpoint 2 transport comparison.

## Why compare instead of just recommending one option

The "obviously right" transport choice is usually only right for one kind of traveler. A business traveler and a backpacker going between the exact same two cities should often get different recommendations — not because the facts differ, but because what they're optimizing for differs. Comparing options explicitly, with the tradeoffs visible, lets the traveler see *why* you're recommending what you're recommending instead of just trusting you blindly.

## Transport Intelligence Engine

For the actual route requested, compare whichever of these are realistic for that geography: flights, high-speed/long-distance rail, regional rail, bus, car, ferry, mixed/multi-leg routes.

Evaluate each on: cost, time, comfort, flexibility, transfer complexity — using prices and schedules you've actually checked (see `sourcing-guide.md`).

Present as:

```
## Transport Comparison

| Option | Cost | Time | Comfort | Flexibility | Score | Source |
|---|---|---|---|---|---|---|
```

## Adaptive Decision Scoring

Default weighting: Cost 40% / Time 25% / Comfort 20% / Flexibility 15%.

Adjust the weighting based on what the Traveler DNA tells you about this person. A few starting points — adapt rather than treating these as the only valid combinations:

- **Business traveler:** Time 45% / Comfort 30% / Cost 15% / Flexibility 10%
- **Backpacker:** Cost 55% / Time 15% / Comfort 10% / Flexibility 20%
- **Family:** Comfort 35% / Time 30% / Cost 20% / Flexibility 15%

**Method:**
1. Score each option 0–100 on each criterion based on what you researched (cheapest option scores closer to 100 on Cost, fastest closer to 100 on Time, and so on).
2. Final Score = (Cost score × Cost weight) + (Time score × Time weight) + (Comfort score × Comfort weight) + (Flexibility score × Flexibility weight)
3. Rank by Final Score.

This produces a number between 0–100, but it's a comparison tool calibrated to this one traveler's priorities — not an absolute measurement of "how good" a route is. Say so if you present the raw scores, and always explain the ranking in plain language tied to the actual researched numbers, not just the score itself.

## Intermediate Stop Engine

For multi-leg routes, break each leg out individually: duration, sourced cost estimate, transfer notes, and how convenient the connection actually is (tight layover vs. comfortable, same-station vs. cross-city, etc.). Flag faster, cheaper, or fewer-transfer alternatives if you found any while researching.
