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

# Files

## File: 2.1_Intro_Transcript.txt/2.1_Intro_Transcript.txt
```
Welcome to the Job Book How to Use Series.

In this series, I’ll show you step by step how to use Cyanic Job Book in your day-to-day operations.

This series is for staff who use Job Book in their daily work. 

Job Book is a project management and job costing system designed for engineering and land surveying companies, but can be used by any field service company.

In this How to Use Series, we will build on what we did previously in the Job Book Setup Series. 

We’ll be using Offices, Line Items, Rate Sheets, and Employees that were set up in the previous series. 
Make sure you’ve completed the Setup Series before starting here.

This How to Use Series focuses on the core daily workflows, including:
Creating Clients and Jobs.
Recording Daily Work Records, DWRs.
Submitting expenses for reimbursement.
Monitoring progress with the Active Job Dashboard.
Approving DWRs and expenses through the backlog process.
Converting DWRs into invoices, or creating invoices from scratch.
Importing invoices into your accounting system

Each video is short and focused. You can watch the entire series to learn the full lifecycle of a job, or jump into the video you need when learning a specific task.

By the end of this series, you’ll be confident managing your daily work in Job Book, no matter your role.

For advanced reporting features, watch our Job Book Reporting Guide Series. 
You’ll find the link in the description below.

In the next video, we’ll cover navigation and the Job Book dashboard, so you’ll always know where to find what you need.

In future videos, we’ll dive into creating clients, setting up jobs, recording DWRs, and much more.

Thanks for watching, and let’s get started.
```

## File: 2.10_DWR Invoice_Backlog_Transcript.txt/2.10_DWR Invoice_Backlog_Transcript.txt
```
Welcome back to the Job Book How to Use Series. 
If this is your first time watching, 
remember that each episode builds on the last.

In the previous video, we cleared the Expense Approval Backlog so
reimbursements and job costs stayed accurate. Those approved expenses now wait
alongside labour in the billing pipeline.

Today, we’ll focus on invoicing the client. 
In Job Book, there are two types of invoices.
Fixed price invoices, where the client is charged a fixed amount for the service.
And time-and-materials invoices, where the client is charged 
based on the actual time spent and materials used during the project.

Time-and-materials invoices are labour intensive to create 
because they require careful tracking of all hours worked 
and materials used during the project. Missing Daily Work Records on an invoice 
means lost revenue and delays cash flow.

Thankfully, Job Book simplifies the invoicing process 
by automatically collecting all approved DWRs 
for jobs set to Time and Materials.
So it's easy to generate draft Invoices 
for final approval from a Project Manager.
To do this we will use the DWR Invoice Backlog. 
And in this video we will focus on the DWR Invoice Backlog. 
Getting this step right keeps billing accurate, 
clients confident, and cash flow predictable.

Why does the DWR Invoice Backlog matter? 
Every approved DWR represents work your team has already delivered.
Until you convert that work into an invoice,
revenue sits in limbo. This backlog is the last review before totals, rates,
and descriptions reach a client. Skipping it risks underbilling, double
billing, or sending the wrong detail trail to accounting.

I’m logged in as an Administrator. 
Typically, an Administrator converts DWRs for Time and Material jobs 
into draft invoices for Project Managers to review and approve.

From the main dashboard, look at the Workflow card 
in the middle of the second row. 
This is where billing queues live for administrators.

-- Click DWR Invoice Backlog --
The DWR Invoice Backlog is the time-and-materials 
invoice creation center for Job Book.

The grid lists every approved DWR that belongs to a time-and-material job 
that has not yet been invoiced. 

If you've watched our DWR Approval Backlog video earlier in this series.
All of this will look very familiar, 
and it behaves almost exactly the same.

At the top left, you’ll see the Invoice Selected DWRs button.
It will stay inactive until we have at least one DWR checked.
At the top right, you’ll see the Expand All, Collapse All buttons

Below that is the grouping bar. 
You can drag column headers here 
to group jobs by Job Number, Project Manager, or other fields.

Below that is the DWR Table, 
which shows all DWRs in the system that have not yet been invoiced.

The first column is a checkbox. 
Clicking the checkbox in the header selects all DWRs for bulk invoice generation. 
Unchecking it clears all selections.

Next are the Date, Created By, and DWR Number columns. 
The DWR Number column contains hyperlinks to the individual DWRs.

Then you have the Job Number, Client, Project Manager, and Office columns.

Sorting and filtering is done just like the DWR Approval Backlog.
Watch the DWR Approval Backlog video earlier in this series 
if you want to learn more about how sorting and filtering works.

Just like the DWR Approval Backlog there is the familiar blue triangle 
on the left side of the table. 
Clicking it, expands the DWR to show more details.

The Expand All and Collapse All work just like the DWR Approval Backlog.

After you’ve reviewed the DWRs, check the boxes for the DWRs you want to 
generate an invoice for. 
The Invoice Selected DWRs button will become active. 

To generate an invoice, click the Invoice Selected DWRs button.
If you select DWRs for multiple different jobs, 
each unique job will generate its own invoice.
-- Click Invoice Selected DWRs --

You’ll see a confirmation pop-up showing the number of DWRs 
you’re about to turn into an invoice. 
Click OK.
-- Click OK --

The selected DWRs have now gererated an Invoice.
You’ll notice the DWRs disappear from the backlog immediately. 

You’ll also see a green popup showing the invoice number 
and which job it was created for.
There is a button you can click on that will take you 
right to the generated Invoice.
If you click the button a new tab will open to the Invoice created. 
-- Click here to access new Invoice --

If you made a mistake while generating the invoice, don’t worry. 
If you delete an invoice generated from the DWR Invoice Backlog, 
the DWRs used to create that invoice will return to the backlog 
for review. 

Let me show you.
-- Click Delete --
-- Click Delete --
This will take you to the Job Book Dashboard, 
so I'll go back to the DWR Invoice Backlog.
-- Click DWR Invoice Backlog --

As you can see the DWRs we used to create the Invoice that we just deleted 
are now back in the DWR Invoice Backlog. 

When you generate an invoice using the DWR Invoice Backlog, 
all invoices go to the Invoices card 
and enter the PM Queue for Project Manager review.

We will do a deep dive on the Invoice process in the next video. 

For now, let's connect the dots. Field teams create DWRs. Project
managers approve them in their respective backlogs. Administrators convert
approved DWRs into invoices here. Project managers sign the drafts,
administrators deliver them, and the Active Job Dashboard stays current the
entire time.

A few best practices make the DWR Invoice Backlog run smoothly:

Schedule a dedicated billing block every week. 
When the queue never grows stale, clients see timely invoices 
and cash flow stabilizes.

Use the grouping bar or filter to process one client at a time 
during month end.
Sending a unified package per client reduces back-and-forth questions.

After each billing session, refresh the grid 
and double-check that you haven’t missed anything.
Anything still in the backlog should have a clear plan to move forward.

Before we wrap up, here’s a quick recap. 
We opened the DWR Invoice Backlog 
and reviewed the supporting DWR data. 
We converted selected DWRs into invoices 
ready for Project Managers to review in the PM Queue. 
Each step keeps the path from field work to revenue clear and controlled.

In the next episode, we’ll stay in the invoicing workflow 
and build invoices from scratch. 
You’ll see how to handle fixed-price jobs, edit draft documents, 
and tailor invoice formats before sending them to clients.

Thanks for watching, and I'll see you in the next video!

And don’t forget to subscribe for more Job Book updates and helpful how-to videos!
```

## File: 2.2_Dashboard_Transcript.txt/2.2_Dashboard_Transcript.txt
```
Welcome back to the Job Book How to Use Series. 

This series is for staff who are working with Job Book daily. 

If you’re joining mid-series, start at the beginning as each video builds on the last.

In the last section, I gave you an introduction to this series. 
In this section, I’ll show you how to use the dashboard to stay on top of your work.

In the Setup Series we explained that every user has a role.
Your role determines what you can see and do in Job Book.

First, we’ll look at the dashboard as a Technician, then as an Administrator.

Let’s hop in. 
I’m logged in as a Technician.

I've just logged into the system as a Technician.

When you first log in to Job Book, you’ll land on the dashboard.

At the top left, you’ll see the Navigate button. This is your main menu. 

At the top right, you'll see the Settings button. This is your user settings. 

For daily work, most staff won’t need the Navigate or Settings menus. The Dashboard has everything you need.

On the dashboard you’ll see what we call Cards.
Most cards work the same way. Use Create New to add something new, or Explore to view and edit.

Depending on the modules your company has and permissions your company has given to you, you might see fewer cards than in this video.

In this system starting on the top left card we see:

The My Tasks Card. This is part of the tasking and scheduling module. 
You’ll see My Schedule, which shows your calendar, 
and My Unscheduled Tasks, which lists tasks that haven’t been scheduled.

The Daily Work Records Card is where you create and manage DWRs.
You can think of DWRs like timesheets but different. More on this later in this series. 

The next card is Personal Reports.
You have a My Time Cards report, allowing you to see a report and status of your time cards,
and a My Expense Report, allowing you to see a report and status of your expenses. 

Next to that you have the Expense Card. This is where you create and manage expenses you need to be reimbursed for. 

On the top right you have the Leave Requests card. This is the Leave module. 
The Company Calendar button, is where you can view leaves on a calendar.

On the bottom left we can see the Assets card. This is the asset module.

On the bottom right there is the Safety module. 
There is the Hazards / Tailgate Create button and the Hazards / Tailgate Explore button.
There are multiple forms in the safety module and they can all be accessed via the More button.

As a Technician your day will most likely consist of looking at your tasks and creating DWRs, all of that is accessible from the Dashboard.

Let's take a look at the dashboard now using the role of Administrator.
Administrators have access to all the Cards in the system. 
Managers and Job Coordinators are limited in their permissions and what Cards and Buttons they can see.
Let's take a look at what Administrators see.

I'm now logged into the system as an Administrator role.
I'll make note of any Buttons or Cards, Managers and Job Coordinators don't have access to. 
I'll skip over any of the cards we've already covered as a Technician role as needed.

Starting on the top left card we see:

The Clients Card. This is your client database.
Missing from the Manager role but available to the Administrator and Job Coordinator is the Create New button.
Only Administrators and Job Coordinators can modify clients using the Explore button.

Next to the Clients Card is the Jobs Card. This is your jobs database.
There is the Active Job Dashboard button, where you can view all your active jobs.
Missing from the Manager role but available to the Administrator and Job Coordinator is the Create New button.
Only Administrators and Job Coordinators can modify jobs using the Explore button. Managers only have view access.

Next to the Jobs Card is the Tasks and Scheduling Card. This is part of the tasking and scheduling module. This Card is missing to the Job Coordinators.
There is the Task Dashboard button, where you can view all the tasks in Job Book. 
There is the Task Scheduler button, this is a calendar view where you assign tasks to employees by dragging and dropping tasks onto them.
And finally there is the Explore Task Templates button. This is where you create task templates to apply to jobs. 

The My Task and Daily Work Records cards we already talked about.

The next row on the left there is the Invoice Card. This is where all the invoices in Job Book are. This Card is missing to the Job Coordinators.
Here we have the Invoice Export button, where you can export your invoices to Excel.
Typically project managers go here to approve invoices for import into your accounting system.

Next to the Invoice Card is the Rate Sheets Card. This is where you create rate sheet templates to apply to customers or jobs. This Card is missing to the Job Coordinators.
Missing from the Manager role but available to the Administrator role is the Create New button.
Then there is the Standard Rates button, where you can view all the cost items in the system.

The next three cards: Workflow, Time & Expense Reports, and Cost Reports are not available to Job Coordinators. 

The Workflow Card shows all approval backlogs for DWRs, expenses, and invoices.
The DWR Approval Backlog lets you review and approve timesheets.
The DWR Invoice Backlog lets you convert approved DWRs on T&M jobs into invoices.
The Expense Approval Backlog lets you review and approve expenses.
The Invoice Process Backlog lets you export finalized invoices into your accounting system.

Next to the Workflow Card is the Time & Expense Reports Card. 
This card provides reporting on labour hours, utilization, and expenses.
The Time Card Report shows labour hours and can be exported to Excel for payroll. 
The Time Grid aggregates hours per employee and helps catch errors. 
The Utilization Report shows utilization, chargeability, and effective rate. 
The Expense Report lists all expenses and their status.

The last card on the right is the Cost Reports Card. Also a good reporting hub.
The Line Item Report button will generate a report and show you all the line items used and the amounts used.
The WIP Report button will generate a work in progress report that will show you all your in flight work and what has been invoiced and what has not been invoiced. 

Moving down and on the left we have the Personal Reports and Expenses Cards covered already.

Next to the Expenses Card is the Leave Requests Card. 
Administrators and Managers have access to the Leave Request Report button. This is a report that shows all the leave requests and the status. 
The Company Calendar, Create New, and Explore, buttons were already covered earlier.

Next to the Leave Requests Card is the Assets card. 
Administrators and Managers have access to the Manage Assets button. This allows you to manage your company’s assets and even assign ownership to employees.
The Create New, and Explore, buttons were covered earlier.

On the right side we have the Safety Card covered already. 

Finally at the bottom we have the Job Maps Card.
The search button will allow you to see all jobs in the system on a map. 
There is a geospatial map where you can see physically where past jobs were and you can search and filter them as needed.

If you’re interested in the 
Task & Scheduling module,
The Leave Requests module,
Or the Assets module, 
We have created series for each.
See the description for more information.

For information on the 
various Reports, 
see our Job Book 
Reporting Guide series.

Or click on the link below 
in the description to learn more.

That’s the dashboard overview. 
In the next video, we’ll create Clients, followed by Jobs.

Thanks for watching!
and I'll see you in the next video!
```

## File: 2.3_Creating_Clients_Transcript.txt/2.3_Creating_Clients_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

This series is for staff who are working with Job Book daily. 

If you’re joining mid-series, start at the beginning since each video builds on the one before it.

In the last section, I showed you the dashboard. 
In this video, I’ll show you how to create clients in Job Book.

Before you can create jobs in Job Book, you first need to set up a client. Every job in Job Book must be tied to a client record.

Let’s go ahead and create a client in the system.

As you may remember from the Dashboard Overview video only a person with the role of Administror or Job Coordinator is able to create a client.
So I'll log into into the system as an Administrator role.

From the dashboard, click the Create New button inside the Clients Card at the top left.
-- Click Create New --

The first tab is the client tab and the first field is Client Name. 
As you may remember from the Job Book Setup Series, any field with a red star is required.
The Client Name is usually the company name. For residential work, use the homeowner’s name.

Let’s enter the client name: “Springfield Engineering Ltd.”

The rest of the fields in the Client tab are not required to make a client but let's go through them anyhow. 

Next is Website. Let's enter: "www.springfield.com"

Then Client Types. Here you can tag this customer with multiple premade types. Doing so will allow you to filter clients by type.
I'll select: Construction and Engineers

After that, Rate Sheet. You can set a default Rate Sheet to this customer such that whenever you create a job for this customer it will default to this rate sheet. 
Assuming you've watched the Job Book Setup Series and have setup some rate sheets in your system you should be able to select a Rate Sheet to apply to this customer. 
In my case I'll pick: "Standard Rates"

Next is Payment Terms. You can choose a preset option or type in custom terms. Payment terms are for reference only and don’t affect system behavior.
I'll select: "Account - 30" 
That way I’ll know to follow up if the customer hasn’t paid within 30 days.

Then the Notes field. You can type multiple lines here as notes on the customer.
I'll leave this blank for now. 

There is an Attachments button where you can upload files pertaining to the customer. 
I'll leave this blank for now. 

Let's move to the Contacts tab. 
-- Click Contacts tab --

Here you can add as many contacts to the client as you like. 
-- Click Add --

You’ll see that First Name and Last Name are required. The other fields are optional.
I'll go ahead and fill this out. 

If this client has more than one contact simply add more by clicking on the Add button on the bottom.
-- Click Add --

I'll go ahead and fill the second contact out also.

Once you've filled out the contacts scroll up and click on the the Addresses tab.
-- Click Addresses --

Here you can add billing addresses for invoices. These are not job site addresses.
Click the Add button to add an address to this client.
-- Click Add --

The first field is the Location Name and is required. The rest are not. 
I'll go ahead and fill this out.

If your customer has multiple offices or mailing addresses you would add them here. 
I'll go ahead and add another location to this client. 

Once you have that completed scroll down to the Save button and click save.
-- Click Save --

If you missed a required field the system will highlight it in red. If you don't see the red field check the other tabs.

Once all the required fields are set you should be able to save the client and you will go back to the dashboard.

Don't worry, if you made any mistakes creating the client you can always edit them. 

To edit a client, from the dashboard, click the Explore button inside the Clients Card at the top left.
-- Click Explore --

You'll see the Client Item List. It defaults to the Active clients tab.
If you want to see all your clients you can click on the All tab. 
This will show you all the active and inactive clients in the system. 

To edit a specific client, simply click the client.
-- Click Client --

From the client display screen you can edit, export to PDF, delete, or return to the client list.
Since referenced clients can’t be deleted, the best practice is to deactivate them instead.
More on that later. 

To Edit the client click the Edit button
-- Click Edit --

Notice this client now has both a System Client Number and a Client Number Alias.

The Client Number Alias can be edited to any unique text you like. 

You can go ahead and edit any field you like. 

At the bottom of the client there is an Active checkbox. 

Because the system does not allow referenced data to be deleted best practice is to deactivate Clients instead of deleting them.

Once all your edits are complete remember to click the Save button.
-- Click Save --

This will take you back to the Client Item List.

I'm going to go ahead and create a few more clients in the system.
Feel free to pause the video and create your own clients.

We’ll use these clients throughout the rest of the How to Use Job Book series and in future training videos.

So how are Clients used in the system?

Like we said every job in Job Book must be tied to a client record.

When exporting invoices to your accounting system, all invoices need to include the client's name and address.

If you’re interested in exporting 
invoices to your accounting system, 
keep watching this series.

For information on 
Client Reports, 
see our 
Job Book Reporting Guide series.

Or click on the link below 
in the description to learn more.

That’s everything you need to know to get started with creating and managing clients in Job Book.

In the next video, 
I’ll show you how to
create Jobs in Job Book. 

After that, we’ll cover creating DWRs.

Thanks for watching!
and I'll see you in the next video!
```

## File: 2.4_Creating_Jobs_Transcript.txt/2.4_Creating_Jobs_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

This series is for staff who are working with Job Book daily. 

If you’re joining mid-series, start at the beginning since each video builds on the one before it.

In the last section, I showed you how to create clients in Job Book. 
In this video, I’ll show you how to create jobs in Job Book.

Every project your company works on should be created as a job in Job Book. 
Jobs tie together clients, offices, project managers, and line items.

Let’s walk through creating a job.

As you may remember from the Dashboard Overview video, only Administrators or Job Coordinators can create jobs.
So I'll log in with the Administrator role.

From the dashboard, click the Create New button inside the Jobs Card second from the top left.
-- Click Create New --

The first field is Job Number. This is required. 
Job Book will automatically generate a number for you, but you can overwrite it with your own company’s numbering system if you prefer.

Next to the Job Number is the Job Number Counter.
You can change the counter by unlocking the blue lock button with a click.
This unlocks the Job Number Counter so you can set it.
I'll set this to: "250001"
When you click the blue lock button it will lock in the counter.

Notice the Job Number now defaults to the Job Number Counter.

Next is the Client field. 
Here you can either create a new client or pick one from the dropdown list of clients you’ve already created.
Let’s choose “Acme Corporation” from the list.

For Client Location you have the option of either using the dropdown and selecting a location you previously made for the client, 
or filling in the Client Address at the time of job creation.
I'll use the dropdown and select: "Head Office"

Notice the Client Address is auto-populated with the address we set when we created the client in the previous video.
However, you can manually edit and override the address.

Next is the Project Name. 
Let’s enter the name of our job: “Boundary Survey 5th Avenue”

After that is the Status. This dropdown is required.
Setting the status and updating the status of the job frequently is considered best practice.
That way staff know exactly where jobs are in the workflow. 
I'll select: "Job Setup" from the list. 

The Add Location button is where you set the job location.
You can add multiple locations to a job if needed. 
For this example, I'll just be adding one location. 

-- Click Add Location -- 
Clicking the Add Location button will add a location to a job.
Here we can see:
Location Name, this is just a site name.
Municipal Address, this is the address the system will try to find on a map. More on that later. 
State or Province
And City.

The Legal Addresses button allows you to include data such as Lot, Block, Plan, and Section, Township, Range, if needed.

I'll go ahead and fill in a location name and municipal address for this job. 
-- PAUSE --

As you can see, I've filled in all the fields.
You'll notice the GPS Coordinates are blank.
If I click on the Map Display dropdown the system will try to find the municipal address. 
-- CLICK Map Display --

As you can see the system found the address and placed a blue pin on the mark. 
If you want to move the pin, simply left click anywhere on the map and the pin will move.
Notice the GPS coordinate also updates. 

Below the Add Location button is the Contacts button.
Like the Add Location button you can add multiple contacts.
-- Click Add Location --

When you click on the Contact button it will add two fields.
The Contact dropdown and the Add to DWR slash Invoice checkbox. 
-- Click Contact dropdown --

The Contact dropdown contains all the contacts we created on the Client.
You can pick an existing contact or create a new one.

I'll pick a contact.
The Add to DWR slash Invoice checkbox will add that selected contact to the DWR and Invoice.
See the creating DWRs and creating Invoices videos in this series for what that looks like. 

Below the Add Contact button is the Project Shared Folder.
Many firms use cloud storage or a share drive to store project data.
You can add a link to either so staff can easily access project data.

The next required field is Project Manager. 
Every job needs a project manager. 
Best practice is for Project Managers to approve DWRs and sign off on invoices for the jobs they’re responsible for.


I'll click on the dropdown and
Select: Lance

The next field is Salesperson or Representative.
Just like Project Manager you can select an employee here.
It's not a required field so I'll skip it.

After that you have the Office field.
This is a dropdown with all your offices or departments.
Every job must be tied to an office. 
If your company has multiple offices, select the one this project is running out of. 
When I click the dropdown notice these are the offices we created in the Job Book Setup Guide.
I'll pick: "Head Office"

The Client Project Number, PO Number, and Subcontract Number fields are self-explanatory, and I'll skip over them.

The PO Amount field is the dollar amount the job is worth.
This will be displayed in the Active Job Dashboard. 
More on that in later videos. 

After the Subcontract # you'll see the required field, DWR Billing Type.

In Job Book there are 4 different billing types:
Overhead, Non-Chargeable, Fixed Price, and Time & Materials

An overhead job is typically work done for internal business operations. 
Think administrative tasks, training, vacation, and similar work.

Non-chargeable jobs often support client work or projects but, for various reasons, cannot or should not be billed to the client.
Examples include equipment maintenance, internal project work, rework or fixes, and bench time.

A fixed price job, sometimes called a lump sum job, is a job with a set price.

Finally, a time & materials, or T&M job, is a job where you bill the customer based on the time and materials spent on the job. 

Under DWR Billing Type, is the Invoice Type field.
The options here are Ticket slash Invoice or Invoice.
Most of the time you will set your job to simply be Invoice. 

But sometimes some of your customers might want to see all the hours worked on a job, without the money associated for that work.
If that is the case set the job to Ticket slash Invoice.
We’ll talk more about this in the invoicing section later in the series.

Next after Invoice Type we have Invoice Line-Item Type.
Detailed will show an individual breakdown of all the line items on the invoice.
Summarized will combine identical line items together into one line.

For example, say you did a T&M job and you had a one-man crew working: 8 hours on Monday, 8 hours on Tuesday, and 4 hours on Wednesday.
If the invoice was set to detailed it will have 3 lines for each day of work. 
If the invoice was set to summarized it will have one line saying one man crew, 20 hours.

It might become clearer when you watch the invoicing section in this series. 

Next, we have the GL Code Prefix.
This is used with accounting systems like Sage when companies want to code jobs for import.

After that is the Job Categories.
Like client types, here you can tag this job with multiple categories. Doing so will allow you to filter jobs by their categories.
I'll select: Construction and Engineering

Next there is Job Scope. 
Just like job categories these are more tags you can add to the job. As you can see we have many job scopes you can tag the job with.
I'll select: Boundary Stake-Out and Commercial Building Construction

If there’s a scope you’d like to use that isn’t on the list, the Job Scope Details field lets you add it.

Order Date and Due Date are fairly self explanatory. 
The due date will be visible on the Active Job Dashboard.

I'll set the order date September 15th and the due date October 31st.

You can add multiple taxes to the job if applicable.
-- Click Add --
-- Click X --

And you can add multiple fees as a percent to the job if needed.
-- Click Add --
An example of a fee would be a percent fee for administration. 
-- Click X --

Additional Fields will create additional fields on the invoice 
-- Click Add --
-- Click X --

There’s also a Notes field. Use this to store any internal notes about the job. 

Next, we have the Rate Sheet. 
You'll notice the "Standard Rates" rate sheet was selected by default. 
This is because when we created the client, we assigned that rate sheet as the default. 
So when we created this job for the "Acme" client it used the default rate sheet. 

You can use a different rate sheet if you like, by simply clicking on the dropdown and selecting a different rate sheet to apply to the job. 
I'll pick: "Construction Survey"

The Billable Line Items section consists of a collection of line items.
These line items represent the:
Labour Costs, 
-- Click Equipment & Materials --
Equipment & Materials, 
-- Click Fixed Price --
and Fixed Price line items. 
-- Click Labour Costs --

Pick the items your staff will use on this job.
When you select a line item, it pulls the default rate from the system. 
You can adjust rates for this specific job if needed.
You have the option of manually selecting individual line items to add to the job.
Or you can click the blue Replace Line Items with Rate Sheet button.
This will import the rate sheet template we created in the How-to Setup Job Book video series.
-- Click Replace Line Items with Rate Sheet -- 

As you can see:
Labour Costs, 
--Scroll down -- 
-- Click Equipment & Materials --
Equipment & Materials, 
-- Click Fixed Price --
and Fixed Price line items. 
--Scroll down --

Have been imported from our "Construction Survey" rate sheet.
-- Click Labour Costs --

You can still manually remove or add line items.
For example, for this job it looks like there are two field staff available to work.
Let's change that. Let's remove the "Survey Assist" and "Party Chief". You can do that by clicking on the X to the left of the line item.
-- Click X --
-- Click X --

Now they are removed but we don't have any field staff line items that people can select and use. Let's add a new line item.
Click the Add button.
-- Click Add --

Notice everything is blank. Click on the Cost Item dropdown
and select: "1 Man Survey Crew"

This is the order the line items are in. If you want to change the order, simply click on the arrows to move the line items. 
I'm going to move the "1 Man Survey Crew" to the top.

Let's take a look at the Fixed Price tab.
-- Click Fixed Price --
There are a lot of line items here we don't need. 
I'm going to remove all of them besides "Construction Survey"

Ok that looks good. Let's go back to the Labour Costs tab.
-- Click Labour Costs --

Let's take a closer look at the individual line items.
Notice the "Unit Cost" for the "1 Man Survey Crew" was automatically set. 
This number came from the default rate that we set in the How-to Setup Job Book video series.

Let's change that to: "$160"

The CAD, Project Manager, and Professional Land Surveyor "Unit Cost" was taken from the "Construction Survey" rate sheet.
You can also override those unit costs but I won't bother.

At this point, you might be wondering about the empty "Budget Quantity" fields. 

The budget quantity fields are used when estimating the amount of time or quantity a line item will take for a given job.
Every job, whether fixed price or T&M, should have an estimate associated with it.
Best practice is to fill in the budget quantity for each individual line item based on the estimate.
We cover budget quantity in more depth in our Job Book Reporting Guide series.

For now, I'm going to fill in the budget quantity for all the line items. 

Now that this is done, I'm going to save the job. 
Don't worry if you need to make any changes to the job, you can always go back and edit the job.
-- Click Save --

Once the job is saved, you'll see the Jobs Item List. It defaults to the Active jobs tab.
The Inactive and the All tabs will show you the inactive jobs and all the jobs in the system respectively.

To edit a specific job, simply click the job.
-- Click Job --

From the job display screen you can edit, export to PDF, close, delete, or return to the job list.
We’ll cover cloning and deleting jobs later.

To Edit the job, click the Edit button
-- Click Edit --

You can go ahead and edit any field you like. Including the Job Number.

At the bottom of the job there is an Active checkbox. 

Once a job is completed and invoiced the best practice is to deactivate the job in the system. 
A deactivated job can’t be selected when creating DWRs.
You can always reactivate a job if it becomes active again or if you need to assign time to it.

All jobs are still visible in the All tab and still visible in the Job Maps.
 
Because the system does not allow referenced data to be deleted best practice is to deactivate Jobs instead of deleting them.

Once all your edits are complete remember to click the Save button.
-- Click Save --

This will take you back to the Job Display screen.

If you click the Clone button, it will create a copy of the job.
A new Job Number will be assigned.
The Status of the job, the PO #, and PO Amount will not be set. 
All the other data will be copied.

Cloning a job is useful when a project has parts that need to be invoiced separately, 
for example, projects with multiple phases or different scopes.

I'm going to go ahead and create a few more jobs in the system.
Feel free to pause the video and create your own jobs.

We’ll use these jobs throughout the rest of the How to Use Job Book series and in future training videos.

-- --

So why are jobs important?
Every DWR, expense, and invoice must be tied to a job.  
Jobs give you real-time visibility on project progress.  
Reports and backlogs are organized by job.  

For information on Job Reports, 
see our Job Book Reporting Guide series.

Or click on the link below in the description to learn more.

That’s everything you need to know to start creating and managing jobs in Job Book.

In the next video, I’ll show you how to create Daily Work Records, or DWRs, which your staff will use to record time and materials.

After that, we’ll cover creating Expenses.

Thanks for watching!
and I'll see you in the next video!
```

## File: 2.5_Creating_DWRs_Transcript.txt/2.5_Creating_DWRs_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

If you’re just joining, make sure you’ve watched the earlier episodes because each one builds on the last.
In the previous video, we created jobs and set up the billing details that your teams will rely on. 
Now we’re ready to capture the actual work. 

In this video, I’ll show you how to create Daily Work Records, or DWRs, in Job Book.

Technicians create most DWRs each day.
So I’m logged in as a Technician, simulating being on a cell phone.
Project managers and administrators can follow the same steps. 

DWRs are the backbone of Job Book. They replace paper timesheets, keep labour, equipment, and materials 
tied to the correct job, and feed the approval, invoicing, and reporting workflows you’ll see later in this series. 

From the dashboard, look for the Daily Work Records card. 

Click Create New
-- Click Create New --

You’ll go straight into a new DWR form. Let’s walk through it from top to bottom.

Date is the first field and defaults to today's date.
The date should be set to when the work happened. 
If you’re logging multiple days, create one DWR per day per job.

The Job field is next. 
-- Click Job dropdown --
Pick the job you worked on today. I’ll choose “Boundary Survey – 5th Avenue,” the job we built in the last episode. 

Below the Job field is the DWR Details.

First, let’s look at the Job details.
-- Click Job Details --
Here you can see the details of the job.

Let’s move into Labour Costs. 
When you click the add button 
-- Click Add under Labour --
you will see Cost Items, Employees, Hours, and Description of work.

Click the Cost Item dropdown.
-- Click Cost Item dropdown --

This section pulls line items from the job, 
so what you’re seeing here is based on the setup we did earlier, when we created the job.
Different jobs will have different line items to pick from.

Choose the labour line item that matches the work performed. 
I’ll select “1 Man Survey Crew.” 

Now select the Employee that did the work. 
-- Click Employee dropdown --
A crew lead can add time for the rest of the crew as well. We’ll add additional labour in just a moment.

Enter Hours Worked. 
Today we were on site for 8 hours. 
You can either select a start time and end time, 
or simply enter the total hours worked.

-- Click Clock Select 8 am --
I'll pick a start time of 8am

-- Click Clock Select 4 pm --
And an end time of 4pm.

Notice that the hours are calculated automatically.

Finally you have the Description of the work. 
The description helps with record keeping and DWR approvals so make sure you add enough details.
-- Type "Set control points along south property line. Heavy rain delayed layout after 1 PM." --
A detailed note helps the project manager understand the day at a glance without calling you for more context.

If you need to break the shift into multiple activities or need to add another crew member, 
add another labour line item. 
When a crew lead enters time for others, make sure the hours match what they worked. 

I'll go ahead and add another crew member.
-- Click Add --

Notice all the familiar fields. 

I'll select “1 Man Survey Crew” again.
For the employee I'll use "Denice Rodman"

Denice worked the same hours as me so this time I'll just input 8 hours, 
instead of using a start and end time. 

I'll fill in the Description of the work.
-- Type "Set up equipment."

Next, we'll log any equipment you used.

Click Equipment & Materials tab
-- Click Equipment & Materials tab --
Then Click Add
-- Click Add --

Click the Cost Item dropdown.
-- Click Cost Item dropdown --

Just like the Labour Costs line items, this section pulls line items from the job,
so what you’re seeing here is based on the setup we did earlier, when we created the job.

Select the equipment line item
In my case, I’ll select "Robotic Total Station" and enter the number of hours.
-- Type "8" --

Add any consumables or materials as separate items.
I'll add four "Iron Survey Posts".
-- Type "4" --

Notice for Equipment and Materials, the Description is not a required field. 

Below DWR Details is the Representative Signature. 
Because someone can create DWRs for other employees, the person creating the record needs to sign off on it.
Assuming you've saved your signature as an employee, 
clicking the "Add My Signature" button will automatically
add your signature and fill in the Representative field.

The Client’s Representative Signature is optional, used when technicians need to get a client’s signature on a DWR.

If you’re still working in the field and plan to come back later to add information, uncheck the Submitted box.
DWRs that have not been submitted will be in your My Form Not Submitted tab. More on that later in the video.

I'll uncheck the Submitted checkbox to show you. 

Now let’s save the record.

-- Click Save --
The system will then Validate the DWR, click the Acknowledge and Close button.

This will take you back to the Dashboard.

To view your DWRs click on the Explore button in the Daily Work Records card.
-- Click Explore --

At the top you’ll see three tabs: My Forms Not Submitted, My Forms Not Approved, and All My Forms.

My Forms Not Submitted, as the name suggests, shows the DWRs you’ve created but not yet submitted for approval.
Here you can see the DWR we just created. 

-- Click My Forms Not Approved --
This is the My Forms Not Approved tab. Notice there are no DWRs here.

DWRs located in the My Forms Not Submitted or My Forms Not Approved tabs can be edited.
Once the DWR has been approved, it can no longer be edited by a technician.
If you need to edit a DWR that has been approved, 
you’ll need to ask a Project Manager or Administrator to uncheck the Submitted box so you can edit it again.

-- Click All My Forms --
The All My Forms tab will show all your DWRs. 
Once a DWR has been approved you will only be able to see it in this tab.
You can not edit DWRs in this tab.

Let's go ahead and submit the DWR we just created.
To do that click on My Forms Not Submitted.
-- Click My Forms Not Submitted --
Then click on the DWR.

There are four buttons on the top of the Display screen. 
Edit, Export to PDF, Delete, and Back.

The Edit button will allow you to edit the DWR.
The Export to PDF button creates a file you can print or email to a customer if needed.
The Delete button will delete the DWR and the Back button will take you back to the display screen.

For now click the Edit button so we can submit the DWR.
-- Click Edit --

Here you can edit whatever information you like. 
When everything is complete and accurate, check the Submitted box and save.
This will add the DWR to the approval backlog for your project manager.

Notice the Submitted Date is automatically saved.

-- Click Save --
Once saved click the Back button 
-- Click Back --

You'll notice on the Explore list your DWR is gone.
That's because you are in the My Form Not Submitted tab.
If you click on the My Form Not Approved tab 
-- Click My Forms Not Approved --
You should see your DWR waiting to be approved by a project manager.

That’s about everything you need to know to create Daily Work Records in Job Book.

If you are a project manager you might be interested in how to approve all these DWRs. 
If so check out our DWR Approval Backlog video.
We’ll step through that approval process from the manager’s point of view.

If you are an administrator you might be interested in how to turn all these DWRs into invoices.
If so check out our DWR Invoice Backlog video. 
We’ll step through that inovice creation from the administrator's point of view.

Before we wrap up, here are a few best practices:
Submit DWRs every day. Waiting until the end of the week increases the risk of missing hours or losing track of equipment.
Double-check the job and date before submitting. Reassigning DWRs after approval takes time away from billing the job.

By following these steps, every DWR becomes a reliable record that supports approvals, dashboards, and invoices without extra work.

In the next video, we’ll stay in the technician role and walk through creating expenses.

Thanks for watching, and I’ll see you in the next video!
```

## File: 2.6_Creating_Expenses_Transcript.txt/2.6_Creating_Expenses_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

If you’re just joining, make sure you’ve watched the earlier episodes because each one builds on the last.
In the previous video, I showed you how to create DWRs.

In this video, I’ll show you how to create expenses in Job Book.
Expenses are out-of-pocket costs your staff pay and need to be reimbursed for.
If your company relies on corporate credit cards, you might have fewer personal expenses to submit.
But when you do pay out of pocket, this is where the Expenses workflow keeps everything organized. 
Submit expenses as promptly as possible. 
Submitting quickly keeps the reimbursement cycle short and gives managers a real-time picture of job costs.

I’m logged in as a Technician, but project managers and administrators can follow the same process.

From the dashboard, look for the Expenses card.

Click Create New
-- Click Create New --

The expense form opens. Let’s go through it from top to bottom.

Date is the first field and defaults to today's date.
Set this to the day the purchase happened. 
Expenses should reflect the transaction date, even if you’re filing them later in the week.
Create one expense for each payment or receipt.

The Employee field is next.
-- Click Employee dropdown --
The logged-in employee appears by default, but you can also file an expense for someone else if needed. 
I’ll leave it as myself for now. 

Below the Employee field is the Job field.
-- Click Job dropdown --
Pick the job that generated the expense. I’ll choose “Boundary Survey - 5th Avenue,” the same project we used in the DWR episode. 
Best practice is to match the expense to the job it applies to.
That keeps budgets aligned and avoids rework at approval time.

Let’s move to the Expense Item dropdown.
-- Click Expense Item --
The Expense Item dropdown shows the expense types set up by your administrators.
Accommodations, Field Allowance, Field Materials Misc, Gas, Misc, and more.

I’ll select “Gas.”

Enter the Total Expense Amount. 
-- Type "78.54" --
I’ll enter seventy-eight dollars and fifty-four cents, the amount shown on the receipt.

For the Description, add a quick note that explains the purchase, such as 
“Filled unit 204 after Boundary Survey crew shift.” 
Detailed notes save time when managers or auditors review the record later.

After Description there is the Attachments button.
When you click the Attachments button,
-- Click Attachments --
you'll be able to take a picture of the receipt with your cellphone. 
Or if you are on a computer you can click the Select File button to upload a file. 

Attach photos or PDFs of every receipt. Job Book stores them with the record so approvers and auditors don’t have to chase you later. 
Take a photo of the receipt as soon as you get back to the truck and upload it while you have a good connection.

Many teams also add a photo of the signed hotel folio as a second backup. 
More documentation means faster approvals.

Finally there is the Submitted checkbox.

If you’re still gathering receipts, uncheck Submitted and you can save a draft expense.
Draft expenses remain in your My Expenses list, and they don’t post to approvals until you finalize them. 
I'll uncheck Submitted.

When you click Save, Job Book checks that all required fields are filled in before saving.
If anything is missing, Job Book will highlight the field in red. 
Simply fix the items, then click Save again.
-- Click Save --

This will take you back to the Dashboard.

To view your Expenses click on the Explore button in the Expenses card.
-- Click Explore --

At the top you’ll see two tabs: My Expenses and All My Expenses.

My Expenses shows the expenses you’ve created but not yet submitted for approval.
Here you can see the expense we just created. 

The All My Expenses tab shows all your expenses. 
Once an expense is approved, you’ll only be able to view it in this tab.
You can not edit expenses in this tab.

Let's go ahead and submit the Expense we just created.
To do that click on the expense. 

There are four buttons on the top of the Display screen. 
Edit, Export to PDF, Delete, and Back.

The Edit button will allow you to edit the Expense.
The Export to PDF button makes a file you can print or email if needed.
The Delete button will delete the Expense and the Back button will take you back to the display screen.

For now click the Edit button so we can submit the Expense.
-- Click Edit --

Here you can edit whatever information you like. 
When everything is complete and accurate, check the Submitted box and save.
This sends the expense to your administrator for approval in the Expense Approval Backlog.

Notice the Submitted Date is date-stamped when the expense was submitted.

-- Click Save --
Once saved click the Back button 
-- Click Back --

You'll notice on the Explore list your Expense is gone.
That's because you are in the My Expenses tab.
If you click on the All My Expenses tab 
-- Click All My Expenses --
You should see your expense waiting to be approved by a project manager.

That’s about everything you need to know to create expenses in Job Book.

If you’re an administrator, check out our Expense Approval Backlog video,
to see how to approve expenses from your point of view.

You can also watch our DWR Invoice Backlog video,
to learn how administrators turn approved DWRs into invoices.

Before we wrap up, here are a few best practices to keep expense processing smooth.
Submit expenses daily or at least weekly so approvers have fresh details and you get reimbursed faster.
Match expenses to the same job you used on your DWR to keep budgets accurate and avoid billing delays.
Upload receipts right away. Faded or missing copies slow down approvals and can jeopardize reimbursement.
Use meaningful descriptions so approvers understand how the purchase supported the job without calling you.
Review your totals before submitting. Fixing small errors now prevents a manager from rejecting the expense later.

By following these habits, expenses move through approvals quickly, you get reimbursed on time, and project costs stay accurate for dashboards and invoices.

That’s everything you need to know to create expenses in Job Book.

In the next video, we’ll switch to the project manager role and explore the Active Job Dashboard, 
where you can monitor budgets, progress, and upcoming deadlines at a glance.

Thanks for watching, and I’ll see you in the next episode!
```

## File: 2.7_Active_Job_Dashboard_Transcript.txt/2.7_Active_Job_Dashboard_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

If you’re just joining, make sure you’ve watched the earlier episodes 
because each one builds on the last.

In the Creating DWRs and Creating Expenses videos, 
we created timesheets and expenses and assigned them to jobs.

All those submissions feed into the Active Job Dashboard.
The Active Job Dashboard brings job status, labour, expenses, and billing together in one view.

Staying on top of it helps you track your budget, keep invoices moving, 
and maintain predictable cash flow. 

You can see job status and dive deep into individual job performance metrics.

I am currently logged in as a Project Manager.
Administrators and Job Coordinators see the same layout and follow the same steps.

From the main dashboard, look at the Jobs card in the top row.
Then click the Active Job Dashboard button.
-- Click Active Job Dashboard --
The Active Job Dashboard becomes the control center for every live project.

At the top left, you’ll see the Export to Excel button. 
Clicking it downloads an Excel file with all the job data you’re currently viewing.

Next to that is the Templating section, where you can create templates 
to customize how you view the Active Job Dashboard.

We do a deep dive into templating in our Job Book Reporting Guide Series

Below that is the grouping bar. 
You can drag column headers here to group jobs by Client Name, Project Manager, or any other field.

Again we do a deep dive into this advanced feature in our 
Job Book Reporting Guide Series.

Below that you have the Job Table.
The Job Table displays all active jobs in the system.
You can change how many columns you see 
and apply filters to the data. More about that later in this video. 

In the default view, from left to right, you’ll see 
the Job Number, the Client Name, and the Project Manager.

the Status column shows exactly where that job sits in your workflow, 
whether that is Job Setup, In Progress, Ready for Billing, or any stage your company uses.

Next the Billing Type, and Due Date.

The next set of columns are the key indicators project managers rely on. 

The Purchase Order amount shows the client’s approved budget. 
The DWR amount adds up all approved hours to date multiplied by their billing rates. 

The Expenses to Date column shows all reimbursable costs submitted through the expense workflow.

Next are the Total Invoiced, Last Invoice Date, and the Action column.

The Action column has four buttons. Each button is specific to the job. 

The Job Charge-Out Rate Report shows all DWR and invoice activity.

The Job Charge-Out Rate Summary Report combines all line items 
so you can compare budgeted amounts, DWRs, and invoices.

The Job History Report lists every line item linked to a job, including assets and notes.

Each report provides valuable insights that can help you make informed decisions 
about job performance, costs, and history related to the job.

For detailed instructions on these reports see our Job Book Reporting Guide Series. 

The final button is the Create Invoice button.
If the job was set to time and material that button will take you to the DWR Invoice Backlog 
and filters for only the DWRs linked to that job.

If the job was set to fixed price that button will create an Invoice for that job. 

If the job was set to non-chargeable or overhead the button will not be displayed. 

We cover the DWR Inovice Backlog and Invoice creation later in this How to Use Job Book Series. 

The Job Table is a crucial tool for tracking job performance 
and is essential to ensure accurate budgeting and financial accountability.

Some of you eagle-eyed viewers, might notice a blue triangle on the left side of the table.
If you click the triangle, it expands to show all the invoices linked to that job.

Looking at the Job Number column you'll see a black arrow. 
This will sort the invoices in ascending or descending order.
If you click the arrow again that column will be unsorted. 

You can sort by any column in the table by clicking on the column.
-- Click Client -- 

You can add or remove columns in the Job Table. 
Simply click the three black dots on any of the columns.
-- Click 3-dots --

You’ll see a dropdown with options to sort ascending or descending, choose columns, or apply filters. 
Hover over Columns to see a checklist of every available column.
Columns that are currently visible are checked. Unchecked columns are hidden.

If the Billing Type column isn’t important to you as a project manager, 
just uncheck it and it will disappear from your view.

Speaking of Project Manager that column shows all the project managers for all the active jobs.
You’re probably not interested in jobs you don’t manage, so let’s filter the list to show only your own jobs.
Click the three black dots again over the Project Manager column. 
-- Click 3-dots --

And hover over the filter item.
You can use “Show items where the value is equal to,” or, what I prefer, “Starts with” or “Contains.”
Then type your name.
-- Write Lance --
and click Filter
-- Click Filter --
Now you can see only the jobs you are managing in the dashboard, 
making it easier to manage your jobs and streamlining your workflow.

That’s about the basics of the Active Job Dashboard. 

If you want to learn about grouping columns, creating and using templates, 
or exploring reports like the Job Charge-Out Rate Report, 
the Summary Report, or the Job History Report, 
check out our Job Book Reporting Guide Series.

Here is how the Active Job Dashboard ties into the rest of Job Book. 

Every DWR and expense you saw in earlier episodes updates these metrics the moment it’s submitted. 
Project managers rely on these numbers to manage their jobs effectively.

Administrators use the Active Job Dashboard to quickly find jobs and then either 
use the DWR Invoice Backlog or the invoice module to keep billing on schedule. 

Keeping the dashboard accurate requires a few habits. 
Update job statuses as soon as milestones change.
Inactive jobs can’t be used by technicians when creating DWRs, 
so keeping your job list up to date helps prevent mistakes.

Make sure new jobs include budget quantities, even for time and materials work, 
because the burn column compares actuals to those targets.

Encourage technicians to submit DWRs and expenses every day. 
Otherwise, the Hours to Date and Expenses to Date columns will fall behind reality.

When a job shows activity but no approved billing, check whether invoices are 
waiting for documents or sitting in draft.

Best practices keep the dashboard useful day after day. 
Check the dashboard every morning to spot issues before crews leave the office.

Review the Burn column before client calls so you can address potential overruns proactively. 
If a job shows zero entries for several days, call the field lead and confirm that 
crews are submitting DWRs on time.

Administrators and project managers should schedule a standing dashboard review.

Keep this rhythm and the Active Job Dashboard becomes your single source of truth 
for how your operations are performing. You’ll always know which jobs are healthy, 
which need attention, and which approvals must be finalized before invoices go out.

In the next video, we will stay in the project manager role 
and work through the DWR Approval Backlog 
so technician submissions keep moving without delay.

Thanks for watching, and I’ll see you in the next video!

And don't forget to subscribe for more updates and tips from the Job Book channel!
```

## File: 2.8_DWR_Approval_Backlog_Transcript.txt/2.8_DWR_Approval_Backlog_Transcript.txt
```
Welcome back to the Job Book How to Use Series.

If this is your first time watching, 
remember that each episode builds on the last.

In the last video, we explored the Active Job Dashboard 
and learned how to monitor project health in real time. 
That dashboard helps identify which jobs need attention.

In this episode, we’ll dive into the DWR Approval Backlog. 
The DWR Approval Backlog is where a Project Manager 
validates the work records that drive every job metric.

This episode is all about clearing that backlog efficiently 
so approved records reach payroll, reporting, 
and billing without delay.

Before we jump into the screen, let’s review why approvals matter. 
Daily Work Records, or DWRs, capture labour, 
equipment, and materials in a single submission. 
Until they’re approved, they’re provisional. 
Approving them confirms that the information is ready 
for payroll, cost tracking, and invoicing.

I’m logged in as a Project Manager so I can walk you through the 
Daily Work Record approval flow from end to end.

From the main dashboard, look at the Workflow card 
in the middle of the second row, 
then click the DWR Approval Backlog button.
-- Click DWR Approval Backlog --
The DWR Approval Backlog is the DWR batch approval center for every project.

At the top left, you’ll see the Approve Selected DWRs button. 
It will be inactive until you select DWRs to approve. 

At the top right, you’ll see the Expand All, Collapse All, 
and Undo Last Approval Batch buttons. 

Below that is the grouping bar. 
You can drag column headers here 
to group jobs by Job Number, Project Manager, or other fields.

Below that is the DWR Table, 
which shows all DWRs in the system that have not yet been approved.

The first column is a checkbox. 
Clicking the checkbox in the header selects all DWRs for bulk approval. 
Unchecking it will deselect all DWRs.

Next are the Date, Created By, Submitted Date, and DWR Number columns. 
The DWR Number column contains hyperlinks to the individual DWRs.

Then you have the Job Number, Client, Project Manager, and Office columns.

By default, DWRs are sorted by Date and Job Number in ascending order. 
That means the oldest DWRs appear first, 
and within each day, they’re sorted by Job Number.

Multiple columns can be sorted at once. 
If you want to sort by only one column, 
you’ll need to remove sorting from the others 
by clicking the sorted column until the arrow disappears.

If I want to sort by Client, I’ll remove sorting from the Job Number column.
-- Click Job Number twice --

And from the Date column.
-- Click Date twice --

Then I’ll click the Client column heading.
-- Click Client once --

When the arrow points up, it’s ascending. Click again to switch to descending.
-- Click Client once --
Click once more to remove sorting.
-- Click Client once --

You can also filter data by clicking the filter icon 
or typing in the quick filter field in certain columns. 

If I’m Lance and only want to see DWRs for jobs I manage, I’ll simply type 'Lance.'
-- Type 'Lance' --

The dropdown will show a filtered list to choose from. 
Select the employee.
-- Click 'Lance L' --

Now all DWRs are filtered to Project Manager Lance. 
You can clear the filter by clicking the X on the quick filter 
or the Clear Filter icon.

More complex filters can be used by clicking the filter icon on the column heading.
-- Click heading filter --

Sometimes a DWR might need a small adjustment. 
If it’s just a typo or a minor fix, you can correct it on the spot. 
Keep in mind that direct edits mean you own that change.

If you need a closer look at or need to edit a specific DWR, 
click the hyperlink. 
-- Click DWR hyperlink --
A new browser tab will open where you can review, edit, 
or manually approve the DWR.
-- Click DWR Tab --

If the submission needs more work, 
tell the technician who submitted the DWR to edit it instead. 
Technicians can edit their own DWRs until they’ve been approved. 
Be clear about what needs to change and why.

Approving multiple DWRs one by one can get cumbersome.
-- Click DWR Approval Backlog Tab --

You might have noticed a blue triangle on the left side of the table. 
If you click it, the record expands to show more details.

You can expand all DWRs at once 
by clicking the Expand All button on the top right. 

You can see the line items used, the hours, the unit, the quantity, and the description. 
This lets you quickly review multiple records 
without opening each DWR individually.

After you’ve reviewed the DWRs, check the boxes for the ones you want to approve. 
The Approve Selected DWRs button will become active. 

To approve in bulk, click the Approve Selected DWRs button.
-- Click Approve Selected DWRs --

You’ll see a confirmation pop-up showing the number of DWRs you’re about to approve. 
Click OK.
-- Click OK --

The selected DWRs have now been approved. 
You’ll notice they disappear from the backlog immediately. 
Approving DWRs locks the records, meaning they’re no longer editable by the technician. 
Approved DWRs can now be used in the DWR Invoice Backlog 
if the job is set to Time and Material, 
or directly when creating an invoice. 

If you made a mistake, you can click the Undo Last Approval Batch button.
-- Undo Last Approval Batch button --

You’ll see a confirmation pop-up showing the number of DWRs you’re about to unapprove. 
Click OK.
-- Click OK --

You should see all the DWRs return to your backlog.

If you ever need to unapprove a DWR 
and the Undo Last Approval Batch is inactive, 
you’ll need to locate the approved DWR manually.
To do this, go to Explore in the Daily Work Records card.
-- Click Navigate Home, Click Explore DWRs --
Then go to the All tab. 
-- Click All tab --
Find the DWR you want to unapprove. 
-- Click DWR --
Open the DWR for editing. 
-- Click Edit --
Uncheck the PM Approved checkbox, then click Save.
-- Click Save --
-- Click Navigate, Home --

That’s about all there is for the DWR Approval Backlog. 

If you want to learn more about the DWR Invoice Backlog, 
check out the DWR Invoice Backlog video later in this series.

Approvals should happen daily or at least before payroll cutoff. 
Delays cause payroll issues and slow invoicing. 
Set aside about ten minutes at the end of each day, 
or first thing in the morning, to clear the queue. 
It keeps cash flow smooth and gives leadership confidence 
in the job data they review.

Remember that approved DWRs feed several backlogs in Job Book. 
They populate the DWR Invoice Backlog for Time and Materials jobs, 
they feed cost actuals in the job budget view, 
and they roll into payroll exports. 
A careful review here prevents errors later. 
Accurate data now means faster invoicing and fewer write-offs down the line.

Here’s a quick recap. 
The DWR Approval Backlog is where you validate every Daily Work Record 
before it affects payroll, reporting, and invoicing. 
Check the queue often, use filters to focus, and review each section carefully. 
Those habits keep your data accurate and your projects on track.

In the next video, we’ll stay in the approvals workflow 
and walk through the Expense Approval Backlog, 
so staff expenses are processed quickly and efficiently.

Thanks for watching, and I’ll see you in the next video!

And don’t forget to subscribe for more Job Book updates and helpful how-to videos!
```

## File: 2.9_Expense_Approval_Backlog_Transcript.txt/2.9_Expense_Approval_Backlog_Transcript.txt
```
Welcome back to the Job Book How to Use Series.
If this is your first time watching, 
remember that each episode builds on the last.

In the last video we explored the DWR Approval Backlog.
We bulk approved daily work records before they flowed into payroll and invoicing.

In this episode, we’re going to clear the Expense Approval Backlog.
This is where submitted expenses wait for a 
Project Manager or Administrator to review.
Think of it as the gatekeeper that protects cash flow, 
reimbursement accuracy, and client billing integrity.

Before we jump into Job Book, let's talk about why this backlog matters.
Expenses in Job Book are costs paid by staff on behalf of a job 
that need reimbursement.
If we approve them blindly we risk billing the wrong client 
or paying staff for the wrong amount.
A steady approval rhythm keeps reimbursements timely 
and your general ledger clean.
It also keeps our job budgets trustworthy 
when leadership checks the numbers.

I am logged in as an Administrator so I can see every expense awaiting review.
You can follow the same process as a Project Manager 
if that is the role assigned to you.

Now let’s walk through the screen together 
and see how the approval process works.
From the main dashboard, look at the Workflow card 
in the middle of the second row,
In the Workflow list choose Expense Approval Backlog.
-- Click Expense Approval Backlog --
The Expense Approval Backlog is the expense batch approval center for Job Book.

At the top left you will see the Approve Selected Expenses button.
It will stay inactive until we have at least one expense checked.
At the top right, you’ll see the Undo Last Approval Batch button.

Below that is the grouping bar. 
You can drag column headers here 
to group jobs by Job Number, Employee Name, or other fields.

Below that is the Expense Table.
The Expense table lists every submitted expense that still needs approval.

The first column is a checkbox. 
Clicking the checkbox in the header selects all expenses for bulk approval. 
Unchecking it clears all selections.

Next is the Date column. 
The Date column contains hyperlinks to the individual Expenses.

Then you have the Submitted Date, Job Number, Expense Item, 
Employee Name, Amount, and Description columns.

By default, Expenses are sorted by Date and Employee Name in ascending order. 
That means the oldest Expenses appear first, 
and within each day, they’re sorted by Employee Name.

You can sort by multiple columns at once. 
To focus on one column, remove sorting from the others 
by clicking the sorted column until the arrow disappears.

Just like we did in the DWR Approval Backlog video in this series.

Just like the DWR Approval Backlog, 
you can filter data using the filter icon 
or by typing in the quick filter field in certain columns.

Sometimes an Expense might need a small adjustment. 
If it’s just a typo or a minor fix, you can correct it on the spot. 

If you need to edit or see attachments on an Expense, 
click the hyperlink. 
-- Click Expense hyperlink --
A new browser tab will open 
-- Click Expense Tab --
where you can review, edit, 
or manually approve the expense.

You can also check off the Processed checkbox.
The Processed checkbox can mean different things depending on the situation. 
For reimbursements, it means the staff member has already been paid. 
For billable expenses, it means the expense was included on an invoice.

If you want to learn more about the relationship between 
Processed and Unprocessed Expenses in Invoices
check out the Creating Invoices video later in this series.

If the submission needs more work, 
tell the staff member who submitted the Expense to edit it instead. 
Technicians can edit their own Expenses until they’ve been approved. 
Be clear about what needs to change and why.

Just like the DWR Approval Backlog approving multiple Expenses 
one by one can get cumbersome.
-- Click Expense Approval Backlog Tab --

If you recall from the Creating Expenses video in this series 
every expense represents one item or receipt.

From the Expense table you should have all the information needed 
to approve an expense without opening each Expense individually.

After you’ve reviewed the Expenses, check the boxes for the ones you want to approve. 
The Approve Selected Expenses button will become active. 

To approve in bulk, click the Approve Selected Expenses button.
-- Click Approve Selected Expenses --

You’ll see a confirmation pop-up showing the number of Expenses 
you’re about to approve. 
Click OK.
-- Click OK --

The selected Expenses have now been approved. 
You’ll notice they disappear from the backlog immediately. 
Approving Expenses locks the records, 
meaning they’re no longer editable by technicians. 

Just like the DWR Approval Backlog 
you can undo a batch approval by clicking on the 
Undo Last Approval Batch button.

The process to manually unapprove an Expense is the same as for unapproving DWRs.
You need to locate the approved Expense,
Edit the expense, and ucheck the Approved checkbox. 

That’s about all there is for the Expense Approval Backlog. 

Let's talk about integration.
Expenses flow directly into the Active Job Dashboard, 
allowing Project Managers to compare committed costs against estimates.

When invoicing a Job all expenses related to the job are listed.
Administrators can then include those expenses if needed 
and set the expenses to Processed.

Here are a few best practices that seasoned administrators follow.
First, schedule a daily approval window.
Clearing the backlog at the same time each day 
keeps reimbursements predictable for staff.
Second, scan for duplicates before you approve.
If two employees submitted the same hotel receipt, reject the duplicate immediately.
These small habits keep approvals fast without sacrificing accuracy.

Before we wrap up, let's recap what we covered.
We opened the Expense Approval Backlog from the Workflow card.
We reviewed an expense record, checked attachments, and confirmed job coding.
We approved clean expenses.
We used bulk approvals to speed up high-volume days.
Most importantly, we saw how this backlog feeds invoicing, reporting, and cash flow.

In the next video we will move deeper into billing 
and explore the DWR Invoice Backlog.
That’s where DWRs for Time and Material jobs land, 
making it easy to build customer invoices.

Thanks for watching, and I’ll see you in the next video!

And don’t forget to subscribe for more Job Book updates and helpful how-to videos!
```
