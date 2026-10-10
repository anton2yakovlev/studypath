# Platform guide

Which connector to use for what, and how to search well. Tool names are the ones each connector exposes; if a tool is missing or renamed, use the closest one and say so.

## Coursera

Tools: `search_courses`, `search_videos`, `search_hands_on_learning`, `get_course_material`, `coursera_roleplay_practice`.

- `search_videos` finds short lessons, good for one concept per module.
- `search_courses` finds full courses; use one course as the spine of a plan when it matches the outcome, then fill gaps with single videos.
- `search_hands_on_learning` finds guided projects, good for the practice slot in a module.
- `get_course_material` returns lesson content for notes and quizzes.
- Search with the module outcome in plain words ("regression with scikit-learn"), not the whole topic.

## Udemy Business

Tools: `search_courses`, `search_learning_paths`, `search_lectures`, `search_labs`, `get_course_curriculum`.

- `search_lectures` finds single lectures inside courses, the best fit for module-level planning.
- `get_course_curriculum` lists sections and lectures with durations; use it to pick the exact lectures from a long course instead of assigning the whole course.
- `search_labs` finds hands-on labs for practice slots.
- `search_learning_paths` gives ready-made sequences; use one as a starting point, then trim to the user's budget.
- This connector needs a Udemy Business account, usually through an employer. Say so if the user cannot sign in.

## O'Reilly

Tool: `search_oreilly_content`.

- Returns books, video courses and live events. Filter the results to video courses and book chapters; a chapter makes a good reading companion to a video lesson.
- Durations may be missing; estimate and mark the estimate.

## Web search (fallback)

- Use when no learning platform is connected or a module has no good match on them.
- Prefer university open courseware, official documentation, and channels of known instructors or institutions. Open the page to confirm the title, author and length before listing it.
- For a public video, the plan can rely only on the title, description and chapters. Offer to refine notes if the user pastes a transcript.

## Picking across platforms

- One spine, many branches: pick one course or learning path as the spine when it covers more than half the outcomes, then fill the rest with single lessons from any platform.
- Do not mix two full courses that cover the same ground. Pick the better one and cite the other as an alternative.
- Always say which platform each lesson is on, because the user may not have access to all of them.
