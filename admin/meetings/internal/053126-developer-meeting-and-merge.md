# Team 10 - 10x Devs Meeting Minutes
---
## Meeting Info
| Field | Details |
|---|---|
| **Meeting Type** | Sprint / Team Standup + Work Session |
| **Date** | TBD (inferred from transcript — please fill in) |
| **Time** | ~8:15 PM – 9:30 PM |
| **Location** | Virtual (Video Call) |
| **Minutes Recorded By** | Evan Marriott |

---
## Attendance: Mark x if Present
Team Leads
- [x] Nicole Sutedja (nsutedja@ucsd.edu)
- [x] Evan Marriott (emarriott@ucsd.edu)

Members
- [x] Aron Wu (arw008@ucsd.edu)
- [x] Bethany Miyamoto (bmiyamoto@ucsd.edu)
- [x] Jensen Guo (jeg076@ucsd.edu)
- [x] Kaley Chung (kac101@ucsd.edu)
- [x] Xuanye Wang (xuw040@ucsd.edu)
- [x] Benedict Luis (bluis@ucsd.edu)
- [x] Han Yang-Lin (hyanglin@ucsd.edu)
- [ ] Prakhar Shah (prs016@ucsd.edu)

---
## Agenda
1. Team standup / status updates (round-robin)
2. Review failing tests and CI status on GitHub branches
3. Branch cleanup, pull requests, and merge conflict resolution

---
## Additional Meeting Notes
- Transcript was saved at the end of the meeting by Evan as a deliberate action.
- A midterm is upcoming on Tuesday; most members have not started studying.
- Nicole needs to leave by 9:30 PM.

---
## Old Business
*Unresolved items carried over from the previous meeting.*

### Item 1: Failing tests on GitHub branches
- **Background:** Tests had been failing on the `new-dash-prototype` branch due to UI refactoring and backend changes; not yet resolved before this meeting.
- **Discussion:** Nicole flagged the failures. Evan identified linting errors (easy fixes) and failing unit tests. Nicole noted one unit test was checking for `filter.js`, which had been deleted. Jensen confirmed missing comments were also causing CI failures.
- **Resolution / Status:** Aron volunteered to investigate unit test failures before the next meeting. Evan committed to fixing linting and other test issues that night.

### Item 2: README and documentation updates
- **Background:** Project setup instructions in the README had not been updated to reflect recent Supabase integration.
- **Discussion:** Evan reminded the team the README needs to be updated before Adria (professor/TA) reviews the project. Target: complete by end of Friday.
- **Resolution / Status:** Carried forward — assigned informally to the team; no single owner designated.

---
## New Business
*New topics introduced at this meeting.*

### Item 1: Pull request for `new-dash-prototype` branch
- **Introduced by:** Evan Marriott
- **Discussion:** Evan proposed opening a PR for the `new-dash-prototype` branch to surface merge conflicts and CI failures in one place, even before the branch is fully ready to merge. Debate arose over whether to connect the backend first. Kevin (Xuanye) confirmed merging now is fine, with another merge expected after backend integration. Bethany opened the PR during the meeting.
- **Resolution / Status:** PR opened by Bethany. Merge conflicts were resolved live by Evan (chose `new-dash-prototype` as the authoritative source for all conflicted files). Tests still need to be fixed before final merge.

### Item 2: ADR for notification system
- **Introduced by:** Evan Marriott
- **Discussion:** Evan noted the team currently has only 5 ADRs and flagged the notification system (NodeMailer + Notify) as a gap. Han also suggested the Supabase ADR should be expanded to include reasoning for using Supabase's built-in authentication.
- **Resolution / Status:** Kevin (Xuanye) volunteered to write the notification system ADR. Evan to update the Supabase ADR.

### Item 3: Additional triggered errors in the test app
- **Introduced by:** Evan Marriott
- **Discussion:** Evan added manually triggered errors (big red buttons) to the test app. Nicole suggested also adding errors triggered by invalid user input (e.g., entering a card number that exceeds the allowed length). Evan agreed to add ~2 such errors that night.
- **Resolution / Status:** Evan to implement and merge the `additional-errors` branch tonight.

### Item 4: GitHub branch cleanup
- **Introduced by:** Evan Marriott
- **Discussion:** Several old, merged branches were identified as candidates for deletion to reduce clutter: original `test-app` branch, `mock-data` branch, `user-research` branch, and the old `dashboard-prototype` branch (superseded by `new-dash-prototype`). Han confirmed the new branch contains all relevant updates from the old one.
- **Resolution / Status:** Evan deleted the stale branches during the meeting. Branches removed: `test-app`, `mock-data`, `user-research`, `dashboard-prototype`.

### Item 5: Rename `prototype` folder in repo
- **Introduced by:** Nicole Sutedja
- **Discussion:** Nicole suggested renaming the `prototype` folder since the project is no longer in prototype stage. Jensen noted that renaming it also requires updating linting test paths. Nicole agreed this is a non-trivial change.
- **Resolution / Status:** Tabled to next sprint. Evan offered to help since he is familiar with the test infrastructure.

### Item 6: Mobile responsiveness and wireframes
- **Introduced by:** Kaley Chung
- **Discussion:** Kaley fixed large-monitor empty space issues and pushed changes. She flagged failing tests related to CSS changes (unrelated to her modifications). She also proposed creating a wireframe for a future mobile view, even if there's no time to implement it this sprint.
- **Resolution / Status:** CSS fix pushed; test failures to be addressed separately. Mobile wireframe proposed as a future-sprint deliverable.

### Item 7: Uptime card on dashboard
- **Introduced by:** Nicole Sutedja
- **Discussion:** Nicole added an uptime card to the dashboard. Han confirmed the backend endpoint returns a list of uptime checks with timestamps and up/down status, which aligns with Nicole's intended display (showing last-checked-up time).
- **Resolution / Status:** Resolved — feature aligned between frontend and backend.

### Item 8: Next sprint checklist review
- **Introduced by:** Nicole Sutedja
- **Discussion:** Nicole proposed revisiting the original project requirements doc sent by Audreya to ensure all boxes are checked. Also noted Team 8's feedback mentioned a missing "definition of done" — can be written retroactively into process docs.
- **Resolution / Status:** Carried forward to next sprint planning.

---
## Decisions Made

### Decision 1: Merge `new-dash-prototype` to main now, reconnect backend later
- **Decision:** Open PR and merge `new-dash-prototype` without waiting for full backend integration.
- **Reasoning:** Kevin confirmed merging is safe now; another merge will happen after backend is connected. Getting code into main sooner reduces long-term merge conflict risk.
- **Dissenting Opinions:** Bethany asked if we should connect the backend first; Kevin noted we'd need to merge again anyway.
- **Why the group proceeded anyway:** Incremental merging is less risky than letting the branch diverge further.

### Decision 2: Evan resolves all merge conflicts by choosing `new-dash-prototype` as authoritative
- **Decision:** For all conflicted files, the `new-dash-prototype` version was accepted wholesale.
- **Reasoning:** Han confirmed the new branch contains all the latest backend refactoring; main was simply behind.
- **Dissenting Opinions:** None — team agreed after Han's clarification.
- **Why the group proceeded anyway:** N/A

### Decision 3: Delete stale branches
- **Decision:** Remove `test-app`, `mock-data`, `user-research`, and old `dashboard-prototype` branches.
- **Reasoning:** All had been merged or superseded; leaving them creates confusion for anyone reviewing the repo.
- **Dissenting Opinions:** None.
- **Why the group proceeded anyway:** N/A

---
## Deferred Items
| Item | Reason Not Discussed |
|---|---|
| Rename `prototype` folder | Non-trivial; requires test path updates — moved to next sprint |
| Full backend–frontend integration | Backend endpoints ready but integration not yet complete |
| Mobile responsiveness implementation | Insufficient time this sprint; wireframe proposed instead |
| Definition of done documentation | Lower priority; to be written retroactively next sprint |

---
## Action Items
| # | Task | Assigned To | Due Date | Status |
|---|---|---|---|---|
| 1 | Fix failing unit tests on `new-dash-prototype` PR (including removing reference to deleted `filter.js`) | Aron Wu | Before next meeting | Open |
| 2 | Fix linting errors on `new-dash-prototype` branch | Evan Marriott | Tonight | Open |
| 3 | Add ~2 input-triggered errors to test app, merge `additional-errors` branch | Evan Marriott | Tonight | Open |
| 4 | Write ADR for notification system (NodeMailer / Notify) | Xuanye Wang | Next sprint | Open |
| 5 | Update Supabase ADR to include reasoning for using Supabase auth | Evan Marriott | Next sprint | Open |
| 6 | Update README / project setup docs to reflect Supabase changes | Team (unassigned) | By Friday | Open |
| 7 | Review original project requirements doc and check off completed items | Nicole Sutedja + Team | Next sprint | Open |
| 8 | Rename `prototype` folder and update all test paths accordingly | Evan Marriott + Nicole Sutedja | Next sprint | Open |
| 9 | Add PR reviewers to `new-dash-prototype` PR and request approvals | Nicole Sutedja | ASAP | Open |
| 10 | Create mobile wireframe for future sprint consideration | Kaley Chung | Next sprint | Open |
