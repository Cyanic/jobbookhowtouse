# Job Book Script Series Specification

## Purpose
Provide a framework for generating a complete **Job Book How to Use Series** of 13 YouTube training videos. Scripts must follow the established narration style from the completed scripts and maintain continuity across the series.

---

## Audience
Job Book staff:
- **Technicians**: Completes Daily Work Records (DWRs), submits expenses.
- **Project Managers**: Tracks progress, Monitors dashboards, DWR approvals.
- **Administrators / Job Coordinators**: Manages clients, jobs, invoices, reports, approvals.
- **Owners / Managers**: approvals, reporting, oversight.

---

## Script Style
- Spoken narration style (natural, step-by-step).
- Reference the **Job Book How to Use Series** if needed.
- Use context-building transitions between episodes.
- Include best practices and role callouts (e.g., *“I’m logged in as an Administrator”*).
- Use on-screen action cues (*“-- Click Save --”*).
- Length: 500–1000 words per script (3–6 minutes when read aloud).
- End each video with a forward link to the next topic.

---

## Video Order / Playlist (13 Episodes)

1. **Intro**  
   - Purpose of the series, prerequisites (Setup Series), overview of daily workflows.

2. **Dashboard**  
   - Technician view: Tasks, DWRs, Expenses, Personal Reports.  
   - Administrator view: Full set of Cards (Clients, Jobs, Reports, Workflow, etc.).

3. **Creating Clients**  
   - Creating a client, required vs. optional fields, contacts, addresses, editing, best practices (deactivation vs. deletion).

4. **Creating Jobs**  
   - Creating a job: job number, client, locations, contacts, project manager, billing types, rate sheets, line items.  
   - Best practices: deactivate vs. delete, cloning jobs.

5. **Creating Daily Work Records (DWRs)**  
   - Technician workflow: entering labour, equipment, materials.  
   - Editing and saving DWRs.

6. **Creating Expenses**  
   - Technician workflow: submitting expenses for reimbursement.  
   - Linking to jobs, best practices.

7. **Active Job Dashboard**  
   - Viewing active jobs, monitoring status, PO amounts, due dates.  
   - Filtering and managing jobs.

8. **DWR Approval Backlog**  
   - Manager/Administrator workflow: approving submitted DWRs.  
   - Best practices for timely approvals.

9. **Expense Approval Backlog**  
   - Manager workflow: reviewing and approving expenses.  
   - Avoiding errors and ensuring accuracy.

10. **DWR Invoice Backlog**  
   - Converting DWRs for Time & Materials jobs into invoices.  
   - Workflow for managers and administrators.

11. **Creating Invoices**  
   - Administrator workflow: invoice types (Ticket/Invoice vs. Invoice).  
   - Line item type (Detailed vs. Summarized).  
   - Editing invoices.

12. **Importing Invoices**  
   - Exporting invoices to accounting systems (QuickBooks, Sage).  
   - Using Invoice Process Backlog.

13. **Next Steps**  
   - Series recap.  
   - Reinforce confidence in daily workflows.  
   - Point to Reporting Guide Series and advanced modules (Tasks, Leave, Assets, Safety).

---

## Constraints
- Scripts must:
  - Start with series continuity statement.
  - Identify relevant role(s).
  - Walk through steps with natural narration.
  - Include explanations and best practices.
  - End with transition to the next video.
- Avoid: filler phrases, UI details that may change (colors/icons).

---

## Success Criteria
A generated script is valid if:
- It matches the established style of the Intro, Dashboard, Clients, and Jobs scripts.
- It runs 400–1200 words in length.
- It blends walkthroughs with role-based best practices.
- It flows logically into the next video.

---

## Example Prompts for LLM

---

## 1. Intro
**Prompt:**  
Role: All staff  
Feature: Series Introduction  
Series Context: First video  
Task: Introduce the Job Book How to Use Series, prerequisites (Setup Series), outline daily workflows (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices), explain short focused episodes, and point to Reporting Guide for advanced features.

---

## 2. Dashboard
**Prompt:**  
Role: Technician and Administrator  
Feature: Navigating the Dashboard  
Series Context: After Intro  
Task: Show Technician dashboard (My Tasks, DWRs, Expenses, Personal Reports) and Administrator dashboard (Clients, Jobs, Workflow, Reports, Rate Sheets, Leave, Assets, Safety, Job Maps). Include role restrictions and best practices.

---

## 3. Creating Clients
**Prompt:**  
Role: Administrator / Job Coordinator  
Feature: Creating and Managing Clients  
Series Context: After Dashboard  
Task: Show creating a client (required fields, optional fields, contacts, addresses, attachments), editing clients, deactivation vs. deletion. Emphasize best practices and prerequisites.

---

## 4. Creating Jobs
**Prompt:**  
Role: Administrator / Job Coordinator  
Feature: Creating and Managing Jobs  
Series Context: After Creating Clients  
Task: Walk through creating a job: job number, client, locations, contacts, project manager, billing type, invoice type, rate sheets, line items, budget quantities. Show editing, cloning, and deactivation best practice.

---

## 5. Creating Daily Work Records (DWRs)
**Prompt:**  
Role: Technician  
Feature: Creating DWRs  
Series Context: After Creating Jobs  
Task: Demonstrate creating a DWR: adding labour, equipment, materials, saving, and editing. Explain why DWRs are essential and tie them back to jobs.

**Output Style (Excerpt):**  
> *Welcome back to the Job Book How to Use Series. In the last video, I showed you how to create jobs in Job Book. In this video, I’ll show you how to create Daily Work Records, or DWRs.*  
> *DWRs are how technicians record their time, equipment, and materials in the system. Every DWR must be tied to a job.*  
> *From the dashboard, click the Create New button inside the Daily Work Records card…*  
> *That’s everything you need to know to create a DWR. In the next video, we’ll cover how to create expenses.*

---

## 6. Creating Expenses
**Prompt:**  
Role: Technician  
Feature: Creating and Submitting Expenses  
Series Context: After Creating DWRs  
Task: Show how to create and submit an expense, attach it to a job, and explain reimbursement workflow. Emphasize accuracy and best practices.

---

## 7. Active Job Dashboard
**Prompt:**  
Role: Project Manager  
Feature: Monitoring Jobs  
Series Context: After Creating Expenses  
Task: Show how to view the Active Job Dashboard, monitor job status, PO amounts, due dates, and use filters. Explain how managers use it for real-time oversight.

---

## 8. DWR Approval Backlog
**Prompt:**  
Role: Manager / Administrator  
Feature: Approving DWRs  
Series Context: After Active Job Dashboard  
Task: Show how to use the DWR Approval Backlog to review and approve submitted DWRs. Explain best practices for timely approvals and workflow impact.

---

## 9. Expense Approval Backlog
**Prompt:**  
Role: Manager  
Feature: Approving Expenses  
Series Context: After DWR Approval Backlog  
Task: Show how to review and approve expenses, identify errors, and manage the Expense Approval Backlog. Emphasize best practices.

---

## 10. DWR Invoice Backlog
**Prompt:**  
Role: Administrator / Manager  
Feature: Converting DWRs into Invoices  
Series Context: After Expense Approval Backlog  
Task: Show how to convert approved DWRs for T&M jobs into invoices. Explain workflow, options, and best practices.

---

## 11. Creating Invoices
**Prompt:**  
Role: Administrator  
Feature: Creating Invoices  
Series Context: After DWR Invoice Backlog  
Task: Show how to create invoices manually or from jobs. Explain invoice type (Ticket/Invoice vs. Invoice), line item type (Detailed vs. Summarized), and editing.

---

## 12. Importing Invoices
**Prompt:**  
Role: Administrator  
Feature: Importing Invoices into Accounting Systems  
Series Context: After Creating Invoices  
Task: Show how to export invoices to QuickBooks or Sage using Invoice Process Backlog. Explain process and best practices.

---

## 13. Next Steps
**Prompt:**  
Role: All staff  
Feature: Series Recap and Next Steps  
Series Context: Final video  
Task: Summarize what’s been covered (Clients, Jobs, DWRs, Expenses, Dashboard, Approvals, Invoices). Reinforce user confidence. Point to Reporting Guide Series and advanced modules (Tasks, Leave, Assets, Safety).

---
