# Job Book Script Specification

## Purpose
Enable a Large Language Model (LLM) to reliably generate, role-specific YouTube scripts that teach staff how to use Job Book features. Scripts should be clear, structured, and ready for recording as talking head videos with screen demonstrations.

---

## Audience
Job Book users with different roles:
- **Administrator**: Manages clients, jobs, invoices, reports, approvals.
- **Project Manager**: Creates jobs, assigns tasks, tracks progress, manages staff.
- **Technician**: Completes Daily Work Records (DWRs), submits expenses, uses scheduling tools.
- **Owner / Manager**: Monitors dashboards, reviews reports, approves expenses/invoices.

Each script must explicitly state which role it is for.

---

## Script Structure (Mandatory)

1. **Title**  
   - Short, YouTube-friendly, feature-specific. Example: *"How to Create a Job in Job Book"*.

2. **Introduction**  
   - 1–2 sentences. State purpose and benefit of learning this feature.
   - Example: *"In this video, you’ll learn how to create a new job so your team can start tracking work and costs immediately."*

3. **Step-by-Step Demo**  
   - Numbered steps with imperative instructions. Example: *"1. From the Dashboard, click Jobs. 2. Select Add Job."*
   - Avoid UI details that may change (colors, icons, layouts). Focus on labels, menus, and buttons.

4. **Conclusion / Next Step**  
   - Reinforce outcome: *"That’s how you create a job in Job Book."*
   - Suggest logical next video: *"Next, we’ll show you how to add job locations."*
   - Optional: link to help documentation (getjobbook.com/help).

5. **Timing**  
   - Scripts should be short enough to read aloud in 1–2 minutes (<250 words).

---

## Tone and Style
- Clear, concise, professional.
- No filler language (e.g., "Hey guys").
- Use imperative verbs: *"Click," "Select," "Enter."*
- Focus on utility: always state the benefit of the action.

---

## Script Topics
Scripts should cover one feature or workflow at a time. Derived from Job Book collections:

- **Clients**: Adding a client, editing client info.
- **Jobs**: Creating a job, assigning a Project Manager, using the Active Jobs Dashboard.
- **Tasks & Scheduling**: Adding a task, viewing tasks, calendar view.
- **Daily Work Records (DWRs)**: Completing a DWR, adding cost items.
- **Invoices**: Generating an invoice, processing invoices.
- **Rate Sheets**: Applying rate sheets to jobs, setting defaults by client.
- **Workflows**: Approving DWRs, processing invoice backlog.
- **Reports**: Time Card, Utilization, Expense, WIP reports.
- **Expenses**: Submitting and approving expenses.
- **Leave Requests**: Submitting a request, reviewing requests (managers).
- **Assets**: Adding an asset, assigning to jobs.
- **Safety**: Submitting an incident report, accessing policy documentation.
- **Job Maps**: Viewing jobs by location, filtering the map.

---

## Constraints
- <250 words per script.
- Each script must be self-contained (no prior video assumed).
- Use consistent script structure.
- Each script targets one role and one feature.
- Mention add-on modules only if relevant: *“This feature is available only if your company has the Safety module enabled.”*

---

## Success Criteria
A script is acceptable if:
- It can be read aloud in under 2 minutes.
- It clearly identifies the role and feature.
- It includes Title, Intro, Steps, Conclusion.
- It avoids redundant or irrelevant details.
- It suggests the next logical learning step.

---

## Example Input/Output

**Input for LLM:**  
Role: Project Manager  
Feature: Creating a Job  
Length: ~90 seconds

**Expected Output:**  
- *Title*: How to Create a Job in Job Book  
- *Intro*: In this video, you’ll learn how to create a new job so your team can track work and costs.  
- *Steps*: 1. From the Dashboard, click Jobs. 2. Click Add Job. 3. Enter the client name, project name, and job number…  
- *Conclusion*: That’s how you create a job in Job Book. In the next video, we’ll cover how to add job locations.  

---

This specification ensures the LLM can consistently generate useful, ready-to-record Job Book scripts.

