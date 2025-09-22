# 'How To Use' Job Book Scripts

## Background

Job Book is a project management software solution for land surveyors and engineers. https://getjobbook.com

After setting up Job Book staff with different roles need to learn how to enter data into the system, and use the various tools and reports in the system. Help documents can be found at - https://getjobbook.com/help

On the Dashboard, Job Book contains a number of collections (or cards) that help staff.

1. Clients
    * Collection of client data
2. Jobs
    * Collection of job data 
    * The Active Job Dashboard will display all the active Jobs in the system
    * Every Job is associated to a Client
    * Jobs have:
        * Job #
        * Client Location
        * Client Address
        * Project Name
        * Status
        * Locations (where the job will be performed)
            * Multiple locations can be created
        * Contacts
        * Project Shared Folder
        * Project Manager
            * An Employee in the system
        * Salesperson / Representative
        * Office
        * Client Project #
        * PO #
        * PO Amount
        * Subcontract #
        * DWR Billing Type - Overhead, Non-Chargeable, Fixed Price, Time & Materials
        * Invoice Type - Ticket / Inboice, Invoice
        * Invoice Line Item Type - Detailed, Summarized
        * GL Code Prefix
        * Job Categories
        * Job Scope
        * Job Scope Details
        * Order Date
        * Due Date
        * Taxes
        * Fees
        * Additional Fields
        * Notes
        * Rate Sheet
        * Billable Line Items
            * Labour Costs, Equipment and Materials, Fixed Price
        * Active

3. Task / Scheduling
    * Addon Module
    * Collection of tasks
    * Tasks are associated with a Job
4. My Tasks
    * Addon Module
    * The users specific tasks
    * There are two types of tasks: Scheduable Tasks and Unscheduable Tasks
    * Scheduable Tasks are displayed on a calendar
    * Unshceduable Tasks are displayed on an item list
5. Daily Work Records
    * Collection of DWRs / timesheets including labour cost items, and equipment & materials cost items used on a job
6. Invoices
    * Collection of invoices
7. Rate Sheets
    * Collection of Rate Sheets 
    * A Rate Sheet is a collection of line items with set rates applied to them
    * Rate Sheets are applied to a Job
    * They can also be associated to a Client such that when a Job is created that Rate Sheet will be set as the default
8. Workflow    
    * DWR Approval Backlog
        * A backlog of unapproved DWRs
    * DWR Invoice Backlog
        * A backlog of DWRs that are associated to a Job that was set to Time & Materials, that have not been invoiced
    * Expense Approval Backlog
        * A backlog of unapproved Expenses
    * Invoice Process Backlog
        * A backlog of Invoices that have not been set to proccessed
        * A place to export the Invoices to a file that an accounting system like QuickBooks or Sage can inport
9. Time & Expense Reports
    * Time Card Report
        * A report with a time range that shows all the Labour Cost Items that were created in the DWRs
    * Time Grid
        * A grid with a time range that has all the employees in the first column and the days in the other columns with their aggregated DWR hours.
    * Utilization Report
        * A report with a time range that shows all the employees and their: T&M Hrs, Fixed Price Hrs, Non-Chargeable Hrs, Overhead Hrs, Total Hrs, Utilization, Chargeability, T&M $, Fixed Price $, Non-Charge $, Toal $, Effective Rate
    * Expense Report
        A report with a time range that shows all the expenses that were created and their status
10. Cost Reports
    * Line Item Report
        * A report with a time range that shows all the Cost Items (Labour Costs, Equipment & Materials Costs) that were created in the DWRs
    * WIP Report
        * A report whith a time range that shows all the work in progress. What line items have been completed and what have been invoiced
11. Personal Reports
    * My Time Cards
        * The users time cards
    * My Expenses
        * The users expenses
12. Expenses
    * Collection of expenses the employee should be reinburced for
13. Leave Requests
    * Addon Module
    * Collection of Leave Requests
    * Leave Request Report
        * A report containing all the leave requests in the system including their status
    * Company Calendar
        A shared calendar with all the leave requests
14. Assets
    * Addon Module
    * A collection of Assets
    * An Asset can be associated with a single or multiple Line Items
    * An Asset can be associated with an Owner / Employee
    * Manage Assets
        * A report containing all the assets in the system with actions that can be applied to the asset
15. Safety
    * Addon Module
    * A meta safety system
    * Multiple collections
        * Employee Incident Reports
        * Hazards/Tailgate Meetings
        * Hazard Near Miss Reports
        * HSE INspection Forms
        * Light Vehicle Inspection
        * Policy Documentation
        * Training Records
        * Unsafe Work Refusal Forms
        * Wirness Statements
        * Worksite Observations
16. Job Maps
    * A geospacial map of all the Job Locations
    * Can be filtered by an multiple of: Job #, Status, Client Name, Client Type, Project Name, Office, Project Manager, Municipal Adress, State / Province, City, Category, Scope, Order Date, Due Date, Active, Lot, Block, Plan Number, LSD, Section Number, Township Number, Range Number, Meridian 

## Problem

The customer is a small to medium sized land survey firm. The have staff with various roles (owner, administrator, project manager, office staff, site staff). Job book has four roles: Administrator, Job Coordinator, Manager, Technician. 

We've already created help documents at https://getjobbook.com/help and we've create a YouTube video series showing the customer how to setup Job Book. 

We now want to create scripts for a YouTube video series showing the various user roles how to use Job Book.

## Goal

## Constraints

* Each script should be as short as possible as to not bore the user.
* A person will read the script and record their screen showing how to use the Job Book System
* There are some completed scripts in /Scripts/ with the remainder as stubs. 

## References

Resources:
1. [Help documentation](https://getjobbook.com/help)
2. [How to Setup Job Book Scripts](/HowToSetup/)
3. [How to Use Job Book Scripts](/Scripts/)

## Implementation Notes for LLM Agent

This section provides a detailed, step-by-step guide for building the Scripts.
