# Team 10 - 10x Devs Meeting Minutes
---

## Meeting Info

| Field | Details |
|---|---|
| **Meeting Type** | TA Check-In |
| **Date** | May 18, 2026 |
| **Time** | 5:00 PM - 5:45 PM PST |
| **Location** | Zoom (Virtual) |
| **Minutes Recorded By** | Prakhar Shah |

---

## Attendance: Mark x if Present

Team Leads

- [x] Nicole Sutedja (nsutedja@ucsd.edu)

- [x] Evan Marriott (emarriott@ucsd.edu)

Members

- [x] Aron Wu (arw008@ucsd.edu)

- [ ] Bethany Miyamoto (bmiyamoto@ucsd.edu)

- [x] Jensen Guo (jeg076@ucsd.edu)

- [ ] Kaley Chung (kac101@ucsd.edu)

- [ ] Xuanye Wang (xuw040@ucsd.edu)

- [x] Benedict Luis (bluis@ucsd.edu)

- [x] Han Yang-Lin (hyanglin@ucsd.edu)

- [x] Prakhar Shah (prs016@ucsd.edu)

---

## Agenda

1. Team Member & Notification Service Updates
2. MVP Prioritization, Deliverables, and Hard Deadlines
3. Frontend Architectural Decisions, Wireframes, and AI Cohesiveness
4. Demo Feedback and Sprint Goals

---

## Additional Meeting Notes

- The presentation video should prioritize showing design choices, AI usage, and the respective pros and cons.
- Focus on quality over quantity and process over product to ensure the project choices are easily justifiable.

---

## Old Business

### Item 1: Sprint 2 Progress & Team Updates
- **Background:** Carrying over the results and goals set during Sprint 2 planning.
- **Discussion:** The team discussed their Sprint 2 progress, goals, and outcomes. Evan expressed that they are very happy with the team's progress so far. Additionally, Evan and Nicole notified the TA that the team has successfully increased internal communication, set up more regular web sync meetings, and successfully migrated all task tracking to GitHub Issues.
- **Resolution / Status:** Resolved — Sprint 2 progress and organizational improvements approved by the TA.

---

## New Business

### Item 1: Team Member & Notification Service Updates
- **Introduced by:** Nicole Sutedja & Prakhar Shah
- **Discussion:**
  - **Nicole's Update:** Nicole has been working through dependency issues and setting up notification systems via email and SWS (Twilio).
  - **Audria's Feedback:** Audria requested that developer team contact information (email and other linked info) be easily accessible, and notifications should be integrated directly through the web app. She noted she likes Twilio but emphasized that the team must provide clear justification in the ADR (Architectural Decision Record) for using it.
  - **Prakhar's Concerns:** Prakhar raised a concern that notifications are not instant enough when delivered solely through the web application, recommending an on-call paging style mechanism for critical alerts. He also raised a potential pricing risk: SMS and email notification support will not be free in the long run.
  - **Audria's Suggestion:** Audria suggested looking at PagerDuty for inspiration on instant alerting systems and will follow up with more information.
- **Resolution / Status:** Carried forward — Team to explore on-call paging alerting models and document Twilio integration justification in the ADR.

### Item 2: MVP Prioritization, Deliverables, and Hard Deadlines
- **Introduced by:** Audria (TA)
- **Discussion:**
  - **MVP Focus:** It is critical to prioritize core features. Audria stressed prioritizing "quality over quantity" and "process over product," as the team needs to be able to fully justify all project decisions.
  - **Wednesday/Thursday Deliverables:**
    - **Video Pitch:** A 4-minute presentation video is due Wednesday night. It must cover project decisions and AI usage (with clear pros and cons).
    - **Extension:** If the team needs more time, they can reach out to Audria for an extension, with the latest submission by Thursday noon.
    - **Office Hours:** Scheduled for Wednesday from 6:00 PM - 7:00 PM.
  - **Code Reviews:**
    - The team needs to obtain repository access for all other Watchtower teams.
    - Every team member must participate in peer-reviewing at least 1 other Watchtower team (subject to change).
    - The code review deliverables must include shoutouts for great features and aesthetics as well as constructive feedback. This review is expected to take around 1 hour.
  - **Milestones:** The hard deadline for the final project is Tuesday of Finals Week. Midterm 2 is scheduled for Week 10.
- **Resolution / Status:** Resolved — Guidelines and schedule for the presentation video and peer reviews finalized.

### Item 3: Frontend Architectural Decisions, Wireframes, and AI Cohesiveness
- **Introduced by:** Audria (TA) / Feedback from Professor Powell
- **Discussion:**
  - **Intentional Design:** Professor Powell requested clear, intentional decisions regarding the frontend, ADR choices, framework choices, and how they connect back to users. These user-centric design connections should be clearly documented/mapped in the wireframe.
  - **Wireframe & Responsiveness:** Wireframes must show responsiveness for desktop and/or mobile layouts. Specific mobile features include accessibility considerations (e.g., a "Powlypaint day free" version for accessibility and responsiveness, and a heatmap layout mapping reachability for mobile interactions).
  - **AI Generation Inconsistencies:** Professor Powell noted that AI-generated assets and designs are easy to spot. When multiple developers generate different parts of the frontend using AI, it results in a disjointed, inconsistent aesthetic. The team needs to unify its frontend design system to create a cohesive brand.
- **Resolution / Status:** Resolved — Frontend design consistency, responsive wireframing requirements, and user connection mapping incorporated into design goals.

### Item 4: Demo Feedback and Sprint Goals
- **Introduced by:** Han Yang-Lin
- **Discussion:**
  - **Demo Review:** Han shared a demo of the current prototype. The feedback was highly positive regarding functionality, but the frontend looks a bit "iffy".
  - **Recommendations:** The team must refine frontend branding and aesthetics to be cohesive. To address concerns about progress, the team should schedule a stakeholder conversation with Professor Powell to get his direct feedback.
  - **This Sprint's Goals:**
    1. Integrate PostgreSQL as the primary database.
    2. Finish accessibility and responsive layout features.
    3. Revamp frontend branding for absolute visual cohesiveness.
    4. Implement the notification service.
- **Resolution / Status:** Resolved — Sprint goals updated to prioritize PostgreSQL integration, accessibility, cohesive branding, and notifications.

---

## Decisions Made

### Decision 1: Focus on Process and Core MVP Quality
- **Decision:** Prioritize high-quality execution of core features over adding extra, low-quality features.
- **Reasoning:** Aligning with TA feedback that "process over product" and robust, justifiable choices are key.
- **Dissenting Opinions:** None.
- **Why the group proceeded anyway:** N/A

### Decision 2: Twilio Justification in ADR
- **Decision:** Document the choice of Twilio as the SMS provider in the ADR, addressing pricing and alternative options.
- **Reasoning:** Audria requested explicit ADR documentation for external communication services.
- **Dissenting Opinions:** None.
- **Why the group proceeded anyway:** N/A

### Decision 3: Standardize Frontend Branding to Address AI Aesthetic Disjointedness
- **Decision:** Create and adhere to a unified UI/UX theme and branding style to override inconsistent AI-generated aesthetics.
- **Reasoning:** Inconsistent design generation by multiple members using AI requires a rigid central design system.
- **Dissenting Opinions:** None.
- **Why the group proceeded anyway:** N/A

---

## Deferred Items

| Item | Reason Not Discussed |
|---|---|
| Detailed PagerDuty alert architecture | Awaiting TA follow-up and team research |

---

## Action Items

| # | Task | Assigned To | Due Date | Status |
|---|---|---|---|---|
| 1 | Record and submit 4-minute presentation video (decision choices, AI pros/cons) | Nicole Sutedja / Team | Wednesday Night (latest Thursday Noon) | In progress |
| 2 | Schedule stakeholder meeting with Professor Powell for frontend/progress feedback | Nicole Sutedja | ASAP | In progress |
| 3 | Obtain repository access to other Watchtower teams and perform code review | Team | Next TA Meeting / Thursday | In progress |
| 4 | Integrate PostgreSQL database into the backend | Database Team | End of Sprint | In progress |
| 5 | Complete responsive layout wireframes & accessibility features (reachability heatmap) | Frontend Team | End of Sprint | In progress |
| 6 | Refine frontend branding & UI design for unified cohesiveness | Frontend Team | End of Sprint | In progress |
| 7 | Implement notification service & document ADR justification for Twilio | Notification Team | End of Sprint | In progress |
