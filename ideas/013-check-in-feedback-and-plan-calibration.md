# Check-in Feedback and Plan Calibration

**Status:** Proposed; the assistant's adjustment and challenge behavior needs discussion.

## Feedback availability

Users should always have an available place in the app to provide feedback whenever they choose. Separately, they should control how often the app proactively checks in; suggested choices include daily, every other day, twice a week, or weekly.

Feedback should support a mix of freeform conversation and structured prompts, with freeform as the primary mode so users can describe context and vent comfortably. See [Conversational Feedback Space](014-conversational-feedback-space.md).

## Idea

Use check-ins as feedback that helps the AI plan better over time. A user may report:

- What went according to plan.
- What did not happen, and what they could not complete.
- Extra progress beyond the plan.
- Whether the schedule worked well or felt too hectic.
- Changes they would like to make.

The assistant should use this feedback to adapt future schedules. If the user says the schedule is difficult, the assistant should ask what is making it difficult and suggest adjustments that protect the user's priorities. If the user still wants a change that could hamper progress, the assistant should explain the likely trade-offs so the user can make an informed choice. Plans should remain workable while still supporting the user's stated goals.

The same supportive, evidence-based approach applies if the AI assesses that a user is not ready to advance to the next goal phase: explain the reasons, reassure the user, and offer structural plan changes to improve their chances if followed consistently. See [Phased Goal Journeys](019-phased-goal-journeys.md).

In proactive check-ins, the AI may raise pending tasks or milestones before a phase-end readiness review. It should ask what got in the way, assess whether the schedule is working, offer solutions, and reassure the user in a life-coach tone. See [Progress-Aware Coaching Check-ins](020-progress-aware-coaching-check-ins.md).

## Questions to resolve

- How should the assistant distinguish a temporary difficult period from a persistent mismatch between the plan and available time?
- How direct should the assistant be when explaining a trade-off that may slow progress?
- What should it do if the user's stated priority conflicts with their repeated choices?
- How should it incorporate extra progress and missed work into future workload estimates?
- What information should be shared with an accountability group, if any?
