# Grokteam – Collaborative Teamwork System with Grok  
**GitHub Repository:** `https://github.com/moussayashir/Grokteam`  
**Author:** Moussa Yashir (moussayashir)  
**Version:** v1.0 Initial requirements. With Moshe's revisions. To be compared with Grok's coming revision.  

## Goal
Transform Grok from an automatic answer engine into an active participant in a human-AI team.

## Objectives
Grokteam will be achieved by creating software external to Grok AI, that manages the interaction with Grok and has the following objectives: **control, transparency and accuracy, feedback loops, external tool integration, and broad coverage**.

## General requirements
1. **Teamwork oriented discussions:** Throughout each discussion, the AI responses will always be oriented to teamwork with a human, in a natural discussive way (short tracked responses and confirmation).

2. **Branch and topic tracking:** The overall discussion and its branches will be followed by the Grokteam software, tracking topics discussed and planned to be discussed. 

3. **Discussion stages:**: Each discussion will have the following stages:     
3.1 Intent - Discussion to determine the current team's project subject, main objective, and goals.  
3.2 Execution plan - Discussion to determine how these goals will be achieved.  
3.3 Execution - Discussion by which the plan will be executed in consecutive confirmed steps.  
3.4 Presentation - Presenting and discussing the results.  

4. **Aquiral repository:** The program will keep a repository of used sources and tools (internal and external) per subject of discussion. 

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

## Approved Requirements

| # | Stage | Short Name | Goal | Brief Description | Status |
|---|-------|------------|------|-------------------|--------|
| 1 | All   | `Track discussion` | Manage | External program (JS add-on) keeps track of discussion stages and topics, follows the chat, modifies prompts with any missing topic and stage info, and manages external calls. | Pending Approval | 
| 2 | 1     | `Agree on topic` | Control | Initial discussion to present the topic, clarify intent, and agree on goals and approach. **No progress without full agreement.** | Approved |
| 3 | All   | `Protected JSON output` | Transparency | Present external data protected from AI changes, previewed in a table using JSON, only after structure discussion. | Approved |
| 4 | 4     | `Result Discussion` | Teamwork | Break response into short steps, track response steps, advance only after confirmed.  | Pending Approval |
| 5 | 2,3,4 | `Run external tools` | When needed suggest external tools to run, execute upon user approval, present result in protected format. | Pending Approval |
| 6 | All   | `Source Repository`  | Report and store approved sources of information and aquiral tools including params | Pending approval |

---

// Todo:  Update next sections according to the text above

### Requirement #1 – `agree on topic`

**Process:**  
1. User presents the topic  
2. Grok asks clarifying questions  
3. Continue until **full mutual agreement** on:  
   - What is being sought  
   - Which source  
   - Desired outcome  
4. Only then proceed to #2 or #3  

**Example:**  
> User: "I want Ibn Ezra’s commentary on 'ויוציאו דבת הארץ'"  
> Grok: "Which edition? Sefaria? Manuscript? Also include Joseph’s verse?"  
> → Continue until clear

---

### Requirement #2 – `protected JSON output`

**Format:** JSON  
**Display:** Table in WikiText (RTL)  
**Protected Zone:** `<pre><code class="protected-json">...</code></pre>` – **Grok must not edit or interpret**  

**Process:**  
1. Plan the structure of the protected data  
2. Back-and-forth discussion until structure is agreed  
3. Extract data into the agreed template  
4. Display in table  
5. **User approval** before continuing  

**Example:**
```json
{
  "source": "Sefaria",
  "ref": "Numbers 13:32",
  "text": "ויוציאו דבת הארץ אשר תרו אתה אל בני ישראל..."
}
