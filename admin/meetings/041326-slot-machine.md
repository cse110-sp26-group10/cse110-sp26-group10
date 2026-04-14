# Team 10 - 10x Devs Meeting Minutes
---
## Meeting Info
| Field | Details |
|---|---|
| **Meeting Type** | Weekly Team Meeting |
| **Date** | April 13, 2026 |
| **Time** | ~4:00–4:40 PM (Zoom 40-min limit) |
| **Location** | Zoom (remote) |
| **Minutes Recorded By** | Evan Marriott (AI note taker) |

---
## Attendance: Mark x if Present
Team Leads
- [x] Nicole Sutedja (nsutedja@ucsd.edu)
- [x] Evan Marriott (emarriott@ucsd.edu)

Members
- [x] Hudson Gehrke (hgehrke@ucsd.edu)
- [x] Aron Wu (arw008@ucsd.edu)
- [x] Bethany Miyamoto (bmiyamoto@ucsd.edu)
- [x] Jensen Guo (jeg076@ucsd.edu)
- [x] Kaley Chung (kac101@ucsd.edu)
- [x] Xuanye Wang (xuw040@ucsd.edu)
- [x] Benedict Luis (bluis@ucsd.edu)
- [x] Han Yang-Lin (hyanglin@ucsd.edu)
- [x] Prakhar Shah (prs016@ucsd.edu) *(joined late)*

---
## Agenda
1. Review repo setup and task manager
2. AI model / tool selection for the AI Slot Machine assignment
3. Baseline run workflow and task assignments

---
## Additional Meeting Notes
- Meeting cut off at ~40 minutes due to free Zoom plan; a new meeting link was created and shared in Slack to continue
- Evan screen-shared the GitHub organization to help members locate both repositories
- Assignment is due **tomorrow, April 14 at midnight**
- This weekly meeting time will recur every week going forward
- A team member offered to host future meetings with a longer Zoom plan

---
## Old Business
*Unresolved items carried over from the previous meeting.*

### Item 1: Prior Sunday Assignments
- **Background:** Members had deliverables due the previous Sunday
- **Discussion:** Evan confirmed everything was turned in as long as everyone signed the required document
- **Resolution / Status:** Resolved — assumed complete

---
## New Business

### Item 1: GitHub Repository Structure
- **Introduced by:** Evan Marriott
- **Discussion:** Evan explained the two-repository structure inside the `cse110-sp26-group10` GitHub organization: (1) the admin/meeting-notes repo and (2) the `ai-slot-machine` project repo. The project repo contains a `prompts/` folder with `original-prompt.txt` and a `step1/` folder for baseline run outputs. Some members needed help locating the org; Evan screen-shared to walk everyone through it.
- **Resolution / Status:** Resolved — all members confirmed they could find the repo

### Item 2: AI Tool and Model Selection
- **Introduced by:** Evan Marriott / Nicole Sutedja
- **Discussion:** Initial discussion favored Claude (Sonnet 4.6) since most members use it. However, the assignment specifies using either OpenAI Codex, Claude Code, or Gemini Code Assistant — not the standard Claude chat interface. After discovering that Claude Code likely requires a paid subscription, the team switched to **OpenAI Codex** as it has a free tier. Members confirmed access to model **o4 / GPT version labeled "5.4"** on the free plan.
- **Resolution / Status:** Resolved — using **OpenAI Codex, model 5.4**

### Item 3: Reasoning Effort Level
- **Introduced by:** Team (raised during model discussion)
- **Discussion:** The assignment states to use the most advanced model and standardize all parameters. "Extra high" reasoning was considered but raised token-budget concerns for members on the free tier. Medium was proposed as a conservative middle ground that keeps all runs consistent.
- **Resolution / Status:** Resolved — using **Medium reasoning effort** for all runs

### Item 4: Baseline Run Workflow
- **Introduced by:** Evan Marriott
- **Discussion:** Each of the 5 assigned members will do 10 baseline runs (50 total). Each run should be saved in `step1/candidate-00X/` in the project repo. Members should clone the repo first and run Codex inside the `step1/` folder. The assignment requires measuring specific values (lines of code, etc.) for each run — these are tracked in the rubric Nicole created. To reduce burden, runners will focus on generating the 10 candidates, and other members will fill in the rubric data after the runs are committed. Each runner should also select their best candidate from their 10 runs; the top 5 will be compiled as final candidates.
- **Resolution / Status:** Resolved — workflow confirmed, team asked to start immediately

### Item 5: Video Presentation
- **Introduced by:** Prakhar Shah
- **Discussion:** Assignment requires a video presentation, no longer than 4 minutes. Evan confirmed no face-on-camera requirement — a screen recording with voiceover is sufficient.
- **Resolution / Status:** Resolved

---
## Decisions Made

### Decision 1: Use OpenAI Codex (model 5.4) instead of Claude
- **Decision:** Switch from Claude Sonnet 4.6 to OpenAI Codex model 5.4
- **Reasoning:** The assignment requires an agentic coding tool (Codex, Claude Code, or Gemini Code Assistant), not the standard Claude chat UI. Codex has a free tier accessible to all members; Claude Code likely requires a paid subscription.
- **Dissenting Opinions:** None formally raised after the clarification
- **Why the group proceeded anyway:** N/A

### Decision 2: Use Medium reasoning effort
- **Decision:** Standardize all Codex runs on Medium reasoning effort
- **Reasoning:** Extra High reasoning consumes significantly more tokens and could exhaust free-tier limits before all 50 runs are complete. The assignment doesn't mandate a specific level, only consistency across runs.
- **Dissenting Opinions:** Some uncertainty about whether higher effort was required; assignment language was reviewed live
- **Why the group proceeded anyway:** Assignment says to standardize parameters, not that Extra High is mandatory; Medium preserves token budget for all members

### Decision 3: Split baseline run responsibilities
- **Decision:** The 5 assigned runners generate 10 candidates each; a separate group fills in rubric measurements after runs are pushed
- **Reasoning:** Reduces cognitive load on runners and lets the rubric work be done in parallel/after, speeding up overall completion
- **Dissenting Opinions:** None
- **Why the group proceeded anyway:** N/A

---
## Deferred Items

| Item | Reason Not Discussed |
|---|---|
| Final selection of top 5 candidates | Runs not yet complete; will be done after all 50 runs are committed |
| Token budget / what to do if members hit Codex free-tier limits | Time ran out; fallback of splitting 10 runs into 5 each was mentioned but not finalized |

---
## Action Items

| # | Task | Assigned To | Due Date | Status |
|---|---|---|---|---|
| 1 | Write README | Nicole Sutedja | Apr 13 (today) | ✅ Completed during meeting |
| 2 | Write and finalize rubric (including all measurement criteria from assignment) | Nicole Sutedja | Apr 13 (today) | ✅ Completed during meeting |
| 3 | Complete 10 baseline Codex runs each; save as `step1/candidate-00X/`; push to repo | 5 assigned members (per task manager) | Apr 13–14 | In Progress |
| 4 | Fill in rubric measurements for all committed runs | Remaining members (per task manager) | Apr 14 | Not Started |
| 5 | Select best candidate from personal 10 runs; provide brief reasoning | Each baseline runner | Apr 14 | Not Started |
| 6 | Compile final top 5 candidates from submitted selections | Evan Marriott / Nicole Sutedja | Apr 14 | Not Started |
| 7 | Record video presentation (screen + voiceover, ≤4 min) | Assigned member (per task manager) | Apr 14 midnight | Not Started |
| 8 | Investigate hosting longer Zoom meetings for future weeks | Volunteer (offered during meeting) | Before next meeting | Not Started |
