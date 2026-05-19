# Team 10 - 10x Devs Meeting Minutes
---

## Meeting Info

| Field | Details |
|---|---|
| **Meeting Type** | Sprint 2 Stand-Up / Check-In |
| **Date** | Not specified in transcript |
| **Time** | 4:01 PM – 4:29 PM |
| **Location** | Zoom (Virtual) |
| **Minutes Recorded By** | Generated from Zoom closed caption transcript |

---

## Attendance: Mark x if Present

Team Leads

- [x] Nicole Sutedja (nsutedja@ucsd.edu)

- [x] Evan Marriott (emarriott@ucsd.edu)

Members

- [ ] Hudson Gehrke (hgehrke@ucsd.edu)

- [x] Aron Wu (arw008@ucsd.edu)

- [x] Bethany Miyamoto (bmiyamoto@ucsd.edu)

- [x] Jensen Guo (jeg076@ucsd.edu)

- [x] Kaley Chung (kac101@ucsd.edu)

- [ ] Xuanye Wang (xuw040@ucsd.edu) *(noted as absent before meeting began)*

- [x] Benedict Luis (bluis@ucsd.edu) *(mic issues; communicated updates via chat, relayed by Evan)*

- [x] Han Yang-Lin (hyanglin@ucsd.edu)

- [x] Prakhar Shah (prs016@ucsd.edu)

---

## Agenda

1. Sprint 2 progress updates (round-robin)
2. GitHub issues review, cleanup, and assignment
3. Database decision and notification method (SMS vs. email)

---

## Additional Meeting Notes

- Sprint 2 is being extended through Thursday to align with the product demo deadline (Wednesday or Thursday submission).
- TA meeting scheduled for tonight at 8 PM — Evan confirmed he will attend.
- Nicole warned she may drop from Zoom due to low battery and would rejoin on her phone; Evan saved the transcript.
- Team agreed to use the Zoom closed caption transcript for meeting notes going forward instead of Granola.

---

## Old Business
*Unresolved items carried over from the previous meeting.*

### Item 1: GitHub Issues Cleanup
- **Background:** Several issues were left open on GitHub even though work had been completed (e.g., user personas).
- **Discussion:** Nicole closed open persona issues during the meeting. Evan emphasized that completed work should be reflected by closing the corresponding issue immediately.
- **Resolution / Status:** Partially resolved — Nicole closed some issues during the meeting; full cleanup deferred to after the meeting.

### Item 2: Watchtower / Test App Integration
- **Background:** Watchtower (the monitoring app) and the test app needed to be connected so that errors from the test app are picked up by Watchtower.
- **Discussion:** Evan built out the test app (a simple e-commerce site with ~5 pages, a purposeful error trigger button, and a post-checkout feedback widget). Han confirmed the integration should be feasible with changes pushed to main. The connection between the two apps has not yet been completed.
- **Resolution / Status:** Carried forward — connecting the test app to Watchtower is the primary goal for this week.

---

## New Business
*New topics introduced at this meeting.*

### Item 1: Notification Method — SMS vs. Email
- **Introduced by:** Prakhar Shah (raised during general discussion)
- **Discussion:** The team debated whether to use SMS or email for user notifications. Nicole noted the professor raised the concern that developers may not check emails on weekends. Prakhar researched Twilio and found a free 30-day plan offering 100 SMS messages and ~4,000 emails. The group agreed Twilio could cover both channels. Nicole plans to confirm with the professor at Wednesday office hours. The team agreed to defer SMS/notification work to the next sprint to stay focused on the MVP for Thursday.
- **Resolution / Status:** Tabled for next sprint — Twilio selected as likely provider; Nicole to confirm with professor on Wednesday.

### Item 2: Database Selection — Postgres vs. MongoDB
- **Introduced by:** Bethany Miyamoto / Han Yang-Lin
- **Discussion:** The team is deciding between PostgreSQL and MongoDB (referred to as "LongoDB" in transcript). Bethany noted Postgres supports JSONB for JSON storage. Han is leaning toward Postgres/SQL as well. The group agreed someone from the dev team should reach out to the TA (Audrey) or the professor to confirm the choice is acceptable before writing an ADR.
- **Resolution / Status:** Carried forward — Bethany will DM the TA/professor; Nicole will write the ADR once confirmed.

### Item 3: GitHub Issue Assignment Process
- **Introduced by:** Evan Marriott
- **Discussion:** Evan requested that all team members assign themselves to GitHub issues they are working on using the "Assign yourself" button on each issue. This makes task tracking and management easier. Nicole will add new issues tonight and assign anyone who hasn't self-assigned.
- **Resolution / Status:** Resolved — team instructed to self-assign by end of day; leads will force-assign any remaining unassigned tasks.

### Item 4: Changelog and AI Usage Log Updates
- **Introduced by:** Evan Marriott / Nicole Sutedja
- **Discussion:** The changelog currently only contains the initial project structure entry. Evan asked the dev team to add entries for the prototype and any other implemented features (takes only a few seconds). Nicole also reminded the team to update the AI usage log if they are using AI tools, noting that the course allows AI use as long as it's documented.
- **Resolution / Status:** Resolved — dev team to update changelog and AI log ASAP.

---

## Decisions Made

### Decision 1: Extend Sprint 2 Through Thursday
- **Decision:** Sprint 2 will not close at its original end date; it will be extended to ensure all current goals are completed before the product demo.
- **Reasoning:** The product demo is this Thursday (or Wednesday), and the team should not begin a new set of goals mid-sprint. Completing the MVP cleanly is the priority.
- **Dissenting Opinions:** None noted.
- **Why the group proceeded anyway:** N/A

### Decision 2: Twilio for Both SMS and Email Notifications (Deferred to Next Sprint)
- **Decision:** Use Twilio as the notification provider for both SMS and email. Notification feature will not be built this sprint — deferred to Sprint 3.
- **Reasoning:** Twilio offers a free 30-day plan with 100 SMS and ~4,000 emails, covering both channels. The professor's feedback indicated email alone may be insufficient for urgent alerts, but the team agreed not to overengineer it now.
- **Dissenting Opinions:** None noted.
- **Why the group proceeded anyway:** N/A

### Decision 3: All GitHub Issues Must Have Assignees
- **Decision:** Every open GitHub issue must have a team member assigned to it. Leads will assign unassigned tasks if not self-assigned by end of day.
- **Reasoning:** Makes it clear who is responsible for each task and simplifies sprint tracking.
- **Dissenting Opinions:** None noted.
- **Why the group proceeded anyway:** N/A

---

## Deferred Items
*Agenda items that were not reached or discussed — carry forward to next meeting's Old Business.*

| Item | Reason Not Discussed |
|---|---|
| Formal sprint retrospective | Intentionally skipped — this was a stand-up, not a retro |
| SMS/Notification implementation | Deferred to Sprint 3; focus this sprint is MVP for Thursday demo |

---

## Action Items
*Tasks assigned as a result of this meeting.*

| # | Task | Assigned To | Due Date | Status |
|---|---|---|---|---|
| 1 | Add new GitHub issues and assign all team members | Nicole Sutedja | Tonight | Pending |
| 2 | Connect prototype to test app; schedule another dev meeting | Nicole Sutedja | Before Thursday | Pending |
| 3 | DM TA (Audrey) or professor to confirm database choice (Postgres) | Bethany Miyamoto | ASAP | Pending |
| 4 | Write ADR for database once confirmed | Nicole Sutedja | After confirmation | Pending |
| 5 | Connect uptime tracking feature to dashboard | Han Yang-Lin | Before Thursday | Pending |
| 6 | Integrate test app with Watchtower | Han Yang-Lin | Before Thursday | Pending |
| 7 | Push linting ADR; integrate ESLint into GitHub Actions CI pipeline | Aron Wu | By Wednesday night | Pending |
| 8 | Begin writing unit tests | Aron Wu | By Wednesday night | Pending |
| 9 | Get ESLint working; get GitHub Actions pipeline working | Benedict Luis | By Wednesday night | Pending |
| 10 | Help Kevin code remaining pages (issues view, deployments, user feedback) | Jensen Guo | Before Thursday | Pending |
| 11 | Update Figma wireframes to be more detailed (hi-fi); help Jensen | Prakhar Shah | Before Thursday | Pending |
| 12 | Push research (135 upside / user personas / user stories) to GitHub | Prakhar Shah | ASAP | Pending |
| 13 | Complete upset user signals research and upload to GitHub | Kaley Chung | This week | Pending |
| 14 | Add more GitHub issues; oversee test app ↔ Watchtower integration | Evan Marriott | Tonight / ongoing | Pending |
| 15 | Attend TA meeting at 8 PM tonight | All (Evan confirmed) | Tonight | Pending |
| 16 | Update changelog with prototype implementation details | Dev team | ASAP | Pending |
| 17 | Update AI usage log if using AI tools | All | ASAP | Pending |
| 18 | Self-assign to relevant GitHub issues | All | Tonight | Pending |
| 19 | Attend Wednesday office hours; confirm Twilio / notification approach with professor | Nicole Sutedja, Evan Marriott | Wednesday | Pending |
