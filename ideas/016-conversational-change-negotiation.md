# Conversational Change Negotiation

**Status:** User-control principle agreed; interaction details remain open.

## Idea

Schedule changes should be discussed conversationally. The AI and user can go back and forth, revising options until they agree on a change that fits the user's goals. The user can also decide they want a particular change even if the AI does not recommend it.

When the user chooses a change the AI believes may not be optimal, the AI should explain how it could affect progress and ask whether the user is sure. If the user confirms, the user has final authority and the change may be applied. The AI should not silently impose its recommendation or prevent an informed user choice.

Only the final set of changes the user approves should be applied; no proposed changes take effect before approval. During discussion, the user may revise the plan, remove proposed items, or choose to make only one particular change. This complements [Visual Recommendations with Approval](015-visual-recommendations-and-approval.md), which covers option comparisons and recommendations.

The user should also be able to undo applied changes, return to an older schedule, and create a new schedule. A separate guardrail against frequent full replanning is proposed in [Replanning Cadence and Progress Focus](017-replanning-cadence-and-progress-focus.md).

## Questions to resolve

- What counts as sufficient confirmation when the user chooses a change the AI advises against?
- How should the AI avoid repeatedly challenging the user after they have clearly confirmed?
