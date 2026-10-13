# Jive Goal Planner

Jive is a goal and workflow planner for people who want to make progress in one or more areas of life. It is in its discovery and planning stage. This repository is currently for organizing product ideas and agreeing on how the app should work. **No software implementation has started.**

## Repository layout

- [`ideas/`](ideas/README.md) — one Markdown document per idea discussed, including open questions and decisions.
- [`frontend/`](frontend/README.md) — future home for the user-facing application; currently documentation only.
- [`backend/`](backend/README.md) — future home for server-side behavior and data; currently documentation only.

## Working agreement

We will discuss and agree on the product and implementation approach before building features. Interview notes and proposals should be recorded under `ideas/`; update the relevant folder README when its high-level direction changes, and keep this file aligned with the overall agreed plan.

## Current direction

- The product is intended for anyone who wants to organize their workflow and grow toward one or more goals; it is not limited to students.
- The proposed core is to clarify goals, turn them into workable daily tasks around fixed commitments, and adapt the plan as priorities or availability change.
- The planning loop should work well end to end; accountability is the proposed differentiator that helps users stay committed. A conversational feedback space should provide personalized support and help improve future plans.
- Progress may combine consistent activity streaks with goal-specific milestones and tangible evidence of growth.
- Goal journeys may be shown as phases: a brief overview of the full path, with detailed steps for the current phase to avoid overwhelming the user.
- Reaching a phase's final milestone should trigger an AI-led progress review. The AI assesses readiness; whether that assessment automatically advances the user or requires their final decision is deferred.
- User-selected check-ins may review pending tasks and milestones, explore what got in the way, and support the user in a life-coach tone.
- Prolonged unfinished tasks may trigger app notices; persistent milestone delays should be discussed during routine AI check-ins. Deeper intervention strategies remain open.
- AI-proposed schedule changes are negotiated conversationally and applied only after approval. The AI may explain a concern and confirm an informed choice, but the user retains final control over their schedule.
- Users should be able to undo changes, restore past schedules, and create new schedules. For frequent replanning, the proposed guardrail starts with gentle reminders and may progress to a temporary block; thresholds and duration remain undecided.
- The first user group and first-version scope are still being explored.
- Social accountability, matching users with similar interests, and nutrition support are exploratory ideas; their place in an initial release is undecided.
- The repository will have `frontend/` and `backend/` at its root.
- A local SQL database may be considered later if the agreed product needs one; no database has been selected or set up.
- No environment secrets are needed at this discovery stage. Local `.env` files are ignored by Git.

## Status

Discovery only. See [`ideas/001-student-planner-discovery.md`](ideas/001-student-planner-discovery.md) for the interview brief and [`ideas/`](ideas/README.md) for individual concepts and unanswered questions.
