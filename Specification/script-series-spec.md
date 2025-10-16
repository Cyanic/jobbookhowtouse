# Job Book Script Series Specification

## Purpose
This document defines the standards and structure for generating scripts in the **Job Book How to Use Series**, a 13-episode YouTube training sequence.  
Each script should maintain consistent tone, pacing, and instructional depth, following the established style of completed scripts (Intro, Dashboard, Clients, Jobs).

---

## Scope and Output
Each script is a complete voice-over narration text intended for use with video editing or teleprompter software.  
Scripts are written in plain text (Markdown-compatible) and do not include scene directions, camera notes, or visual annotations beyond on-screen action cues.

---

## Audience
**Primary Users**
- **Technicians** – Complete Daily Work Records (DWRs) and submit expenses.  
- **Project Managers** – Track job progress, monitor costs, approve DWRs and expenses.  
- **Administrators / Job Coordinators** – Manage clients, jobs, invoices, reports, and approvals.  
- **Owners / Managers** – Oversee approvals, reporting, and company-wide performance.

---

## Narration Persona
All videos are narrated in **first person** by a knowledgeable Job Book trainer.  
The tone is **confident, conversational, and practical**—neither overly casual nor corporate.  
The narrator speaks directly to the viewer (“you”) and refers to their own actions (“I’m logged in as an Administrator”).  
Address the viewer in the singular (“you”), avoid greetings or sign-offs, and use calm, confident phrasing focused on clarity.

Avoid filler phrases and unnecessary enthusiasm; focus on precision and confidence.

---

## Script Format
Each episode follows this sequence:

1. **Introduction** – State topic and purpose of the episode.  
2. **Reference Previous Video** – Connect back to what was just covered.  
3. **Explain the Why** – Establish why this feature matters.  
4. **Show the How** – Step-by-step walkthrough.  
5. **Explain Integration** – Describe how it connects to the broader Job Book workflow.  
6. **Best Practices** – Highlight efficiency tips and common mistakes.  
7. **Series Continuity** – Tie into next episode.  
8. **Outro** – End confidently and transition forward.

Target length: **800–1000 words** (≈3–6 minutes spoken).

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
**Length:** 800–1000 words  
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
12. **Importing Invoices** – Exporting to accounting systems (QuickBooks, Sage).  
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

## Episode Transitions
**Opening Transition:**  
> “In the previous video, we created a client. Now we’ll connect that client to a job.”

**Closing Transition:**  
> “In the next video, we’ll start entering daily work records for this job.”

Use these as clear linguistic markers for viewers and editors.

---

## Constraints

| **Do** | **Don’t** |
|---------|------------|
| Begin with a continuity statement | Describe UI colors or icons |
| Identify target role(s) early | Use filler language (“basically,” “as you can see”) |
| State purpose clearly | Over-explain login or setup steps |
| Include on-screen cues | Mention internal configurations |
| End with next-episode link | Use overly formal or marketing tone |

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

| From | Leads To | Connection |
|------|-----------|-------------|
| Clients | Jobs | Jobs link to client records |
| Jobs | DWRs | DWRs connect to jobs |
| DWRs | DWR Approvals | Workflow for manager review |
| DWR Approvals | Invoicing | Approved DWRs flow into billing |
| Expenses | Expense Approvals | Workflow for administrator review |
| Expense Approvals | Invoicing | Approved Expenses flow into billing |
| DWR Invoice Backlog | Creating Invoices | Exporting data to accounting |
| Invoices | Importing Invoices | Exporting data to accounting |
| Importing Invoices | Next Steps | Closeout and advanced features |

---

## Example Header Templates

# Episode 1 – Intro
**Series:** Job Book How to Use  
**Target Roles:** All staff
**Task:** Introduce the Job Book How to Use Series, prerequisites (Setup Series), outline daily workflows (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices), explain short focused episodes, and point to Reporting Guide for advanced features.
**Length:** ~850 words  
**Previous:** N/A
**Next:** Dashboard

---

# Episode 2 – Dashboard
**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator, Project Manager, and Techniction
**Task:** Show Technician dashboard (My Tasks, DWRs, Expenses, Personal Reports) and Administrator dashboard (Clients, Jobs, Workflow, Reports, Rate Sheets, Leave, Assets, Safety, Job Maps). Include role restrictions and best practices.
**Length:** ~850 words  
**Previous:** Intro
**Next:** Creating Clients

---

# Episode 3 – Creating Clients
**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator
**Task:** Show creating a client (required fields, optional fields, contacts, addresses, attachments), editing clients, deactivation vs. deletion. Emphasize best practices and prerequisites.
**Length:** ~850 words  
**Previous:** Dashboard
**Next:** Creating Jobs

---

# Episode 4 – Creating Jobs
**Series:** Job Book How to Use  
**Target Roles:** Administrator, Job Coordinator
**Task:** Walk through creating a job: job number, client, locations, contacts, project manager, billing type, invoice type, rate sheets, line items, budget quantities. Show editing, cloning, and deactivation best practice.
**Length:** ~850 words  
**Previous:** Creating Clients  
**Next:** Creating DWRs

---

# Episode 5 – Creating Daily Work Records (DWRs)
**Series:** Job Book How to Use  
**Target Roles:** Technician
**Task:** Demonstrate creating a DWR: adding labour, equipment, materials, saving, and editing. Explain why DWRs are essential and tie them back to jobs.
**Length:** ~850 words  
**Previous:** Creating Jobs  
**Next:** Creating Expenses

---

# Episode 6 – Creating Expenses
**Series:** Job Book How to Use  
**Target Roles:** Technician
**Task:** Show how to create and submit an expense, attach it to a job, and explain reimbursement workflow. Emphasize accuracy and best practices.
**Length:** ~850 words  
**Previous:** Creating Daily Work Records (DWRs)  
**Next:** Active Job Dashboard

---

# Episode 7 – Active Job Dashboard
**Series:** Job Book How to Use  
**Target Roles:** Project Manager
**Task:** Show how to view the Active Job Dashboard, monitor job status, PO amounts, due dates, and use filters. Explain how managers use it for real-time oversight.
**Length:** ~850 words  
**Previous:** Creating Expenses 
**Next:** DWR Approval Backlog

---

# Episode 8 – DWR Approval Backlog
**Series:** Job Book How to Use  
**Target Roles:** Manager, Administrator
**Task:** Show how to use the DWR Approval Backlog to review and approve submitted DWRs. Explain best practices for timely approvals and workflow impact.
**Length:** ~850 words  
**Previous:** Active Job Dashboard  
**Next:** Expense Approval Backlog

---

# Episode 9 – Expense Approval Backlog
**Series:** Job Book How to Use  
**Target Roles:** Manager
**Task:** Show how to review and approve expenses, identify errors, and manage the Expense Approval Backlog. Emphasize best practices.
**Length:** ~850 words  
**Previous:** DWR Approval Backlog  
**Next:** DWR Invoice Backlog

---

# Episode 10 – DWR Invoice Backlog
**Series:** Job Book How to Use  
**Target Roles:** Administrator, Manager
**Task:** Show how to convert approved DWRs for T&M jobs into invoices. Explain workflow, options, and best practices.
**Length:** ~850 words  
**Previous:** Expense Approval Backlog  
**Next:** Creating Invoices

---

# Episode 11 – Creating Invoices
**Series:** Job Book How to Use  
**Target Roles:** Administrator
**Task:** Show how to create invoices manually or from jobs. Explain invoice type (Ticket/Invoice vs. Invoice), line item type (Detailed vs. Summarized), and editing.
**Length:** ~850 words  
**Previous:** DWR Invoice Backlog  
**Next:** Importing Invoices

---

# Episode 12 – Importing Invoices
**Series:** Job Book How to Use  
**Target Roles:** Administrator
**Task:** Show how to export invoices to QuickBooks or Sage using Invoice Process Backlog. Explain process and best practices.
**Length:** ~850 words  
**Previous:** Creating Invoices  
**Next:** Next Steps

---

# Episode 13 – Next Steps
**Series:** Job Book How to Use  
**Target Roles:** All staff
**Task:** Summarize what’s been covered (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices). Reinforce user confidence. Point to Reporting Guide Series and advanced modules (Tasks, Leave, Assets, Safety).
**Length:** ~850 words  
**Previous:** Importing Invoices  
**Next:** Job Book Advanced Reporting Series

---

## End of Specification
