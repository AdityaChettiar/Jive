# Jive Goal Planner — Discovery Interview

**Status:** In discussion; no product requirements or implementation choices are finalized.

## Product framing

The initial idea was a student planner. The product owner has since broadened it to a planner for anyone trying to organize their workflow and grow in one or more areas. A user would share goals, fixed commitments (such as work, classes, or chores), and workable time. A conversational assistant would clarify what they want to achieve, help structure a realistic programme, and turn it into daily tasks according to their priorities. The plan should adapt to changing commitments and contexts. Social accountability and connections with like-minded people are additional exploratory directions. Nutrition support may eventually align meals with activities and energy needs.

The goal is to organize the ideas through an interview and agree on how the app should work before implementation begins.

## Current core hypothesis

The complete loop should work well end to end: clarify goals, structure them into realistic plans and daily tasks around fixed commitments, adapt as life changes, and support follow-through. The product owner does not want the other parts treated as secondary or allowed to work poorly. If one differentiator must be named, it is accountability: helping users stay locked in and keep making progress. This is the product owner's stated direction, to validate and refine.

## Interview notes

- Proposed onboarding learns what kind of person the user is (for example, student or working person), gathers a relatively stable weekly routine, asks about activities and goals, and captures priorities for regular available time and newly freed time.
- A user provides goals, fixed commitments (work, classes, chores), and workable time.
- Goal clarification example: if a user says they want to get good at coding, the assistant asks what they want to build and why, then helps narrow it (for example, game development or financial modelling).
- The planner structures steps into a realistic programme and daily tasks. Multiple goals may be pursued at once, with time allocation based on user priorities.
- Proposed adaptation includes exam seasons, vacations, cancelled classes, and other new or freed time. The planner could allocate or reassign tasks to fit priorities.
- Proposed accountability combination: visible streaks for selected activities, occasional progress photos, and regular check-ins at both individual and group levels. Sharing rules and cadence remain undecided.
- Visibility is undecided; current preference is to let users choose whether progress is visible to their group or public. Exact options and defaults will be clarified later.
- Check-ins should let users report what went to plan, what did not, any extra work completed, whether the schedule felt workable or too hectic, and changes they suggest. This feedback should help the AI improve future plans.
- Users should always have an available place in the app to provide feedback whenever they choose. Separately, they should choose how often the app proactively checks in (examples: daily, every other day, twice weekly, or weekly).
- The always-available feedback space should combine freeform conversation with optional structured prompts, with freeform conversation as the main mode. The user values having room to explain details or vent and feel more comfortable. See [Conversational Feedback Space](014-conversational-feedback-space.md).
- Preferred response to a user discussing a problem: the AI should acknowledge and show it understands the specifics, reassure them, offer personalized encouragement rather than generic pep talk, suggest several tailored ways to work on the problem, and close on a constructive note that emphasizes the value of trying even when progress is imperfect.
- When offering solutions, the AI should explain pros and cons, ideally with an engaging visual comparison, then recommend the option that best fits the user's priorities and current situation. The user and AI can revise the proposed set conversationally. If the user chooses a change the AI considers suboptimal, the AI explains the concern and checks the user is sure; if the user confirms, the user has the final say and the change can be made. See [Visual Recommendations with Approval](015-visual-recommendations-and-approval.md) and [Conversational Change Negotiation](016-conversational-change-negotiation.md).
- Users should be able to propose changes, undo them, return to an old schedule, or create a new schedule. Frequent replanning may become a substitute for actual progress, so a minimum interval between major replans is proposed; the interval and how it is enforced are undecided. See [Replanning Cadence and Progress Focus](017-replanning-cadence-and-progress-focus.md).
- Proposed staged replanning guardrail: for the first two or three rapid replanning attempts, offer a gentle reminder that consistency matters and frequent planning can feel like progress without producing it. If changes continue too often, the app may temporarily prevent changes for a period. The frequency threshold and block duration remain undecided.
- Deliberately deferred: whether undoing a change or restoring an older schedule stays available during a temporary replanning block.
- Progress tracking should combine consistency (streaks) with goal-specific milestones and evidence. Examples include completed tasks, built coding projects, artwork, physique updates, language progress, and certifications. See [Progress Signals and Goal Milestones](018-progress-signals-and-goal-milestones.md).
- Milestones should be finalized conversationally: the AI proposes plausible milestones, the user can accept selected ones or contribute their own, and both work toward an agreed set.
- To avoid overwhelming users with a long plan, show the overall goal journey in phases with short previews for later phases. Explain the current phase in detail, with each step needed to reach the next phase. See [Phased Goal Journeys](019-phased-goal-journeys.md).
- A phase's closing milestone can initiate a readiness review. The AI reviews progress, consistency, whether tasks were done on time, and completion of other phase milestones, then discusses its analysis with the user and assesses readiness to advance. Whether the AI's assessment automatically advances the user or the user makes the final call is deliberately deferred.
- If the AI assesses that the user is not ready, it should explain in detail why, do so supportively because the conclusion may hurt, and propose structural daily-plan changes that increase the chance of readiness if the user follows the revised plan consistently. Schedule changes remain subject to the agreed approval flow.
- After a revised plan, the same phase-end milestone remains the readiness signal. Once it is reached, the AI repeats its review of streak consistency, missed tasks and deadlines, and other phase milestones, followed by a conversational exchange. If the user is not ready, the revised-plan and review cycle repeats.
- User-selected progress check-ins can raise pending tasks and milestones before the phase-end review. The AI should ask what got in the way, understand whether the schedule fits, suggest solutions, and reassure the user in a supportive life-coach manner rather than sounding like a teacher. See [Progress-Aware Coaching Check-ins](020-progress-aware-coaching-check-ins.md).
- A task left unfinished for a prolonged period can trigger an app notice or alert. If a milestone remains incomplete for an extended time despite repeated schedule restructuring, the AI can raise it in a routine check-in. The strategy for prolonged inconsistency and the strategy for continued lack of progress despite consistency and repeated adjustments are both deliberately deferred. See [Overdue Alerts and Persistent Blockers](021-overdue-alerts-and-persistent-blockers.md).
- If the user says the schedule is difficult, the assistant should ask what is making it difficult and suggest adjustments that protect the user's priorities. If the user chooses a change that could hamper progress, the assistant should explain the likely trade-offs before proceeding.
- Finding people with shared interests or learning goals is an additional social direction; its relationship to accountability groups remains undecided.
- Product owner emphasizes that the whole planning loop should work well; accountability is the differentiating factor that should push users to stay committed.
- Nutrition support is a possible future area: align food timing or plans with activities and energy needs. Exact scope and evidence standards need discussion.
- Earlier student-specific examples remain relevant as possible use cases: LMS or screenshot timetable import; academics, gym, diet, habits, content creation; backlogs and energy-aware scheduling.
- These are proposals, not confirmed feature requirements.

## Decisions so far

- Keep this repository in discussion and documentation mode until product behavior and implementation approach are agreed.
- Keep `frontend/` and `backend/` at the repository root as the planned application areas.
- The product is intended to serve beyond students, though its first audience is undecided.
- Defer choosing or setting up a local SQL database until its need is clear.
- Do not apply proposed schedule changes without user approval. The user retains final control after the AI explains any concern and confirms a potentially suboptimal choice.

## Open questions

- Which first audience or use case should the first version serve?
- What forms of accountability best help users stay committed without feeling punitive or intrusive?
- What should count as fixed versus movable time?
- What information makes a goal programme realistic and actionable?
- How should the planner prioritize several goals and handle overload?
- How much control should the user have over AI suggestions and automatic rescheduling?
- What should the social layer expose, and should it be in the first release?
- What privacy expectations apply to calendar, routine, goal, and social data?
- What does a useful first release include, and what is explicitly out of scope?
