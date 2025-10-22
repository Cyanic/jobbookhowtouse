This file is a merged representation of the entire codebase, combined into a single document by Repomix.
The content has been processed where security check has been disabled.

# File Summary

## Purpose
This file contains a packed representation of the entire repository's contents.
It is designed to be easily consumable by AI systems for analysis, code review,
or other automated processes.

## File Format
The content is organized as follows:
1. This summary section
2. Repository information
3. Directory structure
4. Repository files (if enabled)
5. Multiple file entries, each consisting of:
  a. A header with the file path (## File: path/to/file)
  b. The full contents of the file in a code block

## Usage Guidelines
- This file should be treated as read-only. Any changes should be made to the
  original repository files, not this packed version.
- When processing this file, use the file path to distinguish
  between different files in the repository.
- Be aware that this file may contain sensitive information. Handle it with
  the same level of security as you would the original repository.

## Notes
- Some files may have been excluded based on .gitignore rules and Repomix's configuration
- Binary files are not included in this packed representation. Please refer to the Repository Structure section for a complete list of file paths, including binary files
- Files matching patterns in .gitignore are excluded
- Files matching default ignore patterns are excluded
- Security check has been disabled - content may contain sensitive information
- Files are sorted by Git change count (files with more changes are at the bottom)

# Directory Structure
```
Active_Job_Dashboard.mdx/
  Active_Job_Dashboard.mdx
Administration_Settings.mdx/
  Administration_Settings.mdx
Clients.mdx/
  Clients.mdx
company-calendar.mdx/
  company-calendar.mdx
DWR_Approval.mdx/
  DWR_Approval.mdx
DWR_Entry.mdx/
  DWR_Entry.mdx
Expense_Approval.mdx/
  Expense_Approval.mdx
Expense_Entry.mdx/
  Expense_Entry.mdx
index.mdx/
  index.mdx
Invoicing_a_Fixed_Price_Job.mdx/
  Invoicing_a_Fixed_Price_Job.mdx
Invoicing_a_Time_and_Materials_Job.mdx/
  Invoicing_a_Time_and_Materials_Job.mdx
Job_Client_Attributes.mdx/
  Job_Client_Attributes.mdx
Job_Maps.mdx/
  Job_Maps.mdx
Job_Setup.mdx/
  Job_Setup.mdx
leave-request-initial-setup.mdx/
  leave-request-initial-setup.mdx
leave-request-report.mdx/
  leave-request-report.mdx
leave-request.mdx/
  leave-request.mdx
leave-tracking-overview.mdx/
  leave-tracking-overview.mdx
Overview.mdx/
  Overview.mdx
Personal_Reports.mdx/
  Personal_Reports.mdx
personal-task-management.mdx/
  personal-task-management.mdx
Rate_Sheets.mdx/
  Rate_Sheets.mdx
Reports.mdx/
  Reports.mdx
Site_Staff_DWR_Entry.mdx/
  Site_Staff_DWR_Entry.mdx
Site_Staff_Expense_Entry.mdx/
  Site_Staff_Expense_Entry.mdx
Site_Staff_Initial_Setup.mdx/
  Site_Staff_Initial_Setup.mdx
Site_Staff_Personal_Reports.mdx/
  Site_Staff_Personal_Reports.mdx
task-dashboard.mdx/
  task-dashboard.mdx
task-plans.mdx/
  task-plans.mdx
task-scheduling.mdx/
  task-scheduling.mdx
task-templates.mdx/
  task-templates.mdx
tasks-and-scheduling-overview.mdx/
  tasks-and-scheduling-overview.mdx
Users_and_Employee_Profiles.mdx/
  Users_and_Employee_Profiles.mdx
```

# Files

## File: Active_Job_Dashboard.mdx/Active_Job_Dashboard.mdx
```
---
title: 'Active Job Dashboard'
description: 'Explore the Active Job Dashboard for a comprehensive overview of active jobs, including financial metrics, status updates, and detailed invoice insights, tailored for administrators and managers.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Active_job_dashboard_1.jpg';
import img2 from '~/assets/images/help/Active_job_dashboard_2.jpg';
import img3 from '~/assets/images/help/Active_job_dashboard_3.jpg';

Administrators and Managers can see a bird's-eye view of the active jobs using the Active Job Dashboard. 

<Screenshot image={img1} alt="Active Job Dashboard - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

In the Active Job Dashboard, the current PO$, DWR$, Expense$, Invoice$ and Status are displayed.

<Screenshot image={img2} alt="Active Job Dashboard - Reporting" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users can click the blue arrow to the left of each row to review the Invoice details of each Job.

In the Actions column of each job, you can launch 3 actions for the job:

#### Job Charge-Out Rate Report

#### Summary Report

#### Create Invoice
Commonly used to create an invoice for a fixed-price job (see [Invoicing a Fixed Price Job](/help/Invoicing_a_Fixed_Price_Job)).

<Screenshot image={img3} alt="Active Job Dashboard - DWR and Invoice Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Administration_Settings.mdx/Administration_Settings.mdx
```
---
title: 'Administration Settings'
description: 'Discover how to manage your Administration Settings in Job Book, covering Offices, Labour Cost Items, Equipment, Fixed Price Items, and Expense Items for optimal setup.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Admin_1.webp';
import img2 from '~/assets/images/help/Admin_office.webp';
import img3 from '~/assets/images/help/Admin_labour_item_1.jpg';
import img4 from '~/assets/images/help/Admin_labour_item_2.jpg';
import img5 from '~/assets/images/help/Admin_equipment_item_1.jpg';
import img6 from '~/assets/images/help/Admin_equipment_item_2.jpg';
import img7 from '~/assets/images/help/Admin_fixed_price_item_1.jpg';
import img8 from '~/assets/images/help/Admin_fixed_price_item_2.jpg';
import img9 from '~/assets/images/help/Admin_expense_item_1.jpg';
import img10 from '~/assets/images/help/Admin_expense_item_2.jpg';

<TableOfContents>
    <ol>
        <li>
            <a href="#introduction">Introduction</a>
        </li>
        <li>
            <a href="#offices">Offices</a>
        </li>
        <li>
            <a href="#line-items">Line Items</a>
            <ol>
                <li><a href="#labour-cost-items">Labour Cost Items</a></li>
                <li><a href="#equipment-and-materials">Equipment and Materials</a></li>
                <li><a href="#fixed-price-items">Fixed Price Items</a></li>
            </ol>
        </li>
        <li>
            <a href="#expense-items">Expense Items</a>
        </li>
    </ol>
</TableOfContents>

## Introduction

Job Book requires some configuration as part of the initial setup. This includes **Offices**, **Labour Cost Items**, **Equipment and Materials**, **Fixed Price Items** and **Expense Items**. The Administration toolbar is under the Navigate button that is visible on every page. 

<Screenshot image={img1} alt="Administration Settings - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Offices

Setting up an office in Cyanic Job Book serves several important purposes, especially for businesses with multiple locations or those managing various projects across different regions. Here are some of the key reasons:

1. **Organizational Structure**: Having defined offices within the system helps in organizing and segregating operations, staff, and resources according to location. This can simplify management and improve operational efficiency.
2. **Job Management**: In regards to job assignments and project management, specifying an office for each job helps in tracking and managing the job based on its geographical location. It enables local teams to oversee projects effectively and ensure that resources are allocated properly.
3. **Customized Reporting**: Offices serve as a basis for generating targeted reports. By setting up separate offices, a company can produce localized reports that provide insights into the performance, productivity, and financials of each specific office. This aids in making informed business decisions.
4. **Invoicing and Billing**: Setting up offices in the system allows the correct office address to be shown on invoices, which is crucial for transparency and legal compliance.

### Setting Up an Office
1. **Navigate to Office Settings**:
* Click on the **Navigate** button located at the top left corner of the dashboard.
* Locate the **Administration** panel in the menu.
* Click **Offices** to proceed to office management.
2. **Create a New Office**:
* Click the **Create** button to start setting up a new office.
* **Name**: Enter a name for your office. This could be 'Head Office' or the name of the town where the office is located. This name is used internally and will not be visible to customers.
* **Address**: Below the name field, you will find a multi-line text field for the address. Enter the office address here.
<Screenshot image={img2} alt="Administration Settings - Create Office" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
3. **Save Your Office Setup**:
* After entering the office details, click **Save** to add the office to your system.

## Line Items

Labour Cost Items, Equipment and Materials and Fixed Price Items are ways to capture costs and bill customers for work done on a job. They are the building blocks for making Rate Sheets and when added to a job, users can enter hours or quantities against those line items in their DWRs or Invoices.

Start by entering the various cost items that are commonly used in your organization. The rates you enter here will be used as defaults but can be customized from Rate Sheet to Rate Sheet, or from Job to Job.

### Labour Cost Items

1. Click **Navigate**, expand the **Administration** group, then click **Labour Cost Items**.
<Screenshot image={img3} alt="Administration Settings - Labour Cost Items View" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
2. Create a new Labour Cost Item

    #### Name
    the name of the new labour cost item

    #### GL Code
    General Ledger Code is a unique shorthand code or number given to each account in the Chart of Accounts within your accounting system.

    #### Category
    A category to help organize the cost item (ex., Field Fees, Professional Fees, etc).

    #### Billing Unit
    The 'unit of measure' that is used for billing. HR (Hours) is the default option.

    #### Billing Unit Cost
    The rate (per unit) for this cost item.

    #### Hourly Cost
    Employees enter their time sheets in hours. When the Billing Unit is HR, the Billing Unit Cost and the Hourly Cost will be the same. If the Billing Unit is not HR, the Hourly Cost and Billing Unit Cost are used to convert hours to the unit used for billing.

    #### Tax Exempt
    If the labour cost item is free from tax at the federal, state, or local level.

    #### Active
    If Active is checked, this cost item can be selected when setting up Rate Sheets or Jobs.
<Screenshot image={img4} alt="Administration Settings - Labour Cost Items Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Equipment and Materials

1. Click **Navigate**, expand the **Administration** group and click **Equipment and Materials**.
<Screenshot image={img5} alt="Administration Settings - Equipment and Materials View" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

2. Create a new Equipment / Material item

    #### Name
    the name of the equipment or material

    #### GL Code
    General Ledger Code is a unique shorthand code or number given to each account in the Chart of Accounts within your accounting system.

    #### Category
    A category to help organize the cost item.

    #### Unit
    The 'unit of measure' that is used for billing.

    #### Unit Cost
    The rate (per unit) for this cost item.

    #### Tax Exempt
    If the labour cost item is free from tax at the federal, state, or local level.

    #### Active
    If Active is checked, this cost item can be selected when setting up Rate Sheets or Jobs.
<Screenshot image={img6} alt="Administration Settings - Equipment and Materials Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Fixed Price Items

Fixed Price Items represent line items that can be added to Invoices, but are not recorded as work in a DWR.

1. Click **Navigate**, expand the **Administration** group and click **Fixed Price Item**.
<Screenshot image={img7} alt="Administration Settings - Fixed Price Items View" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

2. Create a new Fixed Price item

    #### Name
    the name of the fixed price item

    #### GL Code
    General Ledger Code is a unique shorthand code or number given to each account in the Chart of Accounts within your accounting system.

    #### Category
    A category to help organize the cost item.

    #### Unit
    The 'unit of measure' that is used for billing.

    #### Unit Cost
    The rate (per unit) for this cost item.

    #### Tax Exempt
    If the labour cost item is free from tax at the federal, state, or local level.

    #### Active
    If Active is checked, this cost item can be selected when setting up Rate Sheets or Jobs.
<Screenshot image={img8} alt="Administration Settings - Fixed Price Items Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Expense Items

In Job Book, Users can submit expenses for reimbursement, using the Expense Items you configured.

1. Click **Navigate**, expand the **Administration** group and click **Expense Items**.
<Screenshot image={img9} alt="Administration Settings - Expense Items View" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
2. Create a new expense item and input the item's name.
<Screenshot image={img10} alt="Administration Settings - Expense Items Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Clients.mdx/Clients.mdx
```
---
title: 'Clients'
description: 'Learn how to add a client to Job Book, including setting company name, website, client types, rate sheet, contacts, and locations for efficient job management.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Client_1.jpg';
import img2 from '~/assets/images/help/Client_2.jpg';
import img3 from '~/assets/images/help/Client_3.jpg';

To add a Client to Job Book, click Create New on the Client card on the dashboard. 

<Screenshot image={img1} alt="Clients - Create New" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Company Name
The name of the client that can be selected in a Job.

#### Website
The URL of the client's website (if any).

#### Client Type(s)
One or more 'client type' that can be searched later in [Job Maps](/help/Job_Maps).

#### Rate Sheet
The default [Rate Sheet](/help/Rate_Sheets) that is used for new Jobs for this client.

<Screenshot image={img2} alt="Clients - Company Tab" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Contacts
Client contacts that can be added to Jobs for this client.

<Screenshot image={img3} alt="Clients - Contact and Location Tab" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Locations
Office locations for this client that can be selected for a Job for billing.

#### Active
if checked, this client can be selected when creating a new job.
```

## File: company-calendar.mdx/company-calendar.mdx
```
---
title: 'Company Calendar'
description: 'The Company Calendar provides a comprehensive overview of all employee leave requests, holidays, and other important company-wide events.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import companyCalendarNav from '~/assets/images/help/company-calendar/company-calendar-nav.png';
import companyCalendar from '~/assets/images/help/company-calendar/company-calendar.png';
import companyCalendarMonth from '~/assets/images/help/company-calendar/company-calendar-month.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#key-concepts">Key Concepts</a>
        </li>
        <li>
            <a href="#navigating-to-the-company-calendar">Navigating to the Company Calendar</a>
        </li>
        <li>
            <a href="#understanding-the-layout">Understanding the Layout</a>
            <ol>
                <li><a href="#week-view">Week View</a></li>
                <li><a href="#month-view">Month View</a></li>
            </ol>
        </li>
        <li>
            <a href="#filtering-the-calendar">Filtering the Calendar</a>
        </li>
    </ol>
</TableOfContents>

## Key Concepts

The Company Calendar is a centralized tool designed to give managers and administrators a clear view of employee availability. It consolidates all approved leave requests into a single, easy-to-read calendar.

This helps in planning and scheduling by preventing conflicts and ensuring that you always have a real-time overview of your team's availability.

### Navigating to the Company Calendar

To navigate to the Company Calendar, click 'Company Calendar' in the 'Leave Requests' card on the dashboard.

<Screenshot image={companyCalendarNav} alt="Navigating to the Company Calendar" caption="Navigating to the Company Calendar" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Understanding the Layout

The Company Calendar provides both a week and a month view of employee leave.

#### Week View

The default view is the week view, which shows a detailed breakdown of leave for the current week. Each employee with approved leave is listed, and their time off is displayed as a block on the corresponding day. No information about the specifics of the leave requests are displayed, it only shows that time is blocked off for any given employee.

If you are an Administrator or Manager, you can navigate to a Leave Request by clicking on the event in the calendar.

<Screenshot image={companyCalendar} alt="Company Calendar Week View" caption="The Company Calendar (Week View)" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

You can navigate the calendar using the following controls:

*   **Forward/Backward**: Use the **&lt;** and **&gt;** buttons to move one week at a time.
*   **Go to Today**: Click the **Today** button to jump back to the current date.
*   **Change View**: Switch to the **Month** view by clicking the corresponding button.

#### Month View

The month view gives you a broader overview of employee leave for the entire month. Each day with an approved leave request is marked on the calendar.

<Screenshot image={companyCalendarMonth} alt="Company Calendar Month View" caption="The Company Calendar (Month View)" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

You can navigate the calendar using the following controls:

*   **Forward/Backward**: Use the **&lt;** and **&gt;** buttons to move one month at a time.
*   **Go to Today**: Click the **Today** button to jump back to the current date.
*   **Change View**: Switch back to the **Week** view by clicking the corresponding button.

### Filtering the Calendar

To help you focus on specific team members, both the week and month views can be filtered by clicking the 'Employee Filter' multi-select field. This allows you to narrow down the calendar view in several ways:

*   **By Employee**: Select one or more individual employees to see only their leave schedules.
*   **By Office**: Offices are listed at the top of the filter and are identified by an 'office' icon. Selecting an office will show leave for all employees assigned to that location.
*   **By Employee Group**: Below the offices, you can select predefined Employee Groups, which are marked with a 'group' icon. This is useful for viewing the combined schedule for a specific crew or team.

<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/leave-tracking-overview">Leave Tracking: Overview</a></li>
        <li><a href="/help/leave-request-initial-setup">Leave Request Initial Setup</a></li>
        <li><a href="/help/leave-request">Leave Requests</a></li>
        <li><a href="/help/leave-request-report">Leave Request Report</a></li>
        <li>Company Calendar</li>
    </ol>
</TableOfContents>
```

## File: DWR_Approval.mdx/DWR_Approval.mdx
```
---
title: 'DWR Approval'
description: 'Learn how to approve DWRs effectively with our guide. Navigate your dashboard, select multiple DWRs for approval, and utilize filters to streamline the process.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Dwr_approval_1.jpg';
import img2 from '~/assets/images/help/Dwr_approval_2.jpg';
import img3 from '~/assets/images/help/Dwr_approval_3.jpg';
import img4 from '~/assets/images/help/Dwr_approval_4.jpg';

<Screenshot image={img1} alt="DWR Approval - Flow" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click **DWR Approval Backlog** in the Workflow card on the dashboard.

Submitted DWRs will show in the DWR Approval Backlog. Project Managers can select any number of DWRs and click the **Approve Selected DWRs** button. 

<Screenshot image={img2} alt="DWR Approval - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img3} alt="DWR Approval - Selecting DWRs" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Next to each DWR is a blue arrow. Clicking this arrow will show details of the DWR to help with the review.

DWRs can be filtered by Project Manager, Client, Office, and Job Number. 

<Screenshot image={img4} alt="DWR Approval - Filtering and Expanding DWR Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: DWR_Entry.mdx/DWR_Entry.mdx
```
---
title: 'DWR Entry'
description: 'Explore the guide to entering Daily Work Records (DWR) in Job Book, covering step-by-step instructions, from job selection to signatures and obtaining approvals.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Dwr_entry_1.jpg';
import img2 from '~/assets/images/help/Dwr_entry_2.jpg';
import img3 from '~/assets/images/help/Dwr_entry_3.jpg';
import img4 from '~/assets/images/help/Dwr_entry_4.jpg';
import img5 from '~/assets/images/help/Dwr_entry_5.jpg';
import img6 from '~/assets/images/help/Dwr_entry_6.jpg';
import img7 from '~/assets/images/help/Dwr_entry_7.jpg';

Daily Work Records are the timesheets for users to record employees' daily office/site work (working hours, equipment/materials usage) in Job Book. Project Managers will review and approve the submitted DWRs. The flow of DWRs is illustrated as follows:

<Screenshot image={img1} alt="DWR Entry - Flow" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click the "Create New" icon in the "Daily Work Records" card on the dashboard.

<Screenshot image={img2} alt="DWR Entry - Create New" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users must first enter the date and select a job, after which they can fill out the rest of the DWR.

<Screenshot image={img3} alt="DWR Entry - Job Selection" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users will then add labour costs and equipment/materials.

#### Labour Cost
Information on cost items, employees, time cards, and descriptions are available in this section.

#### Equipment and Material
Information on cost items (incidentals, equipment, and material), names, units, and quantities are available in this section.

<Screenshot image={img4} alt="DWR Entry - Entering Labour Costs" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img5} alt="DWR Entry - Entering Equipment and Materials" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img6} alt="DWR Entry - Viewing Job Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

After filling in the DWR details, users can add a representative signature for the DWR, and collect the client's signature if needed. 

<Screenshot image={img7} alt="DWR Entry - Collecting Representative and Client Signatures" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

When finished, users will check the Submitted checkbox and save the DWR. The DWR will then be available to the Project Manager for approval.
```

## File: Expense_Approval.mdx/Expense_Approval.mdx
```
---
title: 'Expense Approval'
description: 'Streamline expense approvals in your land surveying projects with Job Book''s easy-to-use platform, ensuring efficient workflow and financial control.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Expense_approval_1.jpg';
import img2 from '~/assets/images/help/Expense_approval_2.jpg';

In Job Book, Managers and Administrators can easily review and approve submitted expenses.

Click **Expense Approval Backlog** in the Workflow card on the dashboard. 

<Screenshot image={img1} alt="Expense Approval Backlog - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Select one or more expenses and click the **Approve Selected Expenses** button.

<Screenshot image={img1} alt="Expense Approval Backlog - Approving Selected Expenses" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Expense_Entry.mdx/Expense_Entry.mdx
```
---
title: 'Expense Entry'
description: 'Learn how to create and submit expense entries for reimbursement using our step-by-step guide, including adding details, attachments, and final submission.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Expense_1.jpg';
import img2 from '~/assets/images/help/Expense_2.jpg';
import img3 from '~/assets/images/help/Expense_3.jpg';

Employees can create expenses for reimbursement.

Click **Create New** in **Expenses** on the dashboard. 

<Screenshot image={img1} alt="Expenses - Create New" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Enter the date, employee name, job, expense items, and the total amount.

Users can add attachments (ex., receipt photos) and descriptions here.

Check the **Submitted** checkbox and save the expense. 

<Screenshot image={img2} alt="Expenses - Expense Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img3} alt="Expenses - Submitting" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: index.mdx/index.mdx
```
---
title: 'Index'
layout: '~/layouts/HelpLayout.astro'
---

## Administration Guide

<ol>
    <li>
        <h3><a href="/help/Overview">Overview</a></h3>
        <ol>
            <li>
                <a href="/help/Overview#what-is-job-book">What is Job Book</a>
            </li>
            <li>
                <a href="/help/Overview#how-will-job-book-improve-my-life">How will Job Book improve my life?</a>
                <ol>
                    <li><a href="/help/Overview#administrators">Administrators</a></li>
                    <li><a href="/help/Overview#management">Management</a></li>
                    <li><a href="/help/Overview#technicians">Technicians</a></li>
                </ol>
            </li>
            <li>
                <a href="/help/Overview#how-will-job-book-improve-my-company">How will Job Book improve my company?</a>
                <ol>
                    <li><a href="/help/Overview#improve-profitability">Improve Profitability</a></li>
                    <li><a href="/help/Overview#improve-accountability">Improve Accountability</a></li>
                    <li><a href="/help/Overview#improve-sustainability">Improve Sustainability</a></li>
                </ol>
            </li>
            <li>
                <a href="/help/Overview#now-is-the-time">Now is the Time</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Users_and_Employee_Profiles">Users and Employee Profiles</a></h3>
        <ol>
            <li>
                <a href="/help/Users_and_Employee_Profiles#users">Users</a>
            </li>
            <li>
                <a href="/help/Users_and_Employee_Profiles#user-roles">User Roles</a>
                <ol>
                    <li><a href="/help/Users_and_Employee_Profiles#technician">Technician</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#job-coordinator">Job Coordinator</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#manager">Manager</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#administrator">Administrator</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#view">View</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#modify--create--delete">Modify / Create / Delete</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#report-access">Report Access</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#tasks--scheduling-if-scheduling-module-enabled">Tasks / Scheduling</a></li>
                    <li><a href="/help/Users_and_Employee_Profiles#leave-requests-if-module-enabled">Leave Requests</a></li>
                </ol>
            </li>
            <li>
                <a href="/help/Users_and_Employee_Profiles#adding-users-and-setting-roles">Adding Users and Setting Roles</a>
            </li>
            <li>
                <a href="/help/Users_and_Employee_Profiles#new-user-login">New User Login</a>
            </li>
            <li>
                <a href="/help/Users_and_Employee_Profiles#employees">Employees</a>
            </li>
            <li>
                <a href="/help/Users_and_Employee_Profiles#employees">Adding Employees</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Administration_Settings">Administration Settings</a></h3>
        <ol>
            <li>
                <a href="/help/Administration_Settings#introduction">Introduction</a>
            </li>
            <li>
                <a href="/help/Administration_Settings#offices">Offices</a>
            </li>
            <li>
                <a href="/help/Administration_Settings#line-items">Line Items</a>
                <ol>
                    <li><a href="/help/Administration_Settings#labour-cost-items">Labour Cost Items</a></li>
                    <li><a href="/help/Administration_Settings#equipment-and-materials">Equipment and Materials</a></li>
                    <li><a href="/help/Administration_Settings#fixed-price-items">Fixed Price Items</a></li>
                </ol>
            </li>
            <li>
                <a href="/help/Administration_Settings#expense-items">Expense Items</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Rate_Sheets">Rate Sheets</a></h3>
    </li>
    <li>
        <h3><a href="/help/Clients">Clients</a></h3>
    </li>
    <li>
        <h3><a href="/help/Job_Setup">Job Setup</a></h3>
        <ol>
            <li>
                <a href="/help/Job_Setup#basic-configuration">Basic Configuration</a>
            </li>
            <li>
                <a href="/help/Job_Setup#billing-configuration">Billing Configuration</a>
            </li>
            <li>
                <a href="/help/Job_Setup#adding-line-items">Adding Line Items</a>
            </li>
            <li>
                <a href="/help/Job_Setup#archiving-and-removing-line-items">Archiving and Removing Line Items</a>
            </li>
            <li>
                <a href="/help/Job_Setup#activating-and-deactivating-jobs">Activating and Deactivating Jobs</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Job_Client_Attributes">Job and Client Attribute Tags</a></h3>
    </li>
    <li>
        <h3><a href="/help/Active_Job_Dashboard">Active Job Dashboard</a></h3>
    </li>
    <li>
        <h3><a href="/help/DWR_Entry">DWR Entry</a></h3>
    </li>
    <li>
        <h3><a href="/help/DWR_Approval">DWR Approval</a></h3>
    </li>
    <li>
        <h3><a href="/help/Invoicing_a_Time_and_Materials_Job">Invoicing a Time & Materials Job</a></h3>
        <ol>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#overview">Overview</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#invoice-creation">Invoice Creation</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#pm-queue">PM Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#ticket-queue">Ticket Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#admin-queue">Admin Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Time_and_Materials_Job#processed-queue">Processed Queue</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Invoicing_a_Fixed_Price_Job">Invoicing a Fixed Price Job</a></h3>
        <ol>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#overview">Overview</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#invoice-creation">Invoice Creation</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#pm-queue">PM Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#ticket-queue">Ticket Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#admin-queue">Admin Queue</a>
            </li>
            <li>
                <a href="/help/Invoicing_a_Fixed_Price_Job#processed-queue">Processed Queue</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Expense_Entry">Expense Entry</a></h3>
    </li>
    <li>
        <h3><a href="/help/Expense_Approval">Expense Approval</a></h3>
    </li>
    <li>
        <h3><a href="/help/Job_Maps">Job Maps</a></h3>
    </li>
    <li>
        <h3><a href="/help/Personal_Reports">Personal Reports</a></h3>
        <ol>
            <li>
                <a href="/help/Personal_Reports#my-time-cards">My Time Cards</a>
            </li>
            <li>
                <a href="/help/Personal_Reports#my-expenses">My Expenses</a>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/Reports">Reports</a></h3>
        <ol>
            <li>
                <a href="/help/Reports#line-item-report">Line Item Report</a>
            </li>
            <li>
                <a href="/help/Reports#work-in-progress-wip-report">Work in Progress (WIP) Report</a>
            </li>
        </ol>
    </li>
</ol>



## Technician / Site Staff Guide

<ol>
    <li>
        <h3><a href="/help/Site_Staff_Initial_Setup">Technician / Site Staff Initial Setup</a></h3>
    </li>
    <li>
        <h3><a href="/help/Site_Staff_DWR_Entry">DWR Entry</a></h3>
    </li>
    <li>
        <h3><a href="/help/Site_Staff_Expense_Entry">Expense Entry</a></h3>
    </li>
    <li>
        <h3><a href="/help/Site_Staff_Personal_Reports">Personal Reports</a></h3>
    </li>
</ol>

<h2>Task Management and Crew Scheduling</h2>

<ol>
    <li>
        <h3><a href="/help/tasks-and-scheduling-overview">Overview</a></h3>
        <ol>
            <li><a href="/help/tasks-and-scheduling-overview#introduction">Introduction</a></li>
            <li><a href="/help/tasks-and-scheduling-overview#key-concepts">Key Concepts</a></li>
            <li><a href="/help/tasks-and-scheduling-overview#how-it-fits-together">How It All Fits Together</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/task-templates">Task Templates</a></h3>
        <ol>
            <li><a href="/help/task-templates#key-concepts">Key Concepts</a></li>
            <li><a href="/help/task-templates#exploring-task-templates">Exploring Task Templates</a></li>
            <li><a href="/help/task-templates#viewing-a-task-template">Viewing a Task Template</a></li>
            <li><a href="/help/task-templates#editing-a-task-template">Editing a Task Template</a></li>
            <li><a href="/help/task-templates#adding-and-organizing-tasks">Adding and Organizing Tasks</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/task-plans">Task Plans</a></h3>
        <ol>
            <li><a href="/help/task-plans#key-concepts">Key Concepts</a></li>
            <li><a href="/help/task-plans#navigating-to-a-jobs-task-plan">Navigating to a Job's Task Plan</a></li>
            <li><a href="/help/task-plans#importing-task-templates">Importing Task Templates</a></li>
            <li><a href="/help/task-plans#task-status">Task Status</a></li>
            <li><a href="/help/task-plans#task-due-date">Task Due Date</a></li>
            <li><a href="/help/task-plans#assigning-tasks">Assigning Tasks</a></li>
            <li><a href="/help/task-plans#scheduled-tasks">Scheduled Tasks</a></li>
            <li><a href="/help/task-plans#adding-and-organizing-tasks">Adding and Organizing Tasks</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/task-scheduling">Task Scheduling</a></h3>
        <ol>
            <li><a href="/help/task-scheduling#key-concepts">Key Concepts</a></li>
            <li><a href="/help/task-scheduling#navigating-to-the-task-scheduler">Navigating to the Task Scheduler</a></li>
            <li><a href="/help/task-scheduling#understanding-the-layout">Understanding the Layout</a></li>
            <li><a href="/help/task-scheduling#scheduling-a-task">Scheduling a Task</a></li>
            <li><a href="/help/task-scheduling#modifying-a-scheduled-task">Modifying a Scheduled Task</a></li>
            <li><a href="/help/task-scheduling#editing-task-details">Editing Task Details</a></li>
            <li><a href="/help/task-scheduling#filtering-the-calendar-by-employee">Filtering the Calendar by Employee</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/personal-task-management">Personal Task Management</a></h3>
        <ol>
            <li><a href="/help/personal-task-management#overview">Overview</a></li>
            <li>
                <a href="/help/personal-task-management#my-schedule">My Schedule</a>
                <ol>
                    <li><a href="/help/personal-task-management#accessing-my-schedule">Accessing My Schedule</a></li>
                    <li><a href="/help/personal-task-management#viewing-your-schedule">Viewing Your Schedule</a></li>
                    <li><a href="/help/personal-task-management#changing-task-status-in-my-schedule">Changing Task Status</a></li>
                </ol>
            </li>
            <li>
                <a href="/help/personal-task-management#my-unscheduled-tasks">My Unscheduled Tasks</a>
                <ol>
                    <li><a href="/help/personal-task-management#accessing-my-unscheduled-tasks">Accessing My Unscheduled Tasks</a></li>
                    <li><a href="/help/personal-task-management#viewing-your-unscheduled-tasks">Viewing Your Unscheduled Tasks</a></li>
                    <li><a href="/help/personal-task-management#changing-task-status-in-my-unscheduled-tasks">Changing Task Status</a></li>
                </ol>
            </li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/task-dashboard">Task Dashboard</a></h3>
        <ol>
            <li><a href="/help/task-dashboard#overview">Overview</a></li>
            <li><a href="/help/task-dashboard#accessing-the-task-dashboard">Accessing the Task Dashboard</a></li>
            <li>
                <a href="/help/task-dashboard#features">Features</a>
                <ol>
                    <li><a href="/help/task-dashboard#columns">Columns</a></li>
                    <li><a href="/help/task-dashboard#grid-operations">Grid Operations</a></li>
                    <li><a href="/help/task-dashboard#report-templating">Report Templating</a></li>
                </ol>
            </li>
        </ol>
    </li>
</ol>

<h2>Leave Tracking</h2>

<ol>
    <li>
        <h3><a href="/help/leave-tracking-overview">Overview</a></h3>
        <ol>
            <li><a href="/help/leave-tracking-overview#introduction">Introduction</a></li>
            <li><a href="/help/leave-tracking-overview#key-concepts">Key Concepts</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/leave-request-initial-setup">Leave Request Initial Setup</a></h3>
        <ol>
            <li><a href="/help/leave-request-initial-setup#key-concepts">Key Concepts</a></li>
            <li><a href="/help/leave-request-initial-setup#performing-common-tasks">Performing Common Tasks</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/leave-request">Leave Requests</a></h3>
        <ol>
            <li><a href="/help/leave-request#key-concepts">Key Concepts</a></li>
            <li><a href="/help/leave-request#creating-a-leave-request">Creating a Leave Request</a></li>
            <li><a href="/help/leave-request#navigating-existing-leave-requests">Navigating Existing Leave Requests</a></li>
            <li><a href="/help/leave-request#reviewing-a-leave-request">Reviewing a Leave Request</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/leave-request-report">Leave Request Report</a></h3>
        <ol>
            <li><a href="/help/leave-request-report#key-concepts">Key Concepts</a></li>
            <li><a href="/help/leave-request-report#performing-common-tasks">Performing Common Tasks</a></li>
        </ol>
    </li>
    <li>
        <h3><a href="/help/company-calendar">Company Calendar</a></h3>
        <ol>
            <li><a href="/help/company-calendar#key-concepts">Key Concepts</a></li>
            <li><a href="/help/company-calendar#navigating-to-the-company-calendar">Navigating to the Company Calendar</a></li>
            <li><a href="/help/company-calendar#understanding-the-layout">Understanding the Layout</a></li>
            <li><a href="/help/company-calendar#filtering-the-calendar">Filtering the Calendar</a></li>
        </ol>
    </li>
</ol>
```

## File: Invoicing_a_Fixed_Price_Job.mdx/Invoicing_a_Fixed_Price_Job.mdx
```
---
title: 'Invoicing a Fixed Price Job'
description: 'Learn how to create, review, and process invoices for fixed-price jobs with ease, covering steps from invoice creation to payment in Job Book.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Invoice_fp_1.jpg';
import img2 from '~/assets/images/help/Invoice_fp_2.jpg';
import img3 from '~/assets/images/help/Invoice_fp_3.jpg';
import img4 from '~/assets/images/help/Invoice_fp_4.jpg';
import img5 from '~/assets/images/help/Invoice_fp_5.jpg';
import img6 from '~/assets/images/help/Invoice_fp_6.jpg';
import img7 from '~/assets/images/help/Invoice_fp_7.jpg';
import img8 from '~/assets/images/help/Invoice_fp_8.jpg';
import img9 from '~/assets/images/help/Invoice_fp_9.jpg';
import img10 from '~/assets/images/help/Invoice_fp_10.jpg';
import img11 from '~/assets/images/help/Invoice_fp_11.jpg';
import img12 from '~/assets/images/help/Invoice_fp_12.jpg';
import img13 from '~/assets/images/help/Invoice_fp_13.jpg';
import img14 from '~/assets/images/help/Invoice_fp_14.jpg';
import img15 from '~/assets/images/help/Invoice_fp_15.jpg';

<TableOfContents>
    <ol>
        <li>
            <a href="#overview">Overview</a>
        </li>
        <li>
            <a href="#invoice-creation">Invoice Creation</a>
        </li>
        <li>
            <a href="#pm-queue">PM Queue</a>
        </li>
        <li>
            <a href="#admin-queue">Admin Queue</a>
        </li>
        <li>
            <a href="#processed-queue">Processed Queue</a>
        </li>
    </ol>
</TableOfContents>

## Overview

Job Book provides an easy way to create invoices for fixed-price jobs. The invoicing process is illustrated as follows.

<Screenshot image={img1} alt="Invoicing a Fixed Price Job - Flow" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Invoice Creation

Load the [Active Job Dashboard](/help/Active_Job_Dashboard) by clicking **Active Job Dashboard** in the Jobs cards on the dashboard.

<Screenshot image={img2} alt="Invoicing a Fixed Price Job - Active Job Dashboard Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

For the fixed price job, and click the **dollar icon** in the Actions column to create an invoice.

<Screenshot image={img3} alt="Invoicing a Fixed Price Job - Active Job Dashboard Create Invoice" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Edit the invoice details on the invoice creation page. Users can choose to input the invoice details manually (labour cost, equipment & materials, fixed price...) to simply enter a bottom-line total amount. 

<Screenshot image={img4} alt="Invoicing a Fixed Price Job - Invoice Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img5} alt="Invoicing a Fixed Price Job - Invoice Bottom Line Totals" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## PM Queue

After an invoice has been created, a Project Manager will review and sign-off on the invoice. Select **Explore** in the Invoices card on the dashboard. 

<Screenshot image={img6} alt="Invoicing a Fixed Price Job - Invoice PM Queue - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Invoices in the **PM Queue** need a Representative Signature. Click an invoice to review it. 

<Screenshot image={img7} alt="Invoicing a Fixed Price Job - Invoice PM Queue - Invoice Selection" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click **Edit**.

<Screenshot image={img8} alt="Invoicing a Fixed Price Job - Invoice Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Scroll down to the **Representative Signature** field, add a signature, then save the invoice.

<Screenshot image={img9} alt="Invoicing a Fixed Price Job - Collect Representative Signature" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

After signing-off on the invoice, if the invoice type is **Ticket/Invoice**, there is one additional process. The invoices will be sent to the **Ticket Queue** and will require client approval. If the invoice type is **Invoice**, then the invoices will be sent to the **Admin Queue** for administrators to process the invoice as appropriate and check the **Processed** checkbox to complete the invoice. 

## Admin Queue

Invoices in the Admin Queue require an administrator to check the **Processed** checkbox. 

<Screenshot image={img10} alt="Invoicing a Fixed Price Job - Invoice Process Backlog - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users can select the invoice to process. Moreover, if users have accounting needs, they can **export selected invoices**, and use the downloaded file to import to QuickBooks, Sage, Xero or other accounting software. 

<Screenshot image={img11} alt="Invoicing a Fixed Price Job - Invoice Process Backlog - Export to QuickBooks, Sage, Xero" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Processed Queue

The Processed Queue shows invoices that have been processed but not yet paid. After payment, edit the invoice and check the **Paid** checkbox to complete the invoice.

<Screenshot image={img6} alt="Invoicing a Fixed Price Job - Invoice PM Queue - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img12} alt="Invoicing a Fixed Price Job - Processed Queue - Selecting Invoice to Pay" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img13} alt="Invoicing a Fixed Price Job - Invoice Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img14} alt="Invoicing a Fixed Price Job - Invoice Payment" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img15} alt="Invoicing a Fixed Price Job - Paid Queue" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Invoicing_a_Time_and_Materials_Job.mdx/Invoicing_a_Time_and_Materials_Job.mdx
```
---
title: 'Invoicing a Time & Materials Job'
description: 'Learn to efficiently generate invoices for Time & Materials jobs with our step-by-step guide, including detailed workflows and helpful screenshots.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Invoice_tm_1.jpg';
import img2 from '~/assets/images/help/Invoice_tm_2.jpg';
import img3 from '~/assets/images/help/Invoice_tm_3.jpg';
import img4 from '~/assets/images/help/Invoice_tm_4.jpg';
import img5 from '~/assets/images/help/Invoice_tm_5.jpg';
import img6 from '~/assets/images/help/Invoice_tm_6.jpg';
import img7 from '~/assets/images/help/Invoice_tm_7.jpg';
import img8 from '~/assets/images/help/Invoice_tm_8.jpg';
import img9 from '~/assets/images/help/Invoice_tm_9.jpg';
import img10 from '~/assets/images/help/Invoice_tm_10.jpg';
import img11 from '~/assets/images/help/Invoice_tm_11.jpg';
import img12 from '~/assets/images/help/Invoice_tm_12.jpg';
import img13 from '~/assets/images/help/Invoice_tm_13.jpg';
import img14 from '~/assets/images/help/Invoice_tm_14.jpg';
import img15 from '~/assets/images/help/Invoice_tm_15.jpg';

<TableOfContents>
    <ol>
        <li>
            <a href="#overview">Overview</a>
        </li>
        <li>
            <a href="#invoice-creation">Invoice Creation</a>
        </li>
        <li>
            <a href="#pm-queue">PM Queue</a>
        </li>
        <li>
            <a href="#ticket-queue">Ticket Queue</a>
        </li>
        <li>
            <a href="#admin-queue">Admin Queue</a>
        </li>
        <li>
            <a href="#processed-queue">Processed Queue</a>
        </li>
    </ol>
</TableOfContents>

## Overview

Job Book provides a fast and effective way to generate invoices for Time & Material jobs, using the data recorded in DWRs for the job. The invoicing process is illustrated as follows:

<Screenshot image={img1} alt="Invoicing a Time & Materials Job - Flow" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Invoice Creation

Click **DWR Invoice Backlog** in the Workflow card on the dashboard. The DWR Invoice Backlog shows approved DWRs for Time & Materials jobs that have not yet been invoiced.

<Screenshot image={img2} alt="Invoicing a Time & Materials Job - DWR Invoice Backlog - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

DWR details can be reviewed by clicking the blue arrow icon to the left of each DWR.

Select the DWRs to invoice and click the **Invoice Selected DWRs** button. DWRs under one job will be generated into one invoice. 

<Screenshot image={img3} alt="Invoicing a Time & Materials Job - DWR Invoice Backlog - Select DWRs and Generate Invoice" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## PM Queue

After an invoice has been created, a Project Manager will review and sign-off on the invoice. Select **Explore** in the Invoices card on the dashboard. 

<Screenshot image={img4} alt="Invoicing a Time & Materials Job - Invoices - Explore" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Invoices in the **PM Queue** need a Representative Signature. Click an invoice to review it. 

<Screenshot image={img5} alt="Invoicing a Time & Materials Job - Invoices - PM Queue" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click **Edit**.

<Screenshot image={img6} alt="Invoicing a Time & Materials Job - Invoices - Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Scroll down to the **Representative Signature** field, add a signature, then save the invoice.

<Screenshot image={img7} alt="Invoicing a Time & Materials Job - Invoices - Collect Representative Signature" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

After signing-off on the invoice, if the invoice type is **Ticket/Invoice**, there is one additional process. The invoices will be sent to the **Ticket Queue** and will require client approval. If the invoice type is **Invoice**, then the invoices will be sent to the **Admin Queue** for administrators to process the invoice as appropriate and check the **Processed** checkbox to complete the invoice.

## Ticket Queue

Click **Explore** in the Invoices card on the dashboard. Select **Ticket Queue** to view tickets that require customer approval.

To move tickets out of the Ticket Queue and convert them to Invoices, edit the ticket and check the **Client Approved Ticket** checkbox.

<Screenshot image={img8} alt="Invoicing a Time & Materials Job - Invoices - Ticket Queue" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img9} alt="Invoicing a Time & Materials Job - Invoices - Ticket Queue - Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img10} alt="Invoicing a Time & Materials Job - Invoices - Ticket Queue - Client Approved Ticket" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Admin Queue

Invoices in the Admin Queue require an administrator to check the **Processed** checkbox. 

<Screenshot image={img11} alt="Invoicing a Time & Materials Job - Invoices - Invoice Processing Backlog - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img12} alt="Invoicing a Time & Materials Job - Invoices - Invoice Processing Backlog - Select Invoices" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Processed Queue

The Processed Queue shows invoices that have been processed but not yet paid. After payment, edit the invoice and check the **Paid** checkbox to complete the invoice.

<Screenshot image={img13} alt="Invoicing a Time & Materials Job - Invoices - Processed Queue" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img14} alt="Invoicing a Time & Materials Job - Invoices - Processed Queue - Edit" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img15} alt="Invoicing a Time & Materials Job - Invoices - Processed Queue - Paid" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Job_Client_Attributes.mdx/Job_Client_Attributes.mdx
```
---
title: 'Job and Client Attribute Tags'
description: 'Preview the attributes that can be tagged on clients and jobs to help with searching and analytics'
layout: '~/layouts/HelpLayout.astro'
---

Jobs and clients can be tagged with any number of the following attributes to help with [searching](/help/Job_Maps) and analytics.

## Client Types

* Architect
* Commercial Owner
* Consultant
* Construction
* Construction Management
* Developers
* Engineers
* Federal Government
* First Nations/Indigenous Group
* Government
* Land Agents
* Lawyer
* Mining
* Municipal Government
* Oil & Gas
* Pipelines
* Provincial Government
* Realtor
* Residential Owner
* Surveyors
* Utility Company
* Vendor

## Job Categories

* Architectural
* Commercial
* Construction
* Energy
* Engineering
* GIS
* Government
* Industrial
* Infrastructure
* Legal
* Mining
* Municipal
* Oil & Gas
* Pipeline
* Residential

## Job Scopes

* 3D Scanning
* Abandonment
* Access Map
* Access Road
* AGM Mapping
* Air Photo
* Air Space Plan
* Alignment
* ALR/SME Sketch Plan
* ALTA Survey
* Anchor Site
* As-Built Survey
* Bathymetric Survey
* Battery Site
* Benchmark
* Block Face Plan
* Booster
* Boreholes
* Borrow Pit
* Boundary Stake-Out
* Boundary Survey
* Builder Survey Package
* Building Layout
* Cable Right of Way
* CAD Support
* Calculations
* Camp Site
* Canada Lands Survey
* Canal Right of Way
* Cathodic Protection System
* Cement Pit
* Certificate
* Civil Work
* Commercial Building Construction
* Commercial Stakeout
* Compaction Testing
* Compiled Plan
* Compressor Site
* Condominium Plan
* Consolidation Plan
* Construction
* Construction Layout
* Control Network Establishment
* Corrosion Monitor Installation
* Crossing Plan
* Depth of Cover
* Descriptive Plan
* Design
* Development Permit
* Dig Site
* Disposition Renewal
* DLO Survey
* DML Survey
* DPI Survey
* Drafting
* Earthwork Support
* Earthwork Survey
* Easement
* Elevation Survey
* Elevations
* Energy Regulator Application
* Engineering Survey
* Establishment of Monuments
* Estimating
* Explanatory Plan
* Facility
* Facility Abandonment
* Fence Line
* Final Grade Certificate
* Form Board
* Foundation Survey
* Garage Pad Stakeout
* Geotechnical Site Plan
* Gravel Pit
* Gridlines
* Ground Control
* Ground Penetrating Radar
* House Stakeout
* Individual Ownership Plan
* Integrity Survey
* Investigative Survey
* Junction
* Land Act Survey
* Lease Extension
* Lease Measurement
* Lease Survey
* Legal Survey
* LiDAR
* Limit Stakeout
* Liner Pull
* Locating
* Machine Control Support
* Mapping
* Material Surface Lease (MSL)
* Mechanical Survey
* Meter Site
* Miscellaneous
* Miscellaneous Stake-Out
* MLL Sketch Plan Conversion
* MLL Survey
* Monitor Site
* Monitor Wells
* Monitoring
* Monument Establishment
* Monument Plan
* Natural Boundary
* New House Construction
* New House Construction (Multiple Houses)
* Notification Plan
* On Lease
* Ongoing Project
* Pad Site
* Phase I Environmental Site Assessment
* Phase II Environmental Site Assessment
* Photo Mosaic
* Pile Layout
* Piling Survey
* Pipeline Abandonment
* Pipeline Survey
* Plant Site
* Plat
* Plot Plan
* Post Construction Plan
* Posting Plan
* Power Line
* Preliminary P/L Routing
* Preliminary Survey
* Profile
* Property Line Establishment
* Proposal
* Pump Station
* QA / QC Survey
* Radius Map
* Railway
* Re-bore
* Re-Flag Pipeline
* Re-Flag Wellsite
* Real Property Report
* Real Property Report Update
* Reclamation
* Reclamation Survey
* Reference Plan
* Remediation
* Remote Sump
* Residence Sketch
* Right of Way
* Riparian Survey
* Riser Site
* Road Layout
* Road Plan & Survey
* Rough Grade Certificate
* Satellite Site
* Septic System Design
* Sewer
* Site Grading
* Site Layout
* Site Survey
* Sketch Plan
* Slab Survey
* SML Survey
* Spill Response
* Spill Site
* Staking
* Storage Site
* Strata
* Strata Condominium
* Strata Duplex
* Strata Townhouse
* Structural Survey
* Subdivision
* Sump
* Temp Work Space
* Test Lead
* Title Survey
* Tool Tracking
* Topographic Survey
* Topographic Survey for Addition/Renovation
* Topographic Survey for Development
* Topographic Survey for New House
* Topographical
* Tower Site
* Truck Terminal Site
* Turbine
* UAV Inspection
* UAV Survey
* Underground Utility Survey
* Utility ROW
* Valve Site
* Vent Site
* Verification
* Volumetric Survey
* Water Act Application
* Water Hub
* Water Line
* Water Source
* Water Well
* Well Site
```

## File: Job_Maps.mdx/Job_Maps.mdx
```
---
title: 'Job Maps'
description: 'Maximize efficiency in land surveying with our Job Maps feature, allowing staff to search and filter through past job records, ensuring precise project management and operational oversight.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Job_maps_1.jpg';
import img2 from '~/assets/images/help/Job_maps_2.jpg';
import img3 from '~/assets/images/help/Job_maps_3.jpg';
import img4 from '~/assets/images/help/Job_maps_4.jpg';
import img5 from '~/assets/images/help/Job_maps_5.jpg';

Managers and Administrators can search past jobs using the **Job Maps** feature.

Click **Search** in the **Job Maps** card on the dashboard. 

<Screenshot image={img1} alt="Job Maps - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

This screen shows the jobs, job locations and a map of job locations. A maximum of 1000 jobs will be shown, so be sure to filter the jobs and locations by adding filters to narrow down your results.

A filter can be added by clicking the '+' icon in the **Advanced Job filter**. The following fields can be filtered:

* Job #
* Status
* Client Name
* Client Type
* Project Name
* Office
* Project Manager
* Municipal Address
* State / Province
* City
* Category
* Scope
* Order Date
* Due Date
* Active
* Lot
* Block
* Plan Number
* LSD
* Section Number
* Township Number
* Range Number
* Meridian

<Screenshot image={img2} alt="Job Maps - Searching Jobs With Advanced Filtering" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img3} alt="Job Maps - Visualizing Search Results - Job Mapping Software" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img4} alt="Job Maps - Job Search Results Grid" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img5} alt="Job Maps - Job Location Results Grid" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Job_Setup.mdx/Job_Setup.mdx
```
---
title: 'Job Setup'
description: 'Learn how to set up a job efficiently with a detailed guide covering basic configuration, billing settings, adding and managing line items, and job legal addresses.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Job_setup_1.jpg';
import img2 from '~/assets/images/help/Job_setup_2.jpg';
import img3 from '~/assets/images/help/Job_setup_3.jpg';
import img4 from '~/assets/images/help/Job_setup_4.jpg';
import img6 from '~/assets/images/help/Job_setup_6.jpg';
import img7 from '~/assets/images/help/Job_setup_7.jpg';
import img8 from '~/assets/images/help/Job_setup_8.jpg';
import img9 from '~/assets/images/help/Job_setup_9.jpg';
import img10 from '~/assets/images/help/Job_setup_10.jpg';
import img11 from '~/assets/images/help/Job_setup_11.jpg';

<TableOfContents>
    <ol>
        <li>
            <a href="#basic-configuration">Basic Configuration</a>
        </li>
        <li>
            <a href="#billing-configuration">Billing Configuration</a>
        </li>
        <li>
            <a href="#adding-line-items">Adding Line Items</a>
        </li>
        <li>
            <a href="#archiving-and-removing-line-items">Archiving and Removing Line Items</a>
        </li>
        <li>
            <a href="#activating-and-deactivating-jobs">Activating and Deactivating Jobs</a>
        </li>
    </ol>
</TableOfContents>

## Basic Configuration

To set up a new job, click **Create New** in the **Jobs** card on the dashboard. 

<Screenshot image={img1} alt="Job Setup - Create New" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Assign job \#
The job number will count up with each job by default.

#### Assign Client
Choose a client from the client drop-down menu. The client list is imported from [Clients](/help/Clients).

<Screenshot image={img2} alt="Job Setup - Client Selection" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

After selecting a client, the **client's location** can be selected which populates the Client Address.

#### Project Name
Name of the project which will appear on reports, and will be searchable when selecting a job from DWRs and Invoices.

#### Status
The status of the project which will show up on the Active Job Dashboard and Job Maps.

### Locations
    The work locations for the job. These will show up on the Invoices for the job, and all location fields will be searchable in Job Maps.

#### Location Name
A meaningful name to identify the location.

#### Municipal Address

#### State/Province

#### City

#### Legal Addresses
You can enter any number of legal addresses, and specify any combination of legal address fields.

#### GPS Coordinates
Enter coordinates manually or click in the Map Display to set the coordinates.

### Contacts
One or more client contacts that are relevant to the job.

You can select NEW CONTACT to enter details from a contact who is not already in the client. The new contact will be automatically added to the client after saving the job.

#### Add to DWR/Invoice
Check to add this contact to the DWR or Invoice PDF/Word export document.

<Screenshot image={img3} alt="Job Setup - Project Name, Project Status" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Project Manager
The employee who is responsible for DWR and Invoice approvals for this job.

#### Salesperson / Representative

<Screenshot image={img4} alt="Job Setup - Project Manager, Salesperson / Representative" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Office
The office which is responsible for the job/project, and can be used for filtering various reports.

#### Client Project \#
The \# that your client uses to refer to this job.

#### PO \#
The purchase order number for the job.

#### PO Amount
The dollar value of the job, which is used in various cost reports.

#### Subcontract \#
Subcontract number for the job, if any.

## Billing Configuration

### DWR Billing Type

#### Overhead
This is an internal job which will capture overhead or administration time that is not related to client work.

#### Non-Chargeable
This job is related to a client, but the DWRs will not be invoiced to the client.

#### Fixed Price
This job will be invoiced for a set price and does not depend on the hours worked or the equipment used on the job. DWRs will not be invoiced, and an invoice will need to be created manually as described in Invoicing a Fixed Price Job.

#### Time & Material
This job will be invoiced based on the hours worked and the equipment used on the job. Invoices will be generated based on the DWRs for this job as described in Invoicing a Time & Materials Job.

### Invoice Type

#### Ticket / Invoice
If client requires a ticket before invoicing. A ticket will be created from a set of DWRs, and will then become an invoice after customer approval.

#### Invoice
Will create an invoice without involving customer ticket approval.

### Invoice Line Item Type

#### Detailed
Invoices will show each line item billed to the job.

#### Summarized
Invoices will roll-up the line items based on type, and produce a shorter invoice document.

<Screenshot image={img6} alt="Job Setup - DWR Billing Type, Invoice Type, Invoice Line Item Type" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

The following shows the difference between **detailed** and **summarized** invoices:

<Screenshot image={img7} caption="Job Setup - Detailed Invoice Example" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img8} caption="Job Setup - Summarized Invoice Example" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Taxes
Any number of taxes can be entered, which will added to any invoice for this job.

#### Fees
Any number of fees can be entered, which will added to any invoice for this job. The fees are calculated as a percentage of the labour, equipment and fixed price totals before taxes.

#### Additional Fields
Custom fields can be defined which will be added to any invoice for this job.

## Adding Line Items

**Line Items** can be added to a job, which will be available for employees to select on their DWRs. The billable line items include labour costs, equipment & materials, and fixed prices.

#### Rate Sheet
To populate the line items from an existing Rate Sheet, select the appropriate Rate Sheet and click 'Replace Line Items With Rate Sheet'.
Note: Rate Sheets can no longer be applied after the job is used by DWRs or Invoices.

#### Labour Costs
Click the 'Add' button to add a new Labour Cost, and select from the items imported from [Labour Cost Line Items](/help/Administration_Settings#labour-cost-items). Any of the fields (Name, Unit, Unit Cost ($), Budget Quantity, Hourly Cost, Tax Exempt) can be customized.

#### Equipment and Materials
Click the 'Add' button to add a new item, and select from the items imported from [Equipment and Materials](/help/Administration_Settings#equipment-and-materials). Any of the fields (Name, Unit, Unit Cost ($), Budget Quantity, Tax Exempt) can be customized.

#### Fixed Price
Click the 'Add' button to add a new item, and select from the items imported from [Fixed Price Items](/help/Administration_Settings#fixed-price-items). Any of the fields (Name, Unit, Unit Cost ($), Budget Quantity, Tax Exempt) can be customized.

#### Additional Fields
If you would like users to enter additional information on labour and equipment line items in their DWRs, you can add **Additional Fields** for that line item.

## Archiving and Removing Line Items

Line Items can be Archived by checking the **Archived** checkbox. An Archived line item cannot be selected in new DWRs.

Line Items can be removed by clicking the 'X' button to the left of the line item. If the line item is already referenced by existing DWRs or Invoices, the line item will instead by Archived. 

<Screenshot image={img9} alt="Job Setup - Archiving and Removing Line Items" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users can set up more administrative information when users create the job including GL code prefix, Job Categories (Engineering, GIS, Pipeline..etc), Job Scope, Order Date, and Due Date

Moreover, users can set the tax, fees, and additional fees for the job if there are any. Tax (GST, HST, PST) will be added to the invoice. Users can define the fees as administrative fees, discounts, or anything that they want to be shown and calculated on the invoice. and the fee is before tax. The additional fee is for users' specific needs like a work order number or cost center, and it will be shown on the invoice. 

<Screenshot image={img10} alt="Job Setup - Taxes, Fees, Additional Fields" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img11} alt="Job Setup - Taxes and Fees on Invoices" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Activating and Deactivating Jobs

The **Active** checkbox at the bottom of the form is checked by default. When a job is Active, it can be selected by users when entering DWRs. When a job is closed out, make sure to edit the job and uncheck the Active checkbox so users can no longer record time to it.
```

## File: leave-request-initial-setup.mdx/leave-request-initial-setup.mdx
```
---
title: 'Leave Request Initial Setup'
description: 'Learn how to set up the Leave Request module in Job Book, including configuring jobs, leave types, and employee profiles.'
layout: '~/layouts/HelpLayout.astro'
---

import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';
import leaveRequestSetupEmployee from '~/assets/images/help/leave-request-setup/leave-request-setup-employee.png';

<TableOfContents>
    <ol>
        <li><a href="#key-concepts">Key Concepts</a></li>
        <li><a href="#performing-common-tasks">Performing Common Tasks</a></li>
    </ol>
</TableOfContents>

## Key Concepts

Before you can use the Leave Request module, there are a few key concepts you need to understand.

### Eligible Jobs

Only certain jobs are eligible for use in a Leave Request or to be set as a Leave Job in an employee's profile. These jobs must have their **DWR Billing Type** set to **Overhead**. You can learn more about setting up jobs in the [Job Setup](/help/Job_Setup) documentation.

### Leave Types

In Job Book, "Leave Types" are actually **Labour Cost Items**. These are the different types of leave that employees can request, such as "Vacation," "Sick Leave," or "Personal Day." These Labour Cost Items should be configured with the following settings:

*   **Unit**: Set to "HR" (for hours)
*   **Billing Unit Cost**: Set to $0.00

It's a good practice to group all your leave-related Labour Cost Items together under a single category, such as "Leave," for better organization. You can find more information on creating and managing Labour Cost Items in the [Administration Settings](/help/Administration_Settings#labour-cost-items) documentation.

### Employee Profiles

For the Leave Request system to work correctly, each employee's profile must be updated with two specific fields:

*   **Leave Job**: This is the default job that will be used when the employee creates a leave request.
*   **Leave Manager**: This is the employee's manager who will approve or deny their leave requests.

### Weekend Configuration

The system can be configured to either include or exclude weekends when calculating the duration of a leave request. This setting is not user-configurable and must be changed by contacting Cyanic Automation.

## Performing Common Tasks

Here is the typical workflow for setting up the Leave Request module for the first time.

### 1. Create Labour Cost Items

The first step is to create a **Labour Cost Item** for each type of leave you want to make available to your employees.

1.  Navigate to **Administration -> Labour Cost Items**.
2.  Click **Create New**.
3.  Fill in the details for the new leave type. Remember to set the **Unit** to "HR" and the **Billing Unit Cost** to "$0".
4.  Repeat this process for all the leave types you need.

For more detailed instructions, please see the [Administration Settings](/help/Administration_Settings#labour-cost-items) documentation.

### 2. Create a Leave Job

Next, you need to create one or more "Leave Jobs." These are the jobs that will be used to track all leave requests. You might need more than one Leave Job if your company has multiple offices or different tracking requirements.

1.  Navigate to the **Jobs** dashboard and click **Create New**.
2.  Give the job a descriptive name, such as "Internal - Leave Tracking."
3.  **Crucially, set the DWR Billing Type to "Overhead."** This is what makes the job eligible for leave tracking.
4.  In the **Line Items** section, add all the leave-related **Labour Cost Items** that you created in the previous step.

For a complete guide to creating jobs, refer to the [Job Setup](/help/Job_Setup) page.

### 3. Update Employee Profiles

Finally, you need to update each employee's profile to link them to the Leave Request system.

1.  Click **Settings** in the top right of the screen, then click **Employee Profiles**.
2.  Click on an employee to view their profile.
3.  Click **Edit**.
4.  Set the **Leave Job** to the Leave Job you created in the previous step.
5.  Set the **Leave Manager** to the employee's direct manager.
6.  Save the changes.

<Screenshot image={leaveRequestSetupEmployee} alt="Leave Request Setup in Employee Profile" caption="Set the Leave Job and Leave Manager for the employee." classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Repeat this process for all employees who will be using the Leave Request system.

<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/leave-tracking-overview">Leave Tracking: Overview</a></li>
        <li>Leave Request Initial Setup</li>
        <li><a href="/help/leave-request">Leave Requests</a></li>
        <li><a href="/help/leave-request-report">Leave Request Report</a></li>
        <li><a href="/help/company-calendar">Company Calendar</a></li>
    </ol>
</TableOfContents>
```

## File: leave-request-report.mdx/leave-request-report.mdx
```
---
title: Leave Request Report
description: Learn how to use the Leave Request Report to view, sort, and filter leave requests across the company.
layout: '~/layouts/HelpLayout.astro'
---

import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';
import LeaveRequestReportNav from '~/assets/images/help/leave-request-report/leave-request-report-nav.png';
import LeaveRequestReport from '~/assets/images/help/leave-request-report/leave-request-report.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#key-concepts">Key Concepts</a>
        </li>
        <li>
            <a href="#performing-common-tasks">Performing Common Tasks</a>
            <ul>
                <li>
                    <a href="#accessing-the-report">Accessing the Report</a>
                </li>
                <li>
                    <a href="#understanding-the-data">Understanding the Data</a>
                </li>
                <li>
                    <a href="#sorting-and-filtering">Sorting and Filtering</a>
                </li>
                <li>
                    <a href="#navigating-the-report">Navigating the Report</a>
                </li>
                <li>
                    <a href="#saving-and-loading-custom-report-views">Saving and Loading Custom Report Views</a>
                </li>
                <li>
                    <a href="#exporting-to-excel">Exporting to Excel</a>
                </li>
            </ul>
        </li>
    </ol>
</TableOfContents>

## Key Concepts

The Leave Request Report provides a comprehensive, company-wide view of all leave requests. It is a powerful tool for managers and administrators to track employee leave, monitor trends, and ensure that staffing levels are adequate. Unlike views that only show your own requests, this report shows all leave requests in the system, giving you a complete picture of employee availability.

## Performing Common Tasks

### Accessing the Report

The Leave Request Report is available to users with Administrator or Manager permissions.

1.  From the main dashboard, locate the **Leave Requests** card.
2.  Click on the **Leave Request Report** link to open the report.

<Screenshot
    image={LeaveRequestReportNav}
    alt="Navigation to Leave Request Report"
    caption="Access the Leave Request Report from the dashboard."
/>

### Understanding the Data

The report is organized into a grid that provides a comprehensive overview of all leave requests.

<Screenshot
    image={LeaveRequestReport}
    alt="Leave Request Report View"
    caption="The Leave Request Report, showing all leave requests."
/>

The grid contains the following columns:

*   **LR #**: The unique identification number for the leave request. Clicking this number will take you directly to the details of that specific request.
*   **Employee**: The name of the employee who submitted the request.
*   **Job #**: The leave-related job associated with the request. Clicking this number will navigate you to the job details.
*   **Leave Type**: The specific category of leave requested (e.g., Vacation, Sick Day).
*   **Manager**: The manager responsible for approving the request.
*   **Leave Period**: Indicates whether the request is for **Full Day(s)** or a **Partial Day**.
*   **Request Start / End**: The start and end dates of the leave period.
*   **Start Time / End Time**: The specific start and end times for partial-day requests.
*   **Submitted**: The date the leave request was submitted by the employee.
*   **Status**: The current status of the request, which can be **Not Submitted**, **Approved**, or **Rejected**.

### Sorting and Filtering

You can easily organize and find the information you need using the built-in sorting and filtering tools.

*   **Sorting**: To sort the report by any column, simply click on the column header. For example, clicking the **Employee** header will sort the list alphabetically by employee name. Clicking it again will reverse the sort order.
*   **Filtering**: To apply a filter, hover over the header of the column you want to filter and click the column menu icon (three vertical dots). This opens the filter menu, which provides several options to narrow down your data.

    For example, to find all approved leave requests for a specific employee:
    1.  Go to the **Employee** column, click the column menu icon, and type the employee's name into the search box.
    2.  Next, go to the **Status** column, click the column menu icon, and select **Approved** from the list of options.

    The filter menu also provides a list of operators to help you refine your search, such as "Contains," "Starts with," and "Is equal to." You can clear a filter at any time by reopening the column menu and clicking the "Clear" button.

### Navigating the Report

The report displays up to 100 leave requests per page. If there are more than 100 requests, you can use the paging controls at the bottom of the report to navigate forward and back between pages to see all entries.

### Saving and Loading Custom Report Views

The report includes a powerful feature that allows you to save your customized views as templates. A template saves your current settings—including visible columns, column widths, filters, sorting, and grouping—so you can quickly re-apply them later. These templates are saved in your browser and are not shared with other users.

You can manage your templates using the toolbar at the top of the report grid.

*   **To save a new template:**
    1.  Arrange the report exactly as you want it.
    2.  Click the **Save As** button.
    3.  Enter a descriptive name for your template and click **OK**.

*   **To load a saved template:**
    1.  Select the template from the **Select Template...** dropdown list.
    2.  Click the **Load** button.

*   **To update a saved template with your current view:**
    1.  Select the template you want to overwrite from the dropdown list.
    2.  Click the **Save** button and confirm your choice.

*   **To delete a template:**
    1.  Select the template from the dropdown list.
    2.  Click the **Delete** button and confirm.

*   **To reset the report to its default view:**
    *   Click the **Reset** button. This will remove any custom sorting, filtering, or grouping.

### Exporting to Excel

In addition to saving custom views, you can export the report data directly to an Excel file. This is useful for offline analysis, sharing with others, or creating custom charts.

To export the report, look for an **Export to Excel** button or an export icon in the report's toolbar. Clicking this will generate and download an `.xlsx` file containing the data currently displayed in the grid, including any filters or sorting you have applied.

<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/leave-tracking-overview">Leave Tracking: Overview</a></li>
        <li><a href="/help/leave-request-initial-setup">Leave Request Initial Setup</a></li>
        <li><a href="/help/leave-request">Leave Requests</a></li>
        <li>Leave Request Report</li>
        <li><a href="/help/company-calendar">Company Calendar</a></li>
    </ol>
</TableOfContents>
```

## File: leave-request.mdx/leave-request.mdx
```
--- 
title: 'Leave Requests'
description: 'How to create and manage leave requests.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import createNav from '~/assets/images/help/leave-request/leave-request-create-nav.png';
import createRequest from '~/assets/images/help/leave-request/leave-request-create.png';
import exploreNav from '~/assets/images/help/leave-request/leave-request-explore-nav.png';
import approveRequest from '~/assets/images/help/leave-request/leave-request-approve.png';
import awaitingRequest from '~/assets/images/help/leave-request/leave-request-awaiting-my-approval.png';
import dashboardNotification from '~/assets/images/help/leave-request/leave-request-dashboard-notification.png';
import Callout from '~/components/ui/Callout.astro';

<TableOfContents>
    <ol>
        <li><a href="#key-concepts">Key Concepts</a></li>
        <li><a href="#creating-a-leave-request">Creating a Leave Request</a></li>
        <li><a href="#navigating-existing-leave-requests">Navigating Existing Leave Requests</a></li>
        <li><a href="#reviewing-a-leave-request">Reviewing a Leave Request</a></li>
    </ol>
</TableOfContents>

## Key Concepts

A leave request is filled out by an employee to notify management and get approval for any kind of leave, such as:

* Annual Leave
* Compassionate Leave
* Sick Leave
* Unpaid Leave
* Vacation

Leave types are configurable by your administrator. Each employee is assigned a **Leave Job** and a **Leave Manager**. The **Leave Job** is an internal company project used for tracking time off, and the **Leave Manager** is the person who will be notified to approve or reject a leave request.

## Creating a Leave Request

To create a new leave request, find the **Leave Requests** card on your dashboard and click the **Create New** button.

<Screenshot image={createNav} alt="Leave Request Card" caption="The Leave Request card on the dashboard." />

This will open the **Leave Request Form**.

<Screenshot image={createRequest} alt="Leave Request Form" caption="The Leave Request form." />

Fill out the following fields:

*   **Employee**: This will be automatically selected for the current user.
*   **Job**: The Leave Job configured for the employee.
*   **Leave Manager**: The Leave Manager configured for the employee.
*   **Leave Type**: Select the type of leave you are requesting.
*   **Leave Period**: Choose either 'Full Day(s)' or 'Partial Day'.
*   **Start Date**: The date the leave starts.
*   **Start Time**: (Only for 'Partial Day' Leave Type) The time the leave starts.
*   **End Time**: (Only for 'Partial Day' Leave Type) The time the leave ends.
*   **End Date**: (Only for 'Full Day(s)' Leave Type) The date the leave ends.
*   **Description**: A brief description of the leave.
*   **Attachments**: You can attach any number of files to the leave request.
*   **Signature**: If you have a signature saved in your profile, you can click **Add My Signature** to apply it automatically. Otherwise, you can click **Collect Signature** to draw a new one. After adding a signature, you can **View** it or **Delete** it from the request.
*   **Submitted**: This box is checked by default. When submitted, the leave request is sent to your Leave Manager for approval. If you uncheck this box, you can save the request as a draft and come back to it later.

Once you have filled out the form, click **Save**.

## Navigating Existing Leave Requests

To see your existing leave requests, click the **Explore** button on the **Leave Requests** card on your dashboard.

<Screenshot image={exploreNav} alt="Explore Leave Requests" caption="The Explore button on the Leave Requests card." />

This will take you to a list of your leave requests. You can filter the list to see different types of requests:

*   **My Requests (Not Submitted)**: Shows your draft leave requests that have not yet been submitted.
*   **My Requests (Rejected)**: Shows your leave requests that have been rejected by your manager. Once a request is rejected, it cannot be edited or resubmitted.
*   **All My Requests**: Shows all of your leave requests.

If you are a manager, you will see additional views to manage your employees' leave requests:

*   **Awaiting My Approval**: Shows leave requests from your employees that have been submitted but not yet approved or rejected.
*   **Submitted**: Shows all submitted leave requests from all employees that have not yet been approved or rejected.
*   **Rejected**: Shows all rejected leave requests from all employees.
*   **All**: Shows all leave requests from all employees.

## Reviewing a Leave Request

When an employee submits a leave request, their manager will be notified by email and can review it. Managers can access leave requests awaiting their approval in a few ways:

*   From the email notification link.
*   From the **Actions Required** panel on the dashboard.

<Screenshot image={dashboardNotification} alt="Dashboard Notification" caption="The Actions Required panel on the dashboard." />

*   By navigating to the **Awaiting My Approval** view in the leave request list.

<Screenshot image={awaitingRequest} alt="Awaiting Approval List" caption="The 'Awaiting My Approval' view." />

When a manager opens a leave request, they can review the details, make changes if necessary, and then approve or reject it.

<Callout>

**Important:** When a leave request spans multiple days, weekends are automatically excluded by default (this may be configured differently for your site). However, holidays are **not** automatically excluded. The manager must manually deselect any holidays from the calendar by clicking on them before approving the request.

</Callout>

<Screenshot image={approveRequest} alt="Approving a Leave Request" caption="Approving a leave request." />

*   To **approve** a leave request, change the **Approval Status** to 'Approved' and click **Save**. The employee will receive an email notifying them that the request was approved.
*   To **reject** a leave request, change the **Approval Status** to 'Rejected', add any notes for the employee, and click **Save**. The employee will receive an email notifying them that the request was rejected.
*   To **return** a leave request to the employee for changes, uncheck the **Submitted** box and click **Save**. The employee will be notified by email that they need to make changes and resubmit the request.

<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/leave-tracking-overview">Leave Tracking: Overview</a></li>
        <li><a href="/help/leave-request-initial-setup">Leave Request Initial Setup</a></li>
        <li>Leave Requests</li>
        <li><a href="/help/leave-request-report">Leave Request Report</a></li>
        <li><a href="/help/company-calendar">Company Calendar</a></li>
    </ol>
</TableOfContents>
```

## File: leave-tracking-overview.mdx/leave-tracking-overview.mdx
```
---
title: 'Leave Tracking: Overview'
description: 'An overview of the Leave Tracking module in Job Book.'
layout: '~/layouts/HelpLayout.astro'
---

import TableOfContents from '~/components/ui/TableOfContents.astro';

<TableOfContents>
    <ol>
        <li>
            <a href="#introduction">Introduction</a>
        </li>
        <li>
            <a href="#key-concepts">Key Concepts</a>
            <ul>
                <li><a href="#leave-requests">Leave Requests</a></li>
                <li><a href="#approval-workflow">Approval Workflow</a></li>
                <li><a href="#company-calendar">Company Calendar</a></li>
                <li><a href="#leave-request-report">Leave Request Report</a></li>
            </ul>
        </li>
    </ol>
</TableOfContents>

## Introduction

The Leave Request module is designed to streamline the process of requesting, approving, and tracking employee time off. It provides a centralized system for managing all types of leave, from vacation and sick days to personal and compassionate leave. The goal is to make leave management transparent, efficient, and easy for everyone involved.

## Key Concepts

The module is built around a few core concepts:

*   **Leave Requests**: Employees submit leave requests to get approval for time off. Each request includes details like the type of leave, the dates, and a description. This ensures that all necessary information is captured in a standardized way.

*   **Approval Workflow**: Once a request is submitted, it goes to the employee's designated manager for approval. The manager is automatically notified and can review, approve, reject, or return the request for more information. This creates a clear and consistent approval process.

*   **Company Calendar**: The Company Calendar provides a company-wide view of all approved leave. This helps managers and administrators see who is out of the office at a glance, making it easier to plan and schedule work.

*   **Leave Request Report**: For a more detailed analysis, the Leave Request Report offers a comprehensive grid of all leave requests in the system. This powerful tool allows managers to sort, filter, and export leave data to track trends and monitor employee availability.

<TableOfContents title="Related Guides">
    <ol>
        <li>Leave Tracking: Overview</li>
        <li><a href="/help/leave-request-initial-setup">Leave Request Initial Setup</a></li>
        <li><a href="/help/leave-request">Leave Requests</a></li>
        <li><a href="/help/leave-request-report">Leave Request Report</a></li>
        <li><a href="/help/company-calendar">Company Calendar</a></li>
    </ol>
</TableOfContents>
```

## File: Overview.mdx/Overview.mdx
```
---
title: 'Overview'
description: 'Explore Cyanic Job Book''s impact on land surveying companies, enhancing efficiency, accountability, and profitability for all roles.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';

<TableOfContents>
    <ol>
        <li>
            <a href="#what-is-job-book">What is Job Book</a>
        </li>
        <li>
            <a href="#how-will-job-book-improve-my-life">How will Job Book improve my life?</a>
            <ol>
                <li><a href="#administrators">Administrators</a></li>
                <li><a href="#management">Management</a></li>
                <li><a href="#technicians">Technicians</a></li>
            </ol>
        </li>
        <li>
            <a href="#how-will-job-book-improve-my-company">How will Job Book improve my company?</a>
            <ol>
                <li><a href="#improve-profitability">Improve Profitability</a></li>
                <li><a href="#improve-accountability">Improve Accountability</a></li>
                <li><a href="#improve-sustainability">Improve Sustainability</a></li>
            </ol>
        </li>
        <li>
            <a href="#now-is-the-time">Now is the Time</a>
        </li>
    </ol>
</TableOfContents>

## What is Job Book?

Job Book is an easy-to-use project management and workflow system specifically designed for land surveying companies. It helps to automate the flow of value through your company, gives staff the tools they need to stay accountable, and allows you to make better business decisions with realtime analytics and reporting.

Job Book is the result of years of working with survey companies and implementing the very best practices across the whole profession and industry. We have seen first-hand the dramatic improvements in profitability and quality-of-life experienced by our Job Book customers, and we hope you love it as much as our other customers.

## How will Job Book improve my life?

Job Book helps in different ways depending on your role.

### Administrators

1. You will spend much less time:
    * Collecting daily work records and other paperwork from employees.
    * Preparing for payroll and reimbursement activities.
    * Getting project information and approvals from project managers.
    * Creating invoices and keeping track of what work still needs to be billed.
    * Keeping different rate sheets organized across different customers and different kinds of jobs.
    * Generating reports and KPIs for management.
    * Getting data into your accounting system.
2. You will find it reassuring that the system automatically coordinates project manager approvals of invoices and other processes to dramatically reduce the amount of mistakes that could show up during billing.
3. It will be easier to support your customers, with all job information being a few clicks away.
4. You will be able to get your weekends back.

### Management

1. You will be able to see the status and financial health of your jobs in real-time.
2. You will be able to see when a job is going off-track, so you can make that call to your client now, instead of waiting until the end of the month or the end of the project when the hours are tallied up.
3. You will be able to easily search past jobs by area or any information, so that you can easily put together estimates for new jobs.
4. You will be able to catch errors in records submitted by your team, and improve the profitability of your jobs.
5. You will be able to delegate your job activities to other managers, as project information is centralized and easy to pick-up.
6. You will no longer have to wait for Accounting/Bookkeeping to tell you if you are making or losing money on a job.

### Technicians

1. You will spend much less time filling out paperwork.
2. You will find it easier to enter hours and equipment against your jobs.
3. You will spend less time asking your manager about which line items you should be using.
4. You will be able to easily view all of your hours and the status of your expenses.
5. People will stop bugging you about your handwriting or losing paper in the truck.

## How will Job Book improve my company?

Job Book will transform your company and help take things to the next level.

### Improve Profitability

1. Reduce the mistakes that lead to under-billing.
2. Invoice your customers much more quickly.
3. Reduce the amount of overhead across all roles in the company. Administrators will now have more time to do crew organization, scheduling, safety, make marketing materials and book-keeping.
4. Learn what your best kinds of clients and jobs are, so you can focus on what makes you the most money
5. Find where you're coming up short on estimates and where you need to raise your rates.
6. Reduces the pain of growing your company by automating processes and keeping information centralized and organized for everyone who needs it.
7. Makes it much easier to merge with or acquire other companies by having everyone work on the same system.
8. Make more money from your equipment, learn which equipment are most utilized or are bottlenecks.
9. Staff can more easily work remotely, with less communication with the office.
10. When the company makes more money, you will be able to hire the best surveying talent to work different kinds of jobs or increase capacity.

### Improve Accountability

1. Staff are given the tools and are incentivized to enter hours accurately.
2. The system keeps track of what actions must be completed and by whom, so nothing falls through the cracks.
3. Improves visibility on jobs and operations across the organization, and shines a light on problem areas to allow faster correction.
4. Improved clarity around roles and responsibilities results in less conflict between employees.

### Improve Sustainability

1. It will be easier to on-board new hires, and integrate them into a solid existing process.
2. Reduce the pain and lost knowledge from the departure of key staff, as all project information is centralized and easily reassigned.
3. Increasing the amount of time staff spend on what they love and reducing the time spent on tedious overhead will dramatically improve employee retention.
4. When survey companies are more profitable, it improves the stature and sustainability of the whole surveying profession!

## Now is the Time

So, with all of that out of the way, let's get your Job Book system set up as quickly as possible, so you can spend more time doing what you love.

We will be with you every step of the way.

Sincerely,

Mike & Doug, and the Cyanic Job Book team.

_PS: If you don't already have Job Book, [Get Job Book](https://getjobbook.com)_
```

## File: Personal_Reports.mdx/Personal_Reports.mdx
```
---
title: 'Personal Reports'
description: 'Discover how to easily navigate Personal Reports in our project management tool for land surveyors. Track your time cards and expenses with clear, detailed views.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Personal_reports_1.jpg';
import img2 from '~/assets/images/help/Personal_reports_2.jpg';
import img3 from '~/assets/images/help/personal_reports_3.jpg';

In Job Book, employees can review the time cards and expenses they entered or were entered for them.

## My Time Cards

<Screenshot image={img1} alt="Personal Reports - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click **My Time Cards** in the Personal Reports card on the dashboard.

Enter a date range and click **Load Data**. Time cards falling within the date range will be displayed, showing the job number, DWR number, project name, line item, status, and hours. Total hours are summed up at the bottom of the report. 

<Screenshot image={img2} alt="Personal Reports - My Time Cards" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## My Expenses

Click **My Expenses** in the Personal Reports card on the dashboard.

Enter a date range and click **Load Data**.

<Screenshot image={img3} alt="Personal Reports - My Expenses" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: personal-task-management.mdx/personal-task-management.mdx
```
---
title: 'Personal Task Management'
description: 'How to manage your personal tasks, both scheduled and unscheduled.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import mySchedule from '~/assets/images/help/personal-task-management/my-schedule.png';
import myUnscheduledTasks from '~/assets/images/help/personal-task-management/my-unscheduled-tasks.png';
import myScheduleChangeTaskStatus from '~/assets/images/help/personal-task-management/my-schedule-change-task-status.png';
import myScheduleNav from '~/assets/images/help/personal-task-management/my-schedule-nav.png';
import myUnscheduledTasksNav from '~/assets/images/help/personal-task-management/my-unscheduled-tasks-nav.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#overview">Overview</a>
        </li>
        <li>
            <a href="#my-schedule">My Schedule</a>
            <ul>
                <li><a href="#accessing-my-schedule">Accessing My Schedule</a></li>
                <li><a href="#viewing-your-schedule">Viewing Your Schedule</a></li>
                <li><a href="#changing-task-status-in-my-schedule">Changing Task Status</a></li>
            </ul>
        </li>
        <li>
            <a href="#my-unscheduled-tasks">My Unscheduled Tasks</a>
            <ul>
                <li><a href="#accessing-my-unscheduled-tasks">Accessing My Unscheduled Tasks</a></li>
                <li><a href="#viewing-your-unscheduled-tasks">Viewing Your Unscheduled Tasks</a></li>
                <li><a href="#changing-task-status-in-my-unscheduled-tasks">Changing Task Status</a></li>
            </ul>
        </li>
    </ol>
</TableOfContents>

## Overview

You can manage your personal tasks in Job Book using two main screens: "My Schedule" and "My Unscheduled Tasks". "My Schedule" provides a calendar view of your scheduled tasks, while "My Unscheduled Tasks" acts as your personal pool of available tasks that are not placed on the calendar. This allows you to have a clear overview of your workload and prioritize your tasks effectively.

## My Schedule

"My Schedule" provides a calendar view of your tasks for the current week. It is designed to give you a clear overview of your workload and help you plan your time effectively.

### Accessing My Schedule

Access your schedule by clicking on 'My Schedule' in the 'My Tasks' card on the dashboard.

<Screenshot
  image={myScheduleNav}
  alt="My Schedule Navigation"
  caption="Access 'My Schedule' from the dashboard."
/>

### Viewing Your Schedule

-   **Navigate the Calendar:** Use the `<` and `>` buttons to move between weeks, or click the calendar icon to select a specific date.
-   **Task Display Limit:** The weekly view shows a maximum of 4 tasks per day. If a day has more than 4 tasks, they are grouped into a single item labeled "...".
-   **View Daily Details:** Click on any day to see the full, detailed list of tasks for that date.
-   **Task Card Information:** Each task is displayed on its own card, which includes the job number, client, task name, duration, description, status, and a clickable link to the job's location on Google Maps.

Tasks are color-coded to indicate their status, making it easy to see what needs your attention.

-   **Not Started:** Blue
-   **In Progress:** Orange
-   **Completed:** Green

<Screenshot
  image={mySchedule}
  alt="My Schedule"
  caption="The 'My Schedule' view provides a weekly overview of your tasks."
/>

### Changing Task Status in My Schedule

1.  Click on a day to view the task details.
2.  Click the 'Edit Task Status' button for the relevant task.
3.  You can change the status from 'Not Started' to 'In Progress' or 'Completed', and from 'In Progress' to 'Completed'. Completed tasks will still be displayed on your schedule, but their status will be updated.

<Screenshot
  image={myScheduleChangeTaskStatus}
  alt="Change Task Status"
  caption="You can change the status of a task from the task detail view."
/>

## My Unscheduled Tasks

"My Unscheduled Tasks" is a list of your available, unschedulable tasks, sorted by their due date. This acts as a to-do list, allowing you to see all the tasks that are ready for you to work on.

### Accessing My Unscheduled Tasks

Access your unscheduled tasks by clicking on 'My Unscheduled Tasks' in the 'My Tasks' card on the dashboard.

<Screenshot
  image={myUnscheduledTasksNav}
  alt="My Unscheduled Tasks Navigation"
  caption="Access 'My Unscheduled Tasks' from the dashboard."
/>

### Viewing Your Unscheduled Tasks

Each task is displayed on a card with the job number, client, task name, duration, description, status, and a link to the job location on Google Maps.

<Screenshot
  image={myUnscheduledTasks}
  alt="My Unscheduled Tasks"
  caption="The 'My Unscheduled Tasks' view shows a list of all your unscheduled tasks, sorted by due date."
/>

### Changing Task Status in My Unscheduled Tasks

1.  Click the 'Edit Task Status' button for the relevant task.
2.  You can change the status from 'Not Started' to 'In Progress' or 'Completed', and from 'In Progress' to 'Completed'.
3.  Once a task is marked as 'Completed', it will be removed from this list.

<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/tasks-and-scheduling-overview">Tasks and Scheduling: Overview</a></li>
        <li><a href="/help/task-templates">Task Templates</a></li>
        <li><a href="/help/task-plans">Task Plans</a></li>
        <li><a href="/help/task-scheduling">Task Scheduling</a></li>
        <li>Personal Task Management</li>
        <li><a href="/help/task-dashboard">Task Dashboard</a></li>
    </ol>
</TableOfContents>
```

## File: Rate_Sheets.mdx/Rate_Sheets.mdx
```
---
title: 'Rate Sheets'
description: 'Explore how to create and manage Rate Sheets templates for different clients or job types, detailing labour costs, equipment, materials, and fixed price items.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Rate_sheet_1.jpg';
import img2 from '~/assets/images/help/Rate_sheet_2.jpg';
import img3 from '~/assets/images/help/Rate_sheet_3.jpg';
import img4 from '~/assets/images/help/Rate_sheet_4.jpg';

A **Rate Sheet** is a template for a set of line items and prices that can be applied to a Job. Multiple Rate Sheets can be created to help organize and standardize rates for different clients or types of jobs.

From the dashboard, click **Create New** in the **Rate Sheet** card. 

<Screenshot image={img1} alt="Rate Sheets - Create New" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

#### Name
Name the rate sheet according to the use of the sheet (e.x., Acme Corp Standard Rates).

#### Note
Add a comment to the rate sheet.

## Labour Costs

The labour cost items are imported from the [Administration / Labour Cost Items](/help/Administration_Settings#labour-cost-items). Users can select which type of labour cost item they want to list down in the rate sheet. Name the item, and provide unit, unit cost ($), hourly cost, and tax/not taxed information to the rate sheet.

<Screenshot image={img2} alt="Rate Sheets - Labour Costs" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Equipment and Materials

The equipment and materials items are imported from the [Administration / Equipment and Materials](/help/Administration_Settings#equipment-and-materials). Users can select equipment and materials they need to list down in the rate sheet. Name the item, and provide unit, unit cost ($) and tax/not taxed information to the rate sheet.

<Screenshot image={img3} alt="Rate Sheets - Equipment and Materials" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Fixed Price Items

The fixed price items are imported from the [Administration / Fixed Price Items](/help/Administration_Settings#fixed-price-items). Users can select what item t need and list it down in the rate sheet. Name the item, and provide unit, unit cost ($) and tax/not taxed information to the rate sheet. 

<Screenshot image={img4} alt="Rate Sheets - Fixed Price Items" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Reports.mdx/Reports.mdx
```
---
title: 'Reports'
description: 'Maximize efficiency in land surveying with our SaaS tool''s detailed reports feature. Easily generate, filter, and export critical project data to excel, tailored for surveyor needs.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Reports_1.jpg';
import img2 from '~/assets/images/help/Reports_2.jpg';
import img3 from '~/assets/images/help/Reports_3.jpg';
import img4 from '~/assets/images/help/Reports_4.jpg';
import img5 from '~/assets/images/help/Reports_5.jpg';

## Line Item Report

The line item report shows all line items recorded in DWRs for a date range. 

<Screenshot image={img1} alt="Line Item Report - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

On the Line Item Report page, users can load the data by selecting the date range. The line item details include the job#, line item, type, DWR#, Employee, Quality, Unit, DWR Status, and Description. 

<Screenshot image={img2} alt="Line Item Report - Loading Data" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Users can export the data to Microsoft Excel if needed. By clicking the filter icon, users can filter the data they need. Also, the data can be grouped with the column header by dragging the header. 

<Screenshot image={img3} alt="Line Item Report - Exporting to Microsoft Excel" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Work in Progress (WIP) Report

The WIP report shows all hours and equipment recorded in DWRs for a date range, with the corresponding invoice entries. 

<Screenshot image={img4} alt="WIP Work in Progress Report - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img5} alt="WIP Work in Progress Report - Loading Data" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Site_Staff_DWR_Entry.mdx/Site_Staff_DWR_Entry.mdx
```
---
title: 'Site Staff DWR Entry'
description: 'Learn how to create Daily Work Records (DWRs) for you or your crew in Job Book, including entering hours, equipment, and securing approvals.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Site_staff_dwr_entry_1.jpg';
import img2 from '~/assets/images/help/Site_staff_dwr_entry_2.jpg';
import img3 from '~/assets/images/help/Site_staff_dwr_entry_3.jpg';
import img4 from '~/assets/images/help/Site_staff_dwr_entry_4.jpg';
import img5 from '~/assets/images/help/Site_staff_dwr_entry_5.jpg';
import img6 from '~/assets/images/help/Site_staff_dwr_entry_6.jpg';

Hello new Job Book user!

You can enter hours and equipment for you or your team by creating Daily Work Records (DWRs).

Click Create New in the "Daily Work Record" card on the dashboard to start entering your DWR. 

<Screenshot image={img1} alt="Site Staff DWR Entry - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Enter the date and select a job. Once you do this, you will be able to fill out the rest of the DWR. 

<Screenshot image={img2} alt="Site Staff DWR Entry - Job Selection" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Next, you can add labour costs and equipment/materials.

#### Labour Cost
Information on cost items, employees, time cards, and descriptions are available in this section.

#### Equipment and Material
Information on cost items (incidentals, equipment, and material), names, units, and quantities are available in this section.

<Screenshot image={img3} alt="Site Staff DWR Entry - Adding Labor Line Items" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img4} alt="Site Staff DWR Entry - Adding Equipment and Materials Line Items" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img5} alt="Site Staff DWR Entry - Reviewing Job Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

After filling in the DWR details, you will add a representative signature for the DWR, and collect the client's signature if needed. 

<Screenshot image={img6} alt="Site Staff DWR Entry - Collecting Signatures" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

When you are finished, check the **Submitted** checkbox and save the DWR. Your DWR will then go to the Project Manager for approval.
```

## File: Site_Staff_Expense_Entry.mdx/Site_Staff_Expense_Entry.mdx
```
---
title: 'Site Staff Expense Entry'
description: 'Learn how to create and submit expenses on Job Book for internal reimbursement with our step-by-step guide, including adding attachments and details.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Site_staff_expense_entry_1.jpg';
import img2 from '~/assets/images/help/Expense_2.jpg';
import img3 from '~/assets/images/help/Expense_3.jpg';

This page will guide the users to create the expense on Job Book. Employees can create the expense for the internal reimbursement process.

Go to **Expense** on Home Page and click **Create New**. Users can input the date, employee name, the jobs are the employees working on, expense items, and the total amount. Users can add attachments and descriptions here. Don't forget to check the submit checkbox and save the expense.

<Screenshot image={img1} alt="Site Staff Expense Entry - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img2} alt="Site Staff Expense Entry - Expense Details" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img3} alt="Site Staff Expense Entry - Submitting" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Site_Staff_Initial_Setup.mdx/Site_Staff_Initial_Setup.mdx
```
---
title: 'Site Staff Initial Setup'
description: 'Learn how to set up your Job Book account with our step-by-step guide. From receiving your confirmation email to setting your password and creating a reusable signature.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Site_staff_setup_1.jpg';
import img2 from '~/assets/images/help/Site_staff_setup_2.jpg';
import img3 from '~/assets/images/help/Site_staff_setup_3.jpg';
import img4 from '~/assets/images/help/Site_staff_setup_4.jpg';
import img5 from '~/assets/images/help/Site_staff_setup_5.jpg';

Hello new Job Book user!

This section will guide you through the setup process for your new Job Book account.

Once your administrator has created your user, you will receive a confirmation email from no-reply@cyanicautomation.com with the subject:

* Your user to access \<company name\> has been created.

Open this email and click on the link to go to Job Book and set your password. 

<Screenshot image={img1} alt="Site Staff Setup - Confirmation Email" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

The new password must be at least 6 characters long. It should also follow your internal password policy. Once your password has been accepted you will be redirected to your dashboard. 

<Screenshot image={img2} alt="Site Staff Setup - Setting Password" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

If the message "Your user does not have an Employee Profile. Please contact your administrator." shows, please contact your administrator to create your employee profile. 

<Screenshot image={img3} alt="Site Staff Setup - Employee Profile Validation" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

The next step is to set up your signature so you can save time when signing forms. 

<Screenshot image={img4} alt="Site Staff Setup - Reusable Signature Notification" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

You can enter the signature by drawing on the signature pad, or you can upload an image containing your signature. 

<Screenshot image={img5} alt="Site Staff Setup - Reusable Signature Setup" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: Site_Staff_Personal_Reports.mdx/Site_Staff_Personal_Reports.mdx
```
---
title: 'Site Staff Personal Reports'
description: 'Explore your Personal Reports on Job Book to manage your time cards and expenses efficiently.'
layout: '~/layouts/HelpLayout.astro'
---
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Site_staff_personal_reports_1.jpg';
import img2 from '~/assets/images/help/Personal_reports_2.jpg';
import img3 from '~/assets/images/help/personal_reports_3.jpg';

In Job Book, you can review the time cards and expenses you entered or those that were entered for you. 

## My Time Cards

<Screenshot image={img1} alt="My Time Cards - Navigate" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click **My Time Cards** in the **Personal Reports** card on the dashboard.

Enter a date range and click **Load Data**. Time cards falling within the date range will be displayed, showing the job number, DWR number, project name, line item, status, and hours. Total hours are summed up at the bottom of the report. 

<Screenshot image={img2} alt="Personal Reports - My Time Cards" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## My Expenses

Click **My Expenses** in the **Personal Reports** card on the dashboard.

Enter a date range and click **Load Data**.

<Screenshot image={img3} alt="Personal Reports - My Expenses" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```

## File: task-dashboard.mdx/task-dashboard.mdx
```
---
title: 'Task Dashboard'
description: 'A report of all relevant tasks.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import taskDashboardNav from '~/assets/images/help/task-dashboard/task-dashboard-nav.png';
import taskDashboard from '~/assets/images/help/task-dashboard/task-dashboard.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#overview">Overview</a>
        </li>
        <li>
            <a href="#accessing-the-task-dashboard">Accessing the Task Dashboard</a>
        </li>
        <li>
            <a href="#features">Features</a>
            <ul>
                <li><a href="#columns">Columns</a></li>
                <li><a href="#grid-operations">Grid Operations</a></li>
                <li><a href="#report-templating">Report Templating</a></li>
            </ul>
        </li>
    </ol>
</TableOfContents>

## Overview

The Task Dashboard is your central hub for keeping track of all important tasks. It gives you a clear, up-to-the-minute view of everything that needs attention. To keep things tidy, the dashboard only shows you the tasks that are currently relevant. This includes:

-   Any task that hasn't been marked as 'Completed'.
-   Tasks scheduled for a future date.
-   All tasks from a project ('Task Plan') that is still in progress.

## Accessing the Task Dashboard

You can get to the Task Dashboard right from your main dashboard. Just look for the 'Tasks / Scheduling' card and click on 'Task Dashboard'.

<Screenshot
  image={taskDashboardNav}
  alt="Task Dashboard Navigation"
  caption="Access the 'Task Dashboard' from the dashboard."
/>

After clicking, you'll be taken to the main Task Dashboard. It provides a comprehensive grid view of all your relevant tasks, allowing you to quickly see what's on your plate.

<Screenshot
  image={taskDashboard}
  alt="Task Dashboard"
  caption="The Task Dashboard provides a comprehensive overview of all relevant tasks."
/>

## Features

The Task Dashboard is designed to be flexible and powerful, giving you the information you need in the way you want to see it. Here’s a breakdown of what you can do:

### Understanding the Columns

The dashboard is organized into several columns to give you all the details you need at a glance:

-   **Related to**: This is the job number. You can click on it to jump directly to that job's page.
-   **Reference**: The name of the project the task is a part of.
-   **Client**: The client for the job.
-   **Project Manager**: The person in charge of the job.
-   **Task**: The name of the task. Clicking on this will take you to the detailed Task Plan.
-   **Scheduled**: The date the task is scheduled to begin.
-   **Time**: The specific start time for the task, if one has been set.
-   **End**: The date the task is scheduled to be completed.
-   **Status**: This tells you the current state of the task:
    -   **Not Started**: The task is waiting to be started.
    -   **In Progress**: The task is currently being worked on.
    -   **Completed**: The task is finished. The cell will be highlighted in green for easy identification.
    -   **Blocked**: A special status indicating that the task can't be started yet because other tasks it depends on are not complete.
-   **Task Due**: The deadline for the task.
-   **Overdue**: This will show 'Yes' if the task is past its due date but not yet completed. The cell will be highlighted in red to draw your attention.
-   **Assigned to**: The person responsible for completing the task.
-   **Office**: This column is hidden by default, but you can show it by clicking the three vertical dots icon in any column header and selecting it from the menu.

### Customizing Your View

The Task Dashboard is built on a powerful grid system that lets you customize the layout to fit your needs. You can:

-   **Export to Excel**: Click the button in the toolbar to download your current view as an Excel spreadsheet.
-   **Sort**: Click on any column header to sort the entire table by that column. Click again to reverse the sort order. You can also perform **multi-column sorting** by clicking on additional column headers. Each click will add or change the sort order for that column, and previous sorts will be maintained. For example, you can sort by 'Project Manager' first, and then by 'Task Due' date within each project manager's tasks. The order in which you click the headers determines the sorting priority.
-   **Show/Hide Columns**: Click the three vertical dots icon in the right-hand side of each column header to open the column menu, then choose which columns you want to see or hide.
-   **Filter**: The column menu also lets you filter the tasks based on specific criteria, so you can focus on what's most important.
-   **Group**: Drag a column header to the area above the table to group your tasks by that column.
-   **Reorder and Resize Columns**: Drag and drop the column headers to rearrange them, or drag the edge of a column to resize it.

### Saving and Applying Your Layouts (Report Templating)

The Task Dashboard supports Job Book's powerful **Report Templating** feature. This allows you to save your customized grid layouts and apply them later, saving you time and ensuring consistent reporting. This feature enhances the standard grid with extra controls in the grid toolbar.

**What can you save in a template?**

When you save a template, it captures the following aspects of your current Task Dashboard view:

-   **Visible columns**: Which columns are shown or hidden.
-   **Column widths**: The size of each column.
-   **Filters**: Any filters you've applied to narrow down your tasks.
-   **Sorting**: The primary and secondary sort orders applied to your data.
-   **Grouping**: How your tasks are grouped by specific columns.

**How to use Report Templating:**

1.  **Save a new template**: To save your current grid configuration as a new template:
    -   Click the 'Save As' button in the toolbar.
    -   Enter a descriptive name for your template.
    -   Click 'OK'.

2.  **Replace an existing template**: To update a previously saved template with your current grid configuration:
    -   Select the template you wish to update from the 'Select Template...' dropdown in the toolbar.
    -   Click the 'Save' button.
    -   Confirm your action by clicking 'OK' on the confirmation dialog.

3.  **Load a saved template**: To apply a saved template to your current view:
    -   Select the template you want to load from the 'Select Template...' dropdown.
    -   Click the 'Load' button.

4.  **Delete a saved template**: To remove a template you no longer need:
    -   Select the template from the 'Select Template...' dropdown.
    -   Click the 'Delete' button.
    -   Confirm your action by clicking 'OK' on the confirmation dialog.

5.  **Reset to default**: To clear all custom settings and return the grid to its original default configuration:
    -   Click the 'Reset' button in the toolbar.

This feature is incredibly useful for frequently used reports, offering a convenient way to save your personalized views for quick access. Your templates are stored securely in your browser for your individual use.


<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/tasks-and-scheduling-overview">Tasks and Scheduling: Overview</a></li>
        <li><a href="/help/task-templates">Task Templates</a></li>
        <li><a href="/help/task-plans">Task Plans</a></li>
        <li><a href="/help/task-scheduling">Task Scheduling</a></li>
        <li><a href="/help/personal-task-management">Personal Task Management</a></li>
        <li>Task Dashboard</li>
    </ol>
</TableOfContents>
```

## File: task-plans.mdx/task-plans.mdx
```
---
title: 'Task Plans'
description: 'Learn how to use Task Plans to manage the tasks for a specific job.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import imgNav from '~/assets/images/help/task-plans/task-plan-nav.png';
import imgManage from '~/assets/images/help/task-plans/task-plan-manage.png';

<TableOfContents>
    <ol>
        <li><a href="#key-concepts">Key Concepts</a></li>
        <li><a href="#navigating-to-a-jobs-task-plan">Navigating to a Job's Task Plan</a></li>
        <li><a href="#importing-task-templates">Importing Task Templates</a></li>
        <li><a href="#task-status">Task Status</a></li>
        <li><a href="#task-due-date">Task Due Date</a></li>
        <li><a href="#assigning-tasks">Assigning Tasks</a></li>
        <li><a href="#scheduled-tasks">Scheduled Tasks</a></li>
        <li><a href="#adding-and-organizing-tasks">Adding and Organizing Tasks</a></li>
    </ol>
</TableOfContents>

## Key Concepts

A **Task Plan** is a detailed, organized breakdown of all the work required to complete a specific Job. Think of it as a comprehensive to-do list for your project, allowing you to manage every step from start to finish.

Here are the core ideas behind a Task Plan:

*   **Job-Specific:** Each Job has its own unique Task Plan, tailored to its specific requirements.
*   **Hierarchical Tasks:** You can break down large tasks into smaller, more manageable sub-tasks. This helps you organize complex work into clear, actionable steps. For example, a main task like "Field Work" might have sub-tasks such as "Set Control Points" and "Collect Topo Data."
*   **Dependencies:** You can link tasks together to ensure work is completed in the correct order. For tasks that are not schedulable, the system will automatically make them available only after the tasks they depend on are finished. However, if a task is already scheduled to an employee, they can begin working on it regardless of its dependencies.
*   **Schedulable Tasks:** When you mark a task as "schedulable," you are bundling it and all of its sub-tasks together. This entire bundle can then be scheduled on the project calendar as a single, continuous block of work.

## Navigating to a Job's Task Plan

Every Job in the system can have its own unique Task Plan. To access it, first navigate to the desired Job. From the Job's main display page, click on the **Manage Task Plan** button.

<Screenshot image={imgNav} alt="Task Plan Navigation" caption="Task Plan Navigation" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

This will take you to the **Task Plan Editor** for that Job, where you can build and manage the job's tasks.

<Screenshot image={imgManage} alt="Task Plan Management" caption="Task Plan Management" classes={{containerContainer:"mb-6", imageClass:"rounded border"}} />

## Importing Task Templates

You can import one or more Task Templates into your Task Plan to quickly add pre-defined sets of tasks.

1.  Select a **Task Template** from the dropdown list.
2.  Optionally, select a task in the plan that will become the main task for the imported tasks.
3.  Click the **Import Template** button.

If you don't select a main task, the template's tasks will be added to the top level of your plan. If you do select a main task, the new tasks will be added as its sub-tasks. This is useful when a single job requires performing the same set of actions at multiple locations.

For example, imagine a job requires you to perform a topographic survey on two separate parcels of land. You could create two main tasks: "Topo for Parcel A" and "Topo for Parcel B". Then, for each of these main tasks, you can import your standard "Topographic Survey" template. This ensures you follow the exact same procedure for both locations while keeping the work for each parcel neatly organized within the same job.

## Task Status

The status of a task helps you track its progress. There are three possible statuses:

*   **Not Started:** The task has not yet begun.
*   **In Progress:** The task is currently being worked on.
*   **Completed:** The task is finished.

You can change a task's status by double-clicking the **Status** cell for that task in the editor.

**Important Notes:**

*   You can only change the status of tasks that do not have any sub-tasks. The status of a main task, on the other hand, is determined by the status of its sub-tasks. Think of it like a summary: the main task is only complete when all of its sub-tasks are complete. If even one sub-task is still in progress, the main task will also show as in progress.
*   Completed tasks are highlighted in green for easy identification.

## Task Due Date

You can set a **Due Date** for any task. This date is for informational and planning purposes and does not affect the schedule. It is displayed in other parts of the system, like the Scheduler and Task Dashboard, to help with coordination.

To set or change a due date, double-click the **Due** cell for the task and choose a date from the calendar.

If a sub-task's due date is set for after its main task's due date, it will be highlighted in red to indicate a potential planning problem.

## Assigning Tasks

To assign a task to one or more employees, simply double-click the **Assigned To** cell for that task. A list of available employees will appear, allowing you to select who is responsible.

**Important Notes:**

*   You can only assign tasks that are not marked as "schedulable." If a task is scheduled, its assignment is managed from the **Scheduler**, not the Task Plan.
*   To ensure clarity on the field, only one task within a group of a main task and its sub-tasks can have a direct assignment. For example, if you assign the main task "Field Work" to a specific crew, all of its sub-tasks (like "Set Control Points" and "Locate Monuments") will automatically be assigned to that same crew. You cannot assign a sub-task to a different crew than its main task.

## Scheduled Tasks

When a task is scheduled in the **Scheduler**, a calendar icon will appear next to it in the Gantt chart view. If you hover over this icon, a dialog will appear showing details like the scheduled date and any notes.

If a task has **Schedule Notes** added from the Scheduler, a message icon will also appear. Hovering over this will show the notes.

## Adding and Organizing Tasks

You have several tools to build and structure your Task Plan:

*   **Add a task:**
    *   To add a new top-level task, simply click the **+ Add Task** button when no other tasks are selected.
    *   If you have an existing task selected, clicking the **+ Add Task** button will open a menu:
        *   **Add Above:** Adds a new task on the same level, directly above the selected task.
        *   **Add Below:** Adds a new task on the same level, directly below the selected task.
*   **Create a sub-task:**
    1.  Select the task that will be the main task.
    2.  Click the **+ Add Task** button.
    3.  Select **Add Sub-task** from the menu.
    *Alternatively, you can drag and drop an existing task onto another to make it a sub-task.*
*   **Create dependencies between tasks:**
    1.  First, select the tasks you want to link. You can select multiple tasks in a few ways:
        *   **Drag-select:** Click and drag your mouse to draw a selection box around the tasks.
        *   **Ctrl-click:** Hold the `Ctrl` key and click on each individual task you want to select.
        *   **Shift-click:** Click the first task in a sequence, then hold the `Shift` key and click the last task to select all tasks in between.
    2.  Click the **Link** button.
    *   If you selected two tasks, a dependency is created between them.
    *   If you selected more than two tasks, they are linked in sequence (Task 1 -> Task 2 -> Task 3).
*   **Remove a dependency:**
    1.  Select the link between two tasks.
    2.  Click the **Delete Link** button.
*   **Make a task schedulable:**
    1.  Select the task.
    2.  Click the **Toggle Schedulable** button. This bundles the task and its sub-tasks to be scheduled as a single unit.
*   **Delete a task:**
    1.  Select the task.
    2.  Click the **Delete Task** button. This will also delete all of its sub-tasks.
*   **Rename a task:** Double-click the **Task** cell, edit the text, and press `Enter`.
*   **Add a description:** Double-click the **Description** cell, add your text, and press `Enter`.


<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/tasks-and-scheduling-overview">Tasks and Scheduling: Overview</a></li>
        <li><a href="/help/task-templates">Task Templates</a></li>
        <li>Task Plans</li>
        <li><a href="/help/task-scheduling">Task Scheduling</a></li>
        <li><a href="/help/personal-task-management">Personal Task Management</a></li>
        <li><a href="/help/task-dashboard">Task Dashboard</a></li>
    </ol>
</TableOfContents>
```

## File: task-scheduling.mdx/task-scheduling.mdx
```
---
title: 'Task Scheduling'
description: 'Learn how to schedule tasks, assign them to employees, and manage your team’s workload.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import scheduler from '~/assets/images/help/scheduler/scheduler.png';
import schedulerNav from '~/assets/images/help/scheduler/scheduler-nav.png';


import schedulerTaskDetail from '~/assets/images/help/scheduler/scheduler-task-detail.png';
import schedulerMonth from '~/assets/images/help/scheduler/scheduler-month.png';
import schedulerEmployeeFilter from '~/assets/images/help/scheduler/scheduler-employee-filter.png';
import schedulingIntegrationImg from '~/assets/images/leave-tracking-scheduling-integration.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#key-concepts">Key Concepts</a>
        </li>
        <li>
            <a href="#navigating-to-the-task-scheduler">Navigating to the Task Scheduler</a>
        </li>
        <li>
            <a href="#understanding-the-layout">Understanding the Layout</a>
        </li>
        <li>
            <a href="#scheduling-a-task">Scheduling a Task</a>
        </li>
        <li>
            <a href="#modifying-a-scheduled-task">Modifying a Scheduled Task</a>
        </li>
        <li>
            <a href="#editing-task-details">Editing Task Details</a>
        </li>
        <li>
            <a href="#leave-tracking-integration">Leave Tracking Integration</a>
        </li>
        <li>
            <a href="#filtering-the-calendar">Filtering the Calendar</a>
        </li>
    </ol>
</TableOfContents>

## Key Concepts

The Task Scheduler is your central hub for assigning and managing your team’s workload. It provides a visual overview of all schedulable tasks and your team’s availability, allowing you to plan and allocate work efficiently.

You can move tasks from the Unscheduled Tasks grid onto the calendar to schedule them, and then adjust dates and assignments by dragging and dropping tasks directly on the calendar.



### Navigating to the Task Scheduler

You can access the scheduler directly from your main dashboard.

1.  From the dashboard, find the **Tasks / Scheduling** card.
2.  Click the **Task Scheduler** link to open the scheduling view.

<Screenshot image={schedulerNav} alt="Navigating to the Task Scheduler" caption="Navigating to the Task Scheduler" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Understanding the Layout

The Task Scheduler is composed of two primary components: the Unscheduled Tasks grid at the top and the Schedule Calendar below it.

*   **Unscheduled Tasks Grid**: A list of all tasks that are ready to be scheduled but have not yet been assigned a date or team member.
*   **Schedule Calendar**: A calendar view that displays scheduled tasks for each employee, giving you a clear picture of who is working on what and when.

#### The Unscheduled Tasks Grid

This grid lists all tasks from your projects that have been marked as "schedulable" but haven't been placed on the calendar yet.

<Screenshot image={scheduler} alt="Unscheduled Tasks Grid" caption="The Unscheduled Tasks Grid" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

The grid provides the following information:

*   **Client**: The client associated with the task's project.
*   **Related to**: A clickable link to the project, identified by its Job Number.
*   **Reference**: The Project Name for quick identification.
*   **Ordered**: The date the project was ordered.
*   **Due**: The project's overall due date.
*   **Task Due**: The specific due date for the task, if one was set in the [Task Plan](/help/task-plans).

You can sort the list by clicking on any column header or filter it by clicking the filter icon in the header.

When you click the filter icon, a menu will appear with options to help you narrow down the list. You can type in a value to search for, and the grid will show only the tasks that match. The filter menu also provides a list of operators to help you refine your search, such as "Contains," "Starts with," and "Is equal to."

#### The Schedule Calendar

The calendar displays all the tasks that have been scheduled for your team. By default, it opens in a weekly view, with each team member having their own row showing their assigned tasks for the week.

<Screenshot image={scheduler} alt="Schedule Calendar" caption="The Schedule Calendar" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

You can navigate the calendar using the following controls:

*   **Forward/Backward**: Use the **&lt;** and **&gt;** buttons to move one week or month at a time.
*   **Change View**: Switch between **Week** and **Month** views by clicking the corresponding button.

<Screenshot image={schedulerMonth} alt="Scheduler Month View" caption="The Schedule Calendar (Month View)" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
*   **Go to Today**: Click the **Today** button to jump back to the current date.
*   **Select a Date**: Click the calendar icon to open a date picker and select a specific date to view.

Tasks on the calendar are color-coded to indicate their status:

*   **Not Started**: Blue
*   **In Progress**: Orange
*   **Completed**: Green

### Scheduling a Task

To schedule a task, you simply drag it from the Unscheduled Tasks grid and drop it onto the calendar.

1.  Find the task you want to schedule in the **Unscheduled Tasks** grid.
2.  Click and hold the task's row.
3.  Drag the task down to the **Schedule Calendar**.
4.  Drop the task on the desired date in the row of the employee you want to assign it to.

- *Note: Scheduling by dragging and dropping only works when the calendar is in the **Week** view.*

### Modifying a Scheduled Task

Once a task is on the calendar, you can easily adjust its schedule or assignment.

*   **Reschedule or Reassign**: In the **Week** view, drag and drop the task to a new date or a different employee's row.
*   **Reschedule in Month View**: In the **Month** view, you can drag and drop a task to a different day.
*   **Adjust Task Duration**: To change the length of a task, hover over its start or end edge until the cursor changes, then click and drag to extend or shorten it.

    *Note: In the week view, it is not possible to extend a task beyond the current week. To do this, use the [Scheduled Task Details panel](#editing-task-details).*
*   **Unschedule a Task**: Hover over the task to reveal an **x** button in the corner. Click the **x** and confirm to remove the task from the calendar and return it to the Unscheduled Tasks grid.

### Editing Task Details

For more detailed changes, you can open the task details panel.

1.  Double-click any scheduled task on the calendar.
2.  The **Scheduled Task Details** panel will appear.

<Screenshot image={schedulerTaskDetail} alt="Scheduled Task Details Panel" caption="Scheduled Task Details Panel" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

From this panel, you can:

*   View a summary of the task, including the project number, client, and task name.
*   Adjust the **Start Date** and **End Date**.
*   Set a specific **Start Time** to control the order of tasks on a given day.
*   Add **Schedule Notes** that will be visible to the assigned employee on their personal schedule.
*   **Unschedule** the task by clicking the "Unschedule Task" button.

Click **Save** to apply your changes or **Cancel** to discard them.

### Leave Tracking Integration

To help you avoid scheduling conflicts, the calendar is fully integrated with the [Leave Tracking module](/leave-tracking). When an employee’s time off is approved, it automatically appears as a blocked-out period on the schedule.

This gives you a complete picture of your team’s availability, ensuring you don’t accidentally assign work to someone who is on vacation.

<Screenshot image={schedulingIntegrationImg} alt="Leave shown in the Task & Crew Scheduler" caption="Approved leave appears directly in the scheduler to prevent conflicts." classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Filtering the Calendar

To help you focus on specific team members, both the week and month views can be filtered by clicking the 'Employee Filter' multi-select field. This allows you to narrow down the calendar view in several ways:

*   **By Employee**: Select one or more individual employees to see only their schedules.
*   **By Office**: Offices are listed at the top of the filter and are identified by an 'office' icon. Selecting an office will show schedules for all employees assigned to that location.
*   **By Employee Group**: Below the offices, you can select predefined Employee Groups, which are marked with a 'group' icon. This is useful for viewing the combined schedule for a specific crew or team.

Employee groups allow you to quickly select multiple employees at once. For example, you might create groups for "Crew 1" or "Office Staff." To manage your employee groups, go to the **Settings** panel (found in the top-right of the screen), select **Groups**, and then you can create new groups or modify existing ones by adding or removing employees.

<Screenshot image={schedulerEmployeeFilter} alt="Filtering the Calendar" caption="Filtering the Calendar" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />


<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/tasks-and-scheduling-overview">Tasks and Scheduling: Overview</a></li>
        <li><a href="/help/task-templates">Task Templates</a></li>
        <li><a href="/help/task-plans">Task Plans</a></li>
        <li>Task Scheduling</li>
        <li><a href="/help/personal-task-management">Personal Task Management</a></li>
        <li><a href="/help/task-dashboard">Task Dashboard</a></li>
    </ol>
</TableOfContents>
```

## File: task-templates.mdx/task-templates.mdx
```
---
title: 'Task Templates'
description: 'Learn how to use Task Templates to streamline your project setup and ensure consistency across all of your jobs.'
layout: '~/layouts/HelpLayout.astro'
---

import Screenshot from '~/components/ui/Screenshot.astro';
import TableOfContents from '~/components/ui/TableOfContents.astro';

import imgNav from '~/assets/images/help/task-template/task-template-nav.png';
import imgExplore from '~/assets/images/help/task-template/task-template-explore.png';
import imgEdit from '~/assets/images/help/task-template/task-template-edit.png';
import imgDisplay from '~/assets/images/help/task-template/task-template-display.png';

<TableOfContents>
    <ol>
        <li>
            <a href="#key-concepts">Key Concepts</a>
        </li>
        <li>
            <a href="#exploring-task-templates">Exploring Task Templates</a>
        </li>
        <li>
            <a href="#viewing-a-task-template">Viewing a Task Template</a>
        </li>
        <li>
            <a href="#editing-a-task-template">Editing a Task Template</a>
        </li>
        <li>
            <a href="#adding-and-organizing-tasks">Adding and Organizing Tasks</a>
        </li>
    </ol>
</TableOfContents>

## Key Concepts

Task Templates are a powerful feature in Job Book that allow you to create reusable sets of tasks for your projects. This saves you time and ensures consistency across all of your jobs.

*   **Hierarchical Tasks:** You can break down large tasks into smaller, more manageable sub-tasks. Think of this like a to-do list where a main item has several steps. For example, 'Field Work' is a main task, and all the items below it are its sub-tasks. This makes complex work easier to track. When all the sub-tasks are finished, the main task is considered complete.
*   **Dependencies:** You can link tasks together to ensure work is completed in the correct order. For tasks that are not schedulable, the system will automatically make them available only after the tasks they depend on are finished. However, if a task is already scheduled to an employee, they can begin working on it regardless of its dependencies.
*   **Schedulable Tasks:** When you mark a task as "schedulable," you are bundling it and all of its sub-tasks together. This entire bundle can then be scheduled on the project calendar as a single, continuous block of work.
*   **Active Status:** The "Active" checkbox determines whether the entire template is available for use in new projects.

## Exploring Task Templates

You can find your library of Task Templates by navigating to **Tasks / Scheduling > Explore Task Templates** from the main dashboard.

<Screenshot image={imgNav} alt="Task Template Navigation" caption="Task Template Navigation" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

This will take you to the **Explore Task Templates** page, where you can see a list of all available templates. From here, you can create a new template from scratch or click on an existing template to view its details.

<Screenshot image={imgExplore} alt="Task Template Exploration" caption="Task Template Exploration" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

## Viewing a Task Template

After clicking on a template from the Explore page, you will see the **Task Template Display** screen. This view is read-only, allowing you to safely review the template's structure and tasks without making accidental changes.

<Screenshot image={imgDisplay} alt="Task Template Display" caption="Task Template Display" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

From this screen, you have two options:

*   **Clone:** This creates a complete copy of the current template. You will be prompted to provide a new name for the cloned template, which you can then edit independently.
*   **Edit:** This will take you to the **Task Template Editor**, where you can modify the template's name, tasks, and dependencies.

## Editing a Task Template

To modify a template, click the **Edit** button on the **Task Template Display** screen. This will take you to the **Task Template Editor**, where you can make changes to a template. This powerful tool allows you to build complex task hierarchies with dependencies.

<Screenshot image={imgEdit} alt="Task Template Editor" caption="Task Template Editor" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

### Adding and Organizing Tasks

*   **Add a task:**
    *   To add the first task to a new template, simply click the **+ Add Task** button.
    *   If you have an existing task selected, clicking the **+ Add Task** button will open a menu:
        *   **Add Above:** Adds a new task on the same level, directly above the selected task.
        *   **Add Below:** Adds a new task on the same level, directly below the selected task.
*   **Create a sub-task:**
    1.  Select a task to be the parent task.
    2.  Click the **+ Add Task** button.
    3.  Select 'Add Child' from the menu.
    *Alternatively, you can drag and drop an existing task onto another to make it a sub-task.*
*   **Create dependencies between tasks:**
    1.  First, select the tasks you want to link. You can select multiple tasks in a few ways:
        *   **Drag-select:** Click and drag your mouse to draw a selection box around the tasks.
        *   **Ctrl-click:** Hold the `Ctrl` key and click on each individual task you want to select.
        *   **Shift-click:** Click the first task in a sequence, then hold the `Shift` key and click the last task to select all tasks in between.
    2.  Click the **Link** button.
    *   If you selected two tasks, a dependency is created between them.
    *   If you selected more than two tasks, they are linked in sequence (Task 1 -> Task 2 -> Task 3).
*   **Remove a dependency:**
    1.  Select the link between two tasks.
    2.  Click the **Delete Link** button.
*   **Make a task schedulable:**
    1.  Select the task.
    2.  Click the **Toggle Schedulable** button.
*   **Delete a task:**
    1.  Select the task.
    2.  Click the **Delete Task** button.


<TableOfContents title="Related Guides">
    <ol>
        <li><a href="/help/tasks-and-scheduling-overview">Tasks and Scheduling: Overview</a></li>
        <li>Task Templates</li>
        <li><a href="/help/task-plans">Task Plans</a></li>
        <li><a href="/help/task-scheduling">Task Scheduling</a></li>
        <li><a href="/help/personal-task-management">Personal Task Management</a></li>
        <li><a href="/help/task-dashboard">Task Dashboard</a></li>
    </ol>
</TableOfContents>
```

## File: tasks-and-scheduling-overview.mdx/tasks-and-scheduling-overview.mdx
```
---
title: 'Tasks and Scheduling: Overview'
description: 'An overview of the Tasks and Scheduling module in Job Book.'
layout: '~/layouts/HelpLayout.astro'
---

import TableOfContents from '~/components/ui/TableOfContents.astro';

<TableOfContents>
    <ol>
        <li>
            <a href="#introduction">Introduction</a>
        </li>
        <li>
            <a href="#key-concepts">Key Concepts</a>
            <ul>
                <li><a href="#task-templates">Task Templates</a></li>
                <li><a href="#task-plans">Task Plans</a></li>
                <li><a href="#task-scheduling">Task Scheduling</a></li>
                <li><a href="#personal-task-management">Personal Task Management</a></li>
            </ul>
        </li>
        <li>
            <a href="#how-it-fits-together">How It All Fits Together</a>
        </li>
    </ol>
</TableOfContents>

## Introduction

Welcome to the Tasks and Scheduling module! This set of tools is designed to help you and your team manage your work from start to finish. It allows you to standardize your processes, plan your projects, schedule work for your crews, and keep track of your own tasks. This helps everyone know what they need to do and when, reducing confusion and making sure work gets done efficiently.

## Key Concepts

Here are the main ideas you'll need to know to get started.

### Task Templates

Think of Task Templates as reusable checklists for your common jobs. If you do the same kind of work over and over, you can create a template with all the steps involved. This saves you from having to create the same list of tasks every time you start a new job. It also helps ensure that every job is done consistently and no steps are missed.

### Task Plans

A Task Plan is where you take a Task Template and apply it to a specific job. Once you've added a template to a job, you can customize it as needed, set due dates, and assign tasks to different people. You can also link tasks together, so that when one task is finished, the next one is automatically handed off to the right person.

### Task Scheduling

Task Scheduling is how you take tasks from your Task Plan and put them on a calendar. This is especially useful for work that needs to be done by a field crew on a specific day. You can see who is available, drag and drop tasks onto their schedule, and make sure everyone knows where they need to be and when.

### Personal Task Management

This is your personal to-do list. It shows you all the tasks that have been assigned to you, both scheduled and unscheduled. You can see what you need to work on, update the status of your tasks as you complete them, and keep track of your workload for the week.

## How It All Fits Together

Here’s a simple way to think about how these pieces work together:

1.  You start by creating **Task Templates** for the different types of work you do.
2.  When you get a new job, you create a **Task Plan** for it, using one of your templates as a starting point. You assign the tasks to your team.
3.  For tasks that need to be done on a specific day, you use **Task Scheduling** to put them on the calendar for your crews.
4.  Each team member then uses their **Personal Task Management** screen to see what they need to do, whether it's a scheduled task for the day or an office task they can work on when they have time.

By using these tools together, you can create a smooth workflow for your entire team, from the office to the field.

<TableOfContents title="Related Guides">
    <ol>
        <li>Tasks and Scheduling: Overview</li>
        <li><a href="/help/task-templates">Task Templates</a></li>
        <li><a href="/help/task-plans">Task Plans</a></li>
        <li><a href="/help/task-scheduling">Task Scheduling</a></li>
        <li><a href="/help/personal-task-management">Personal Task Management</a></li>
        <li><a href="/help/task-dashboard">Task Dashboard</a></li>
    </ol>
</TableOfContents>
```

## File: Users_and_Employee_Profiles.mdx/Users_and_Employee_Profiles.mdx
```
---
title: 'Users and Employee Profiles'
description: 'A comprehensive guide on managing user and employee profiles within Job Book. Learn about user roles, adding users, setting roles, and employee onboarding.'
layout: '~/layouts/HelpLayout.astro'
---
import TableOfContents from '~/components/ui/TableOfContents.astro';
import Screenshot from '~/components/ui/Screenshot.astro';

import img1 from '~/assets/images/help/Users_employees_1.jpg';
import img2 from '~/assets/images/help/Users_employees_2.jpg';
import img3 from '~/assets/images/help/Users_employees_3.jpg';
import img4 from '~/assets/images/help/Users_employees_4.png';
import img8 from '~/assets/images/help/Users_employees_8.jpg';
import img9 from '~/assets/images/help/Users_employees_9.jpg';
import img10 from '~/assets/images/help/Users_employees_10.jpg';

<TableOfContents>
    <ol>
        <li>
            <a href="#users">Users</a>
        </li>
        <li>
            <a href="#user-roles">User Roles</a>
            <ol>
                <li><a href="#technician">Technician</a></li>
                <li><a href="#job-coordinator">Job Coordinator</a></li>
                <li><a href="#manager">Manager</a></li>
                <li><a href="#administrator">Administrator</a></li>
                <li><a href="#view">View</a></li>
                <li><a href="#modify--create--delete">Modify / Create / Delete</a></li>
                <li><a href="#report-access">Report Access</a></li>
                <li><a href="#tasks--scheduling-if-scheduling-module-enabled">Tasks / Scheduling</a></li>
                <li><a href="#leave-requests-if-module-enabled">Leave Requests</a></li>
            </ol>
        </li>
        <li>
            <a href="#adding-users-and-setting-roles">Adding Users and Setting Roles</a>
        </li>
        <li>
            <a href="#new-user-login">New User Login</a>
        </li>
        <li>
            <a href="#employees">Employees</a>
        </li>
        <li>
            <a href="#employees">Adding Employees</a>
        </li>
    </ol>
</TableOfContents>

## Users

Users are able to log in to Job Book with an email and a password.

## User Roles

Users are assigned roles that control what they can see and do in the system.

### <a id="technician"></a>Technician

This role is for staff who will be entering timesheets (Daily Work Records), expenses and safety forms into the system. Technicians do not have access to any financial information, and can generally only see records that they entered themselves.

### <a id="job-coordinator"></a>Job Coordinator

This role is similar to the Technician, but with additional permissions to update Jobs and Clients. The Job Coordinators role is ideal for users who need to coordinate and update job information without the broader privileges granted to Managers.

### <a id="manager"></a>Manager

This role allows users to perform Technician tasks, in addition to a number of management duties such as approvals and invoicing. Managers have access to financial information, and can generally see records across the whole system.

### <a id="administrator"></a>Administrator

This role allows access to everything in the system, including the creation and modification of Clients, Jobs, Rate Sheets and line items. Administrators can also create and delete users, and set user roles.

## View

| | Technician | Job Coordinator | Manager | Administrator |
| --- | --- | --- | --- | --- |
| **Navigate** | | | | |
| Clients | | ✔ | ✔ | ✔ |
| Equipment and Materials | ✔ | ✔ | ✔ | ✔ |
| Expense Items | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |
| Jobs | ✔ | ✔ | ✔ | ✔ |
| Labour Cost Items | ✔ | ✔ | ✔ | ✔ |
| Fixed Price Items | ✔ | ✔ | ✔ | ✔ |
| Offices | ✔ | ✔ | ✔ | ✔ |
| Training Courses | | ✔ | ✔ | ✔ |
| Vehicles | ✔ | ✔ | ✔ | ✔ |
| Rate Sheets | | ✔ | ✔ | ✔ |
| Expenses | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |
| DWRs | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |
| Invoices | | ✔ | ✔ | ✔ |
| Safety | ✔ (Their own) | | ✔ | ✔ |
| **Settings** | | | | |
| Users | | | | ✔ |
| Roles | | | | ✔ |
| Employee Profiles | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |

## Modify / Create / Delete

| | Technician | Job Coordinator | Manager | Administrator |
| --- | --- | --- | --- | --- |
| **Navigate** | | | | |
| Clients | | ✔ | | ✔ |
| Equipment and Materials | | | | ✔ |
| Expense Items | | | | ✔ |
| Jobs | | ✔ | ✔ | ✔ |
| Labour Cost Items | | | | ✔ |
| Fixed Price Items | | | | ✔ |
| Offices | | | | ✔ |
| Training Courses | | | | ✔ |
| Vehicles | | | | ✔ |
| Rate Sheets | | | | ✔ |
| Expenses | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |
| DWRs | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |
| Invoices | | | ✔ | ✔ |
| Safety | ✔ (Their own) | | ✔ | ✔ |
| **Settings** | | | | |
| Users | | | | ✔ |
| Roles | | | | ✔ |
| Employee Profiles | ✔ (Their own) | ✔ (Their own) | ✔ | ✔ |

## Report Access

| | Technician | Job Coordinator | Manager | Administrator |
| --- | --- | --- | --- | --- |
| **Reports** | | | | |
| Active Job Dashboard | | ✔ | ✔ | ✔ |
| Expense Report | | | ✔ | ✔ |
| Line Item Report | | | ✔ | ✔ |
| My Expenses | ✔ | ✔ | ✔ | ✔ |
| My Time Cards | ✔ | ✔ | ✔ | ✔ |
| Time Card Report | | | ✔ | ✔ |
| Time Grid | | | ✔ | ✔ |
| Utilization Report | | | ✔ | ✔ |
| WIP Report | | | ✔ | ✔ |
| Job Maps | | ✔ | ✔ | ✔ |
| **Workflow** | | | | |
| DWR Approval Backlog | | | ✔ | ✔ |
| DWR Invoice Backlog | | | ✔ | ✔ |
| Expense Approval Backlog | | | ✔ | ✔ |
| Invoice Process Backlog | | | ✔ | ✔ |

## Tasks / Scheduling (if [Scheduling module](/task-crew-scheduling) enabled)

| | Technician | Job Coordinator | Manager | Administrator |
| --- | --- | --- | --- | --- |
| **Navigate** | | | | |
| Task Plans | | | ✔ | ✔ |
| Task Templates | | | ✔ | ✔ |
| **Reports and Utilities** | | | | |
| Task Dashboard | | | ✔ | ✔ |
| Task Scheduler | | | ✔ | ✔ |
| My Schedule | ✔ | ✔ | ✔ | ✔ |
| My Unscheduled Tasks | ✔ | ✔ | ✔ | ✔ |

## Leave Requests (if module enabled)

| | Technician | Job Coordinator | Manager | Administrator |
| --- | --- | --- | --- | --- |
| **Navigate** | | | | |
| Leave Requests | | | ✔ | ✔ |
| **Reports and Utilities** | | | | |
| Company Calendar | ✔ | ✔ | ✔ | ✔ |
| Leave Request Report | | | ✔ | ✔ |

## Adding Users and Setting Roles

Click **Settings**, then click **Users**.

<Screenshot image={img1} alt="Adding users and setting roles - click Settings" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

<Screenshot image={img2} alt="Adding users and setting roles - click Users" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

On the **User Administration** page, users can review the user list and **Create** a new user. 

<Screenshot image={img3} alt="Adding users and setting roles - create new User" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

On the Create User page enter the new user's name and email, then assign the appropriate role. 

<Screenshot image={img4} alt="Adding users and setting roles - set user name, email and roles" classes={{containerClass:"mb-6 w-2/3 mx-auto", imageClass:"rounded border"}} />

## New User Login

After creating a new user, an email will be sent to that user with a link to login for the first time and set their password.

This process is described from the user's point-of-view in [Site Staff Initial Setup](/help/Site_Staff_Initial_Setup).

## Employees

Employees represent people who can be selected in line items in timesheets (DWRs) and other parts of Job Book.

Employees can be linked to Users for those who use the system to enter time sheets for themselves. Employees do not need to be linked to Users for those who do not use the system, but when their hours are entered by someone else (e.x., by a party chief, etc).

Note: if a User logs into Job Book and is not linked to an Employee, a warning will show up on their dashboard to contact their administrator. A User without an Employee will be unable to perform a number of tasks in the system. 

## Adding Employees

Click **Settings**.

<Screenshot image={img1} alt="Adding users and setting roles - click Settings" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Then, click **Employee Profiles**.

<Screenshot image={img8} alt="Adding users and setting roles - click Employee Profiles" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Click "Create" to create a new Employee. 

<Screenshot image={img9} alt="Adding users and setting roles - create new Employee" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />

Enter the employee name, the User who is linked to this Employee, and the employee code (if applicable).

If Active is checked, this Employee can be selected when entering a DWR. 

<Screenshot image={img10} alt="Adding users and setting roles - set Employee name, user, and code" classes={{containerClass:"mb-6", imageClass:"rounded border"}} />
```
