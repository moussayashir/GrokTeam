# Grokteam – Collaborative Teamwork System with Grok  
**GitHub Repository:** `https://github.com/moussayashir/Grokteam`  
**Author:** Moussa Yashir (moussayashir)  
**Version:** v1.1 – Completed header and req table. First revision.  

## Goal
Transform Grok from an automatic answer engine into an active participant in a human-AI team.

## Objectives
Grokteam will be achieved by creating software external to Grok AI, that manages the interaction with Grok and has the following objectives: **control, transparency and accuracy, feedback loops, external tool integration, and broad coverage**.

## General Instructions
1. **Teamwork oriented discussions:** Throughout each discussion, the AI responses will always be oriented to teamwork with a human, in a natural discussive way (short tracked responses and confirmation).

2. **Branch and topic tracking:** The overall discussion and its branches will be followed by the Grokteam software, tracking topics discussed and planned to be discussed.

3. **Discussion stages:**
   - **Stage I** – Initial discussion stage.
   - **Stage II** – Execution plan discussion stage.
   - **Stage III** – Execution stage.
   - **Stage IV** – Presentation stage.

4. **Aquiral repository:** The program will keep a repository of used sources and tools (internal and external) per subject of discussion.

5. **Confirm-Gated Discussion** – **Short Name:** `confirm-gated discussion`  
   - Discussion that **proceeds only after explicit user confirmation**.  
   - **Rule:** Everywhere "discussion" appears in requirements, it **implies** `confirm-gated discussion`.  
   - No action taken without **separate previous consent**.  
   - **Emphasize** for high-impact (tool execution, storage, text changes).

**Note:** Grokteam tracks state of each **discussion stage** and **topic** as: `{planned, current, completed, skipped, done}`.  
Branch tracking will be added in the future, including identifying conversation branches going off the main topic or discussing side tracks. A view of the discussion tree with its branches and states will be available in the Grokteam UI and stored in the Grokteam repositories.

## Future Features
- **Branch headline and discussion tree tracking** – Tree of discussions, branches, and states.

## Directives
The goal objectives will be achieved using the following directives:

| # | Objective                 | Directives                                                                | 
|---|---------------------------|-------------------------------------------------------------------------- |
| 1 | Managed externally        | External program for tracking activity and discussion stage               |
| 2 | Control                   | Clarification discussion, Execution after confirmation, Discussion stages |
| 3 | Transparency and Accuracy | Response-format discussion, Raw data protected from AI, Resource report, External source discussion and confirmation, Source repository |
| 4 | Teamwork (Feedback loops) | Answer breakdown, Short steps, Tracking topics, Confirmation |
| 5 | External tool integration |  external tools with repository, execute after approval      |
| 6 | Broad coverage            | Track branching discussions with resumable topics            |

---

## 0. General Requirements Table

| #     | Short Name                        | Goal                    | Brief Description (Outcome)                                               | Status           |
|-------|-----------------------------------|-------------------------|---------------------------------------------------------------------------|------------------|
| 0.1   | `External JS Chrome add-on`       | Manage                  | External (JS Chrome add-on) tracks stages/topics, follows chat, modifies prompts with missing info, manages external calls | Pending Approval |
| 0.1.1 | `Track discussion stages`         | Manage                  | Stages tracked and displayed in header                                    | Pending Approval |
| 0.1.2 | `Follow chat`                     | Manage                  | Real-time chat monitoring                                                 | Pending Approval |
| 0.1.3 | `Modify prompts`                  | Manage                  | Prompts auto-updated with missing stage/topic info                        | Pending Approval |
| 0.1.4 | `Manage external calls`           | Manage                  | Handles tool calls with logging                                           | Pending Approval |
| 0.2   | `Natural Discussion`              | Teamwork                | Natural, collaborative dialogue                                           | Pending Approval |
| 0.2.1 | `Give short responses`            | Teamwork                | Responses limited to short, focused steps                                 | Pending Approval |
| 0.2.2 | `Track response topics`           | Teamwork                | Topics (given/planned) tracked and listed                                 | Pending Approval |
| 0.2.3 | `Confirm before proceed`          | Teamwork                | User must confirm before next response or action                          | Pending Approval |
| 0.3   | `Track discussion stages`         | Control                 | Stage state and result tracked in JSON                                    | Pending Approval |
| 0.3.1 | `Stage in response header`        | Control                 | Current stage shown in every AI response                                  | Pending Approval |
| 0.3.2 | `Track stage state`               | Control                 | State: {planned, current, completed, skipped}                             | Pending Approval |
| 0.3.3 | `Store stage result`              | Control                 | Result saved as JSON object                                               | Pending Approval |

---

## 1. Stage I – Initial Discussion Requirements

| #   | Short Name                          | Goal                    | Brief Description (Outcome)                                               | Status           |
|-----|-------------------------------------|-------------------------|---------------------------------------------------------------------------|------------------|
| 1.1 | `User initiated prompt`             | Control                 | Capture initial user request                                              | Pending Approval |
| 1.2 | `Topic choice discussion`           | Control                 | `confirm-gated discussion` → agreed main topic                            | Pending Approval |
| 1.3 | `Intent clarifications`             | Control                 | `confirm-gated discussion` → clarified user intent                       | Pending Approval |
| 1.4 | `Goals and approach discussion`     | Control                 | `confirm-gated discussion` → agreed goals and approach                    | Pending Approval |

---

## 2. Stage II – Execution Plan Requirements

| #     | Short Name                                  | Goal                    | Brief Description (Outcome)                                               | Status           |
|-------|---------------------------------------------|-------------------------|---------------------------------------------------------------------------|------------------|
| 2.1   | `Acquisition means`                         | External integration    | Tools and sources selected and stored                                     | Pending Approval |
| 2.1.1 | `Discuss acquisition means`                 | External integration    | `confirm-gated discussion` → select tools/sources                         | Pending Approval |
| 2.1.2 | `Store confirmed means in repository`       | Transparency            | Save approved tools and params                                            | Pending Approval |
| 2.2   | `Data accuracy planning`                    | Transparency            | Accuracy needs, format, and plan agreed                                   | Pending Approval |
| 2.2.1 | `Identify data accuracy needs`              | Transparency            | `confirm-gated discussion` → define accuracy requirements                | Pending Approval |
| 2.2.2 | `Determine protected data format`           | Transparency            | `confirm-gated discussion` → agree on JSON/table format                   | Pending Approval |
| 2.2.3 | `Determine data acquisition plan`           | Control                 | `confirm-gated discussion` → plan steps, tools, params                    | Pending Approval |
| 2.2.4 | `Store confirmed plans in repository`       | Transparency            | Save full acquisition plan                                                | Pending Approval |
| 2.3   | `Agree on execution steps`                  | Control                 | Execution mode and steps confirmed                                        | Pending Approval |
| 2.3.1 | `Bulk or step-by-step`                      | Control                 | Decide execution mode                                                     | Pending Approval |
| 2.3.2 | `Discuss each step if bulk`                 | Control                 | `confirm-gated discussion` → review all steps                             | Pending Approval |
| 2.3.3 | `Store execution plan in repository`        | Transparency            | Save final execution plan                                                 | Pending Approval |

---

## 3. Stage III – Execution Requirements

| #   | Short Name                                  | Goal                    | Brief Description (Outcome)                                               | Status           |
|-----|---------------------------------------------|-------------------------|---------------------------------------------------------------------------|------------------|
| 3.1 | `Confirm each step before execution`        | Control                 | **User must confirm** before any step runs                                | Pending Approval |
| 3.2 | `Bulk execution confirmation`               | Control                 | Confirm which steps run in bulk                                           | Pending Approval |
| 3.3 | `Track execution and handle errors`         | Control                 | Log results, discuss errors                                               | Pending Approval |
| 3.4 | `Pass protected data back to Grok`          | Transparency            | Return raw data in agreed format with instructions                        | Pending Approval |

---

## 4. Stage IV – Presentation Requirements

| #   | Short Name                                  | Goal                    | Brief Description (Outcome)                                               | Status           |
|-----|---------------------------------------------|-------------------------|---------------------------------------------------------------------------|------------------|
| 4.1 | `Save full result`                          | Transparency            | Result stored and link shown to user                                      | Pending Approval |
| 4.2 | `Plan result-presentation steps`            | Teamwork                | Break result into topical presentation steps                              | Pending Approval |
| 4.3 | `Present summary and begin steps`           | Teamwork                | Quick summary + start result-presentation steps                           | Pending Approval |
| 4.4 | `Step discussion`                           | Teamwork                | `confirm-gated discussion` per result-presentation step                   | Pending Approval |
| 4.5 | `Large data display`                        | Usability               | Full texts, links in Grokteam tabs                                        | Pending Approval |

---

## Technical Requirements

### JS Chrome Add-on Requirements
- **Platform:** Chrome Extension (Manifest V3)
- **Permissions:** `activeTab`, `storage`, `scripting`, `webNavigation`, `declarativeContent`
- **Content Scripts:** Inject into `grok.x.ai` and `chat.x.ai`
- **Background Service Worker:** Persistent state, message passing
- **UI:** Popup panel + side panel (optional)
- **Storage:** `chrome.storage.local` for session data, IndexedDB for large logs
- **Communication:** `chrome.runtime.sendMessage` between content, popup, and background
- **Prompt Injection:** Modify outgoing messages to include stage/topic/state context
- **External Tool Handling:** Intercept and route tool calls via background worker
- **Security:** No external network calls without user consent

---

## Frameworks & Libraries
> **To be determined** – Will be selected during implementation phase based on performance, size, and compatibility.

---

// Todo:  Update next sections according to the text above
