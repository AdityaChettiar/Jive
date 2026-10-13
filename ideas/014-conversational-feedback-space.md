# Conversational Feedback Space

**Status:** Proposed; response style and boundaries need discussion.

## Idea

Keep an always-available place where users can talk about how their plan is going. Use a mix of freeform conversation and structured prompts, with freeform conversation as the primary mode. A conversation can draw out context and detail that a form may miss, while giving the user room to vent and feel comfortable getting things off their chest.

This space can support the plan feedback loop: the user may explain what went to plan, what did not, extra progress, how the schedule felt, and changes they want. The AI can use the conversation to improve future plans. See [Check-in Feedback and Plan Calibration](013-check-in-feedback-and-plan-calibration.md).

## Preferred response flow

The user should not have to choose between “just listen” and “give advice.” When they discuss a problem, the assistant should:

1. Acknowledge the specific situation and demonstrate that it understands the details.
2. Reassure the user and offer personalized encouragement, avoiding generic pep talk that could feel irritating.
3. Suggest a variety of solutions tailored to the problem.
4. End constructively, reinforcing that trying and continuing to make an effort matters even when things do not go perfectly.

For schedule changes, recommendations should follow [Visual Recommendations with Approval](015-visual-recommendations-and-approval.md): explain trade-offs and wait for the user's approval before applying a change.

## Questions to resolve

- How should the assistant transition from discussing a problem to proposing schedule or goal changes?
- Which structured prompts would help without making the conversation feel like a form?
- What tone and kinds of reassurance feel personal rather than generic?
