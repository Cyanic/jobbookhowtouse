# Job Book Script Series Specification

## Purpose

This document defines the standards and structure for generating scripts in the **Job Book How to Use Series**, a 13-episode YouTube training sequence.  
Each script should maintain consistent tone, pacing, and instructional depth, following the established style of completed scripts (Intro, Dashboard, Clients, Jobs, and previous scripts).

---

## Scope and Output

Each script is a talking head text intended for use with teleprompter software.  
Scripts are written in plain text (Markdown-compatible) and do not include scene directions, camera notes, or visual annotations beyond on-screen action cues.

---

## Audience

**Primary Users**

The video series is designed for Job Book users, including:

- **Technicians** – Complete Daily Work Records (DWRs) and submit expenses.
- **Project Managers** – Track job progress, monitor costs, approve DWRs and expenses.
- **Administrators / Job Coordinators** – Manage clients, jobs, invoices, reports, and approvals.
- **Owners / Managers** – Oversee approvals, reporting, and company-wide performance.
  These roles define the intended viewers, not the narrator’s role.

---

## Narration Persona

Scripts are written in first person, but from the perspective of a Job Book trainer — an expert explaining how the system works, not a field user performing real work.
The narrator demonstrates actions as examples rather than as actual workflow participation.

Tone: confident, conversational, and precise — similar to a knowledgeable instructor guiding a tutorial.
The narrator speaks directly to the viewer (“you”) and refers to their own actions (“I’m logged in as an Administrator”).
Address the viewer in the singular (“you”), and use calm, confident phrasing focused on clarity.

Avoid phrasing that suggests the narrator is a Land Surveyor or project team member.

---

## Script Format

Each episode follows this sequence:

1. **Series Hook (Standard Introduction)** –

   ```
   Welcome back to the Job Book How to Use Series.
   If this is your first time watching,
   remember that each episode builds on the last.
   ```

   _(Skip this section for Episode 1.)_

2. **Previous Episode Reference** –  
   Briefly summarize what was covered in the last video and how it connects here.

   ```
   In the last video we explored the...
   ```

3. **Episode Introduction** –  
   State the topic and purpose of this episode.

4. **Explain the Why** –  
   Establish why this feature or workflow matters to the viewer’s role.

5. **Show the How** –  
   Walk through the steps in Job Book. Use clear on-screen cues  
   (`-- Click Save --`, `-- Add Job --`) for major actions.

6. **Explain Integration** –  
   Describe how this feature connects to the broader Job Book workflow  
   (e.g., how DWRs feed invoices or approvals).

7. **Best Practices** –  
   Highlight efficiency tips, role-specific guidance, and common mistakes to avoid.

8. **Series Continuity** –  
   Prepare the viewer for the next topic with a transition line  
   (“In the next video, we’ll look at…”).

9. **Outro** –  
   End confidently, reaffirming the skill learned and encouraging continued viewing.

10. **Final Lines** –

```
Thanks for watching, and I’ll see you in the next video!
And don’t forget to subscribe for more Job Book updates
and helpful how-to videos!
```

Target length: **700–1400 words** (≈2–8 minutes spoken).

The narrator is a Job Book trainer demonstrating features to survey company staff, not a Land Surveyor using the system in production.

---

## On-Screen Action Cues

Use double dashes and imperative form for all visible interface actions.  
Each cue should appear on its own line.

Examples:

```
-- Click Add Client --
-- Select Rate Sheet --
-- Press Save --
```

These lines mark visual steps for editors and should be easily searchable in text.

---

## Episode Metadata

Each script begins with a metadata header:

```
# Episode [#] – [Title]
**Series:** Job Book How to Use
**Target Roles:** [e.g., Technician, Administrator]
**Task:** [Concise one-sentence summary of what the episode demonstrates]
**Length:** 800–1200 words
**Previous:** [Title of previous episode]
**Next:** [Title of next episode]
**Tags:** [Dashboard, Technician, Workflow]
```

**Task Field Definition:**  
A one-sentence summary of what the narrator will demonstrate and explain in the episode.  
Begin with an action verb (“Show,” “Demonstrate,” “Walk through,” “Explain”) and limit to two lines.

---

## Video Order / Playlist (13 Episodes)

1. **Intro** – Series purpose, prerequisites (Setup Series), overview of daily workflows.
2. **Dashboard** – Technician vs. Administrator dashboards and cards.
3. **Creating Clients** – Required vs. optional fields, contacts, deactivation vs. deletion.
4. **Creating Jobs** – Job details, rate sheets, cloning, and best practices.
5. **Creating DWRs** – Technician workflow: labour, equipment, materials.
6. **Creating Expenses** – Technician workflow for expense submissions.
7. **Active Job Dashboard** – Viewing, filtering, and monitoring jobs.
8. **DWR Approval Backlog** – Approving submitted DWRs efficiently.
9. **Expense Approval Backlog** – Reviewing and approving expenses.
10. **DWR Invoice Backlog** – Converting approved DWRs into invoices.
11. **Creating Invoices** – Invoice types, editing, and summaries.
12. **Invoice Process Backlog** – Exporting to accounting systems (QuickBooks, Sage).
13. **Next Steps** – Series recap and links to advanced modules.

---

## Script Style

- Written for spoken narration—simple sentences, natural rhythm.
- Use transitions between topics (“Now that we’ve created a client, let’s connect it to a job”).
- Reference the **Job Book How to Setup Series** or earlier **How to Use** episodes when helpful.
- Include **role callouts** (“I’m logged in as a Project Manager”) to clarify context.
- Integrate **best practices** and avoid listing every button or icon.
- Avoid UI details that may change (colors, icon shapes, menu order).
- Use natural pacing: one idea per sentence, short paragraphs (1–3 sentences).
- Insert blank lines where natural pauses occur for teleprompter readability.
- End every script with a **forward transition** to the next video.

---

### Line Formatting

Break text into logical line lengths, ideally **no longer than 80 characters per line**.
Do not hard-wrap at exactly 80 characters—wrap naturally at clause or phrase boundaries
to preserve readability.

When generating or revising scripts, preserve all existing line breaks unless they clearly violate
the line length or readability guidelines.

Do not merge or collapse short lines together.

Do not reflow text that is already properly formatted into 3–4 line paragraphs.

Treat each existing line break as intentional for teleprompter pacing.

Treat each line break as a soft wrap for teleprompter display.
Avoid single paragraphs that extend beyond 3–4 lines.

---

## Background Information

When generating a script, use the following sources to ensure accuracy and continuity:

1. **Job Book Help Documentation**

   - Primary reference: ./Reference/jobbook-help-documents.md
   - Use it to confirm terminology (menu names, field labels, feature names), workflow order, and user-role responsibilities.
   - Mirror the functional language used in the Help documentation, but rewrite it in a natural spoken-narration style.
   - Any references to image files can be ignored as they are not in this repository.

2. **Previous Scripts in the Series**

   - Always review the scripts that precede the current one (e.g., when generating Episode 2.8, review Episodes 2.1–2.7).
   - Extract context such as:
     - How features were introduced and explained.
     - Transitions or references used between videos.
     - Terminology and tone patterns.
   - Reuse established phrases and continuity hooks for consistency across episodes.

3. **Role Context**

   - Use audience and role definitions from this specification to ground examples (Technician, Project Manager, etc.).
   - Maintain the same role behavior as described in prior scripts — e.g., if a Technician creates DWRs in one episode, keep that consistent.

4. **Edge Cases**
   - For Episode 1 (Intro): no prior scripts — base context solely on this specification and Setup Series references.
   - For the final episode (Next Steps): summarize and link forward to upcoming “Reporting Guide” or advanced modules.

**Goal:**  
Ensure each script draws from existing Job Book documentation and previously written episodes to maintain consistent workflow descriptions, vocabulary, and teaching rhythm.

---

## Episode Transitions

**Opening Transition:**

> “In the previous video, we created a client. Now we’ll connect that client to a job.”

**Closing Transition:**

> “In the next video, we’ll start entering daily work records for this job.”

Use these as clear linguistic markers for viewers and editors.

---

## Constraints

| **Do**                            | **Don’t**                                           |
| --------------------------------- | --------------------------------------------------- |
| Begin with a continuity statement | Describe UI colors or icons                         |
| Identify target role(s) early     | Use filler language (“basically,” “as you can see”) |
| State purpose clearly             | Over-explain login or setup steps                   |
| Include on-screen cues            | Mention internal configurations                     |
| End with next-episode link        | Use overly formal or marketing tone                 |

---

## Success Criteria

A generated or written script is considered valid if it meets all of the following:

- **Length:** 800–1000 words (±20%).
- **Structure:** Matches the required format and flow.
- **Voice:** First-person instructional, confident tone.
- **Continuity:** References previous episode and introduces next.
- **Role Inclusion:** At least one mention of narrator’s current role.
- **On-Screen Actions:** Minimum of three cues using the `-- Action --` format.
- **Best Practices:** At least one role-based efficiency tip or warning.
- **Completeness:** Can stand alone but fits within the playlist sequence.

---

## Testing & Review

Before finalization, use this checklist:

☐ References previous and next episode
☐ Establish why this feature matters
☐ Contains ≥3 on-screen cues  
☐ Includes at least one best-practice statement  
☐ Tone matches narrator persona  
☐ Transitions read smoothly aloud

Additional review steps:

1. **Read Aloud Test:** Verify pacing and spoken clarity.
2. **UI Validation:** Confirm menu names and button labels match current Job Book interface.
3. **Continuity Check:** Ensure episode references align correctly.

---

## File Naming Convention

Use the following format for all script files:  
`2.[#]_[ShortTitle]_Transcript.md`  
Example: `2.4_Creating_Jobs_Transcript.md`

---

## Optional: Series Continuity Matrix

Use this to cross-reference dependencies between episodes:

| From                    | Leads To           | Connection                          |
| ----------------------- | ------------------ | ----------------------------------- |
| Clients                 | Jobs               | Jobs link to client records         |
| Jobs                    | DWRs               | DWRs connect to jobs                |
| DWRs                    | DWR Approvals      | Workflow for manager review         |
| DWR Approvals           | Invoicing          | Approved DWRs flow into billing     |
| Expenses                | Expense Approvals  | Workflow for administrator review   |
| Expense Approvals       | Invoicing          | Approved Expenses flow into billing |
| DWR Invoice Backlog     | Creating Invoices  | Exporting data to accounting        |
| Invoices                | Exporting Invoices | Exporting data to accounting        |
| Invoice Process Backlog | Next Steps         | Closeout and advanced features      |

---

## Example Header Templates

# Episode 1 – Intro

**Series:** Job Book How to Use  
**Target Roles:** All staff
**Task:** Introduce the Job Book How to Use Series, prerequisites (Setup Series), outline daily workflows (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices), explain short focused episodes, and point to Reporting Guide for advanced features.
**Previous:** N/A
**Next:** Dashboard

---

# Episode 2 – Dashboard

**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator, Project Manager, and Techniction
**Task:** Show Technician dashboard (My Tasks, DWRs, Expenses, Personal Reports) and Administrator dashboard (Clients, Jobs, Workflow, Reports, Rate Sheets, Leave, Assets, Safety, Job Maps). Include role restrictions and best practices.
**Previous:** Intro
**Next:** Creating Clients

---

# Episode 3 – Creating Clients

**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator
**Task:** Show creating a client (required fields, optional fields, contacts, addresses, attachments), editing clients, deactivation vs. deletion. Emphasize best practices and prerequisites.
**Previous:** Dashboard
**Next:** Creating Jobs

---

# Episode 4 – Creating Jobs

**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator
**Task:** Walk through creating a job: job number, client, locations, contacts, project manager, billing type, invoice type, rate sheets, line items, budget quantities. Show editing, cloning, and deactivation best practice.
**Previous:** Creating Clients  
**Next:** Creating DWRs

---

# Episode 5 – Creating Daily Work Records (DWRs)

**Series:** Job Book How to Use  
**Target Roles:** Technician
**Task:** Demonstrate creating a DWR: adding labour, equipment, materials, saving, and editing. Explain why DWRs are essential and tie them back to jobs.
**Previous:** Creating Jobs  
**Next:** Creating Expenses

---

# Episode 6 – Creating Expenses

**Series:** Job Book How to Use  
**Target Roles:** Technician
**Task:** Show how to create and submit an expense, attach it to a job, and explain reimbursement workflow. Emphasize accuracy and best practices.
**Previous:** Creating Daily Work Records (DWRs)  
**Next:** Active Job Dashboard

---

# Episode 7 – Active Job Dashboard

**Series:** Job Book How to Use  
**Target Roles:** Project Manager
**Task:** Show how to view the Active Job Dashboard, monitor job status, PO amounts, due dates, and use filters. Explain how managers use it for real-time oversight.
**Previous:** Creating Expenses
**Next:** DWR Approval Backlog

---

# Episode 8 – DWR Approval Backlog

**Series:** Job Book How to Use  
**Target Roles:** Manager, Administrator
**Task:** Show how to use the DWR Approval Backlog to review and approve submitted DWRs. Explain best practices for timely approvals and workflow impact.
**Previous:** Active Job Dashboard  
**Next:** Expense Approval Backlog

---

# Episode 9 – Expense Approval Backlog

**Series:** Job Book How to Use  
**Target Roles:** Manager
**Task:** Show how to review and approve expenses, identify errors, and manage the Expense Approval Backlog. Emphasize best practices.
**Previous:** DWR Approval Backlog  
**Next:** DWR Invoice Backlog

---

# Episode 10 – DWR Invoice Backlog

**Series:** Job Book How to Use  
**Target Roles:** Administrator, Manager
**Task:** Show how to convert approved DWRs for T&M jobs into invoices. Explain workflow, options, and best practices.
**Previous:** Expense Approval Backlog  
**Next:** Creating Invoices

---

# Episode 11 – Creating Invoices

**Series:** Job Book How to Use  
**Target Roles:** Administrator
**Task:** Show how to create invoices manually or from jobs. Explain invoice type (Ticket/Invoice vs. Invoice), line item type (Detailed vs. Summarized), and editing.
**Previous:** DWR Invoice Backlog  
**Next:** Invoice Process Backlog

---

# Episode 12 – Invoice Process Backlog

**Series:** Job Book How to Use  
**Target Roles:** Administrator
**Task:** Show how to export invoices to QuickBooks or Sage using Invoice Process Backlog. Explain process and best practices.
**Previous:** Creating Invoices  
**Next:** Next Steps

---

# Episode 13 – Next Steps

**Series:** Job Book How to Use  
**Target Roles:** All staff
**Task:** Summarize what’s been covered (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices). Reinforce user confidence. Point to Reporting Guide Series and advanced modules (Tasks, Leave, Assets, Safety).
**Previous:** Exporting Invoices  
**Next:** Job Book Advanced Reporting Series

---

## End of Specification
