# Lesson 01 · Conversation evidence

AI-drafted task summary, not a transcript or grade. It may be public. Use actual
short quotes or labeled paraphrases, name any help supplied, and link actual
work. Leave missing contributions Pending. A learner can review, correct or
remove excerpts before publication; accuracy approval is not proof of learning.
Label role-play honestly rather than treating it as an actual learner response.

**Lesson:** STUDIO-001. **Available conversation context:** This coaching chat; current contribution excerpts approved for accuracy.

## Prediction

Learner revised explanation after AI help:
"Https sends the request to DNS and then into DigitalOcean's Droplet. Then the browser sends the https request to droplet where Traefik routes the correct Docker container."

AI help before this revision: explained DNS lookup and Traefik hostname routing.
AI clarification, accepted by the learner: DNS returns the droplet IP; it does not forward HTTPS. The browser connects to that IP and Traefik routes the request to the calculator container. The learner approved keeping the quote, correction and help note.

## Check interpretation

Learner quote: "The check establishes that the calculator is accessile through the public IP https, processes the 6x7 multiplication and returns the correct result 42. It checks only that one calculation and none of the other operations. It also does not check for different inputs or invalid inputs."
AI clarification: this check used the public HTTPS hostname, not HTTPS directly
to the IP. Separate automated checks tested selected invalid inputs.


## Browser observation

Learner quote: "It shows the correct answer 6x7 on both the JavaScript calculated locally as well as Python verified by FastAPI."
This is the learner's reported observation, separate from AI runtime checks.


## Keep decision

Learner chose keep. After AI asked for a reason and offered matching expected
results as an example, learner wrote:
"Yes both the frontend and backend answers matched perfectly signifying that both processes work for that specific input. We still would have to test other operations and invalid input error handling."


## Review

Learner approved the current prediction quote, AI correction and help note in this chat. Learner also approved the interpretation, browser observation and keep-decision excerpts as accurate in this chat. Approval records accuracy, not proof of understanding.

## AI work and next step

AI ran local setup and selected read-only server/HTTPS checks. Learner established SSH access, ran configure/plan/doctor, added DNS and created issue #1. Doctor reported ready for a new launch. New launch evidence is saved. Learner supplied interpretation, browser observation and keep reason. Fast checks passed: Black, Pylint and 91 tests; 2 deselected. Browser E2E remains unrun. Repeat live verification passed; latest sanitized evidence is in studio/evidence.json, with the original launch retained in studio/launch-evidence.json. Local Docker is unavailable in WSL. Next: reviewed PR/CI work; full E2E remains pending.
