# Phased Goal Journeys

**Status:** Proposed planning and presentation approach.

## Idea

Avoid overwhelming users by presenting a long goal as a journey divided into phases. The user can see the overall path, but does not have to absorb every task at once.

- Show the journey's phases with a short brief for each later phase.
- Explain the phase the user is currently in detail.
- Show the steps and tasks needed to complete the current phase and reach the next one.
- Expand later phases with detailed plans as the user progresses.

## Phase-end readiness review

A milestone at the end of a phase can trigger a review rather than an automatic phase transition. The AI should examine:

- Progress made during the phase.
- Consistency across the phase.
- Whether tasks were completed on time.
- Whether the other milestones in the phase were reached.

The AI then discusses its detailed analysis with the user in conversation and assesses whether the user is ready to move on. It is not yet decided whether the AI's readiness assessment automatically advances the user or whether the user makes the final call. This authority decision is deliberately deferred for later.

## If the user is not ready

If the AI concludes that the user is not ready to advance, it should:

1. Converse with the user and provide a detailed explanation of why it reached that conclusion.
2. Deliver the review with care and reassurance, recognizing that hearing they are not ready may hurt the user's feelings.
3. Propose structural changes to the user's daily plan and tasks, aiming to make readiness more likely if the user follows the revised plan consistently.

Any proposed schedule changes still follow the user approval and conversational negotiation flow in [Visual Recommendations with Approval](015-visual-recommendations-and-approval.md) and [Conversational Change Negotiation](016-conversational-change-negotiation.md).

## Repeat the review cycle

After a revised plan is agreed, the user continues toward the same phase-end milestone. Once that milestone is reached, repeat the phase review: assess streak consistency, missed tasks and deadlines, and the other milestones in the phase, then discuss the analysis with the user. If the user is still not ready, revise the plan and repeat the cycle again.

## Questions to resolve

- Who makes the final readiness decision after the AI and user discuss the phase review?
- How should the review account for missed deadlines, changed circumstances, or deliberate changes to the plan?
- How should a delayed phase-end milestone affect the timing of progress-aware check-ins?
- How much of the overall journey should be visible in the initial overview?
- When should later phases be revised based on the user's progress or changing goals?
