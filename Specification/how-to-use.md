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

The customer (specifically, project managers in the company) thinks the above reports are not usable for quickly reviewing time that people have submitted to their projects, and would like more of a timeline view where they can see for each relevant employee, a breakdown of hours per project/line item.

This is the quote from the customer, take it with a grain of salt:
> I have attached an example image of a timesheet view one of the team have sent me. They would like to have a new report display screen that lets them view the submitted timeshet entries like this, so they can easily see over a week period who has submitted what hours each day, they say this view would save them alot of time when reviewing their own submissions or for the manager's who are reviewing a site team's submissions. Maybe we would need two different viewer tier's for this report, for every site staff they can view this layout report for themselves only to review their entries for the week and for managers/admin they can filter by job (displays this report view for all entries from any staff against this job) and a second tier filter if they want to view for a specific staff member on that project (so only can second tier filter by a staff member assigned in back end on the job not able to see for any staff in the company). 

The screenshot they sent us is available [here](/reference/clients/benchmarksurveys/timepro-screenshot.png), it should be used for inspiration, but we'll be going above and beyond.

## Goal

## Constraints

* Hours are always displayed in a calendar-style that is easy for users to visualize, specifically **one column per date**.
* Kendo UI (jQuery) is available and should be used for controls where possible.
* Performance is a major consideration.
  * Use function-backed datatables for Jobs, Employees, and aggregated time.
  * Do not query raw DWR items directly. Use PostgreSQL functions exposed as datatables that accept `start`/`end` and return optimized rows, queried via `clientSupport.js`.
* Use async/await instead of promises

## Sizing and Responsiveness

The Time Inspector UI is optimized for smaller screens while maintaining readability on desktop. Styling is scoped under a root wrapper class to avoid affecting other views.

- Root wrapper: The HTML container uses `.ti-root`. All CSS selectors are prefixed with `.ti-root` to scope styles locally.
- Compact grid defaults: Grid typography runs slightly smaller than theme defaults.
  - Base: font-size ≈ 0.95em, line-height ≈ 1.35; cell padding ≈ 0.35em 0.5em.
  - Kendo toolbar and buttons: reduced internal padding for a denser layout.
- Breakpoints: Two responsive tiers adjust typography and spacing.
  - ≤ 800px: font-size ≈ 0.9em; cell padding ≈ 0.3em 0.45em; buttons and grid toolbar padding reduced; date pickers shrink to ~130px width.
  - ≤ 480px: font-size ≈ 0.85em; cell padding ≈ 0.25em 0.4em; filter controls stack to one column; date pickers shrink to ~110px width.
- Filter bar layout: Uses a CSS grid with labels aligned to the baseline of inputs so wrapped content (including warnings) stays visually aligned. On small screens, inputs wrap and labels become left-aligned.
- Date range warning: The `#ti-date-warning` element is responsive and wraps as needed.
  - On narrow widths, it flows to a full-width line beneath the date controls to prevent overflow.
  - Text updates at runtime to reflect the configured `MAX_RANGE_DAYS` value.
- Line Item column width: The “Line Item” column narrows on smaller screens to preserve horizontal space for date columns.
  - Default width: 200px.
  - ≤ 800px viewport: 125px.
  - Implementation details: implemented via shared helpers `getResponsiveWidth()` and `setupResponsiveColumnWidth()` in `clients/benchmarksurveys/app/time-inspector-common`. The grid initializes the column width with `getResponsiveWidth(800, 125, 200)` and keeps it in sync across viewport changes via `setupResponsiveColumnWidth(grid, { field:'lineItemName', breakpoint:800, narrow:125, wide:200, resizeNs })`.
- Date columns and totals: Date columns remain fixed width to support consistent scanning; totals are right-aligned and bolded for emphasis.

Where to change sizes:

- CSS compactness and breakpoints: `public/clients/benchmarksurveys/app/time-inspector.html` under the `<style>` block scoped to `.ti-root`.
- Line Item column breakpoint/widths: `public/clients/benchmarksurveys/app/time-inspector.js` in `loadData()` (uses `tiShared.getResponsiveWidth()` and `tiShared.setupResponsiveColumnWidth()` from the common module).

## Stories

The creation of a new 'Time Inspector' report for Job Book that will allow project managers to answer the following questions:

1. For a date range, show me hours for projects that I'm interested in, broken down by employee/project/line item.
2. For a date range, show me hours for a set of specific employees, broken down by employee/project/line item.
3. Let me filter to a specific set of projects.
4. Let me filter to a specific set of employees.

## Filter Specification

This is the most complex part of the application, allowing the user to filter jobs and employees either specifically or using a role- and range-aware "smart" mode.

- Project manager model: Jobs now support multiple PMs.
  - Primary PM is stored as `job.project_manager_id`.
  - Additional PMs are stored as rows in `collection_data_graph` with `predicate='additionalProjectManagers'` and `obj_id=<employee_id>`.
- "My Jobs (PM)": A job is considered “mine” when the current employee is either the primary PM or listed as an additional PM, and the job has DWR/Leave activity in the selected date range.
  - Backend source of truth: `benchmarksurveys.my_jobs_active_in_date_range(principal_id, realm_id, data)`.
- Employees relevant to jobs: Given a job, relevant employees are those with DWR time or Leave Requests on that job within the date range.
- Smart jobs modes presented to the user:
  - My Jobs (PM): intersect job list with `my_jobs_active_in_date_range`. This is the default and the only option for non-admin, non-office users.
  - All Jobs: shows all jobs with in-range activity; available only to roles `Administrator` and `Office Staff`.
- All jobs are searchable by job number, project name, or client name. All records (including Jobs) have UUID identifiers.
- All employees are searchable by name and identified by UUID.
- Employee filter coherence: The employee list filters by the “effective job IDs”.
  - If jobs are selected: list only employees active on those jobs.
  - If no jobs are selected and Smart Filter is “My Jobs (PM)”: list only employees active on the user’s PM jobs.
  - Otherwise: list all employees active in-range.

## References

Resources:

## References

Resources:

1. [Generic Report Framework](/public/components/page/reportComponentFactory.js)
2. [Client Support](/public/js/clientSupport.js)

Sample reports:

1. Leave Request Report
  * [js/viewmodel](/public/clients/jobbook/app/leave-request-report.js) [html/template](/public/clients/jobbook/app/leave-request-report.html)
2. Time Grid (dynamic column implementation)
  * [Extension](/public/clients/jobbook/app/time-grid-extension.js)

## Implementation Notes for LLM Agent

This section provides a detailed, step-by-step guide for building the Time Inspector report.

### 1. Frontend Development

The frontend will be built using the existing report framework and Kendo UI components.

#### 1.1. UI Components (HTML Template)

Create an HTML file (e.g., `/public/clients/benchmarksurveys/app/time-inspector.html`) with the following Kendo UI widgets:

1.  **Date Range Filter:**
    *   Start Date: `<input id="ti-start-date" />` (Kendo DatePicker)
    *   End Date: `<input id="ti-end-date" />` (Kendo DatePicker)
    *   Quick Range Presets: `<div class="ti-quick-chips"></div>` (buttons rendered by JS: Last 7/14/31 days, This week, Last week, This month, Last month).
    *   Default to the last 7 days.

2.  **Job Filter:**
    *   **Smart Filter:** `<input id="ti-job-smart-filter" />` (Kendo DropDownList)
        *   Data Source: `[{ text: "My Jobs (PM)", value: "pm" }, { text: "My Jobs (Hours)", value: "hours" }, { text: "All Jobs", value: "all" }]`
        *   Default to "My Jobs (PM)".
    *   **Specific Jobs:** `<select id="ti-job-selector" multiple="multiple"></select>` (Kendo MultiSelect)
        *   Enable server filtering, searching by job number, project name, or client name.
        *   This will be populated based on the Smart Filter selection.

3.  **Employee Filter:**
    *   **Specific Employees:** `<select id="ti-employee-selector" multiple="multiple"></select>` (Kendo MultiSelect)
        *   Enable server filtering, searching by employee name.
        *   The data source for this should be dynamically populated based on the selected jobs.

4.  **Summary Bar + Collapsible Filters (mobile-first):**
    *   Summary container: `<div class="ti-summary-bar">` shows a compact textual summary (e.g., `7d • My jobs • 3 jobs • 2 employees`).
    *   Toggle: `<button class="ti-summary-toggle">Filters</button>` collapses/expands the filter panel on small screens (≤600px).
    *   Behavior: On small screens the filter panel is collapsed by default and the date row (inputs + chips) becomes horizontally scrollable.

5.  **Report Display:**
    *   `<div id="ti-grid"></div>` (Kendo Grid)
    *   This grid will be initialized with dynamic columns.

#### 1.2. ViewModel Logic (JavaScript)

Create a JavaScript file (e.g., `/public/clients/benchmarksurveys/app/time-inspector.js`) that will contain the view model logic.

1.  **Initialization:**
    *   Initialize Kendo UI widgets defined in the HTML (date pickers, job dropdown/multiselect, employee multiselect, grid).
    *   Build quick-range chips into `.ti-quick-chips` and wire click handlers.
    *   Initialize the summary bar and the collapse toggle (uses `aria-expanded`).

2.  **Filter Interaction Logic (Auto-load):**
    *   **`ti-job-smart-filter.change` event:**
        *   Role-gated options: "All Jobs" is available only to `Administrator` and `Office Staff`; otherwise only "My Jobs (PM)" is shown and enforced.
        *   Get the selected value (e.g., "My Jobs (PM)" or "All Jobs").
        *   Load jobs for the range from the `jobs_active_in_date_range` datatable.
        *   If "My Jobs (PM)" is selected, intersect with IDs from `my_jobs_active_in_date_range` for the range.
            - Notes: `my_jobs_active_in_date_range` returns only jobs where the current user is a Project Manager (either primary `project_manager_id` or listed in `additionalProjectManagers`) and the job has DWR/Leave activity in-range.
        *   Set the Kendo MultiSelect (`#ti-job-selector`) data source to the resulting list, clear selection, update the summary, and auto-load results.
        *   Changing this filter also refreshes the Employee selector to keep employees in sync with the effective job set.
    *   **Pre-populating Employee Filter:**
        *   Load employees for the range from the `employees_active_in_date_range` datatable.
        *   The employee list filters dynamically by the "effective job IDs":
            - If one or more jobs are selected, show only employees active on those jobs in-range.
            - If no jobs are selected and Smart Filter is "My Jobs (PM)", show only employees active on the user’s PM jobs (from `my_jobs_active_in_date_range`).
            - Otherwise (All Jobs, no jobs explicitly selected), show all employees active in the range.
        *   When the filter reduces the list, any selected employees not present are automatically deselected (pruned) to avoid invalid selections.
    *   **Date pickers change:**
        *   Start-date changes “preserve duration” by automatically shifting the end date to keep the same inclusive span (clamped to the max range).
        *   End-date changes freely and update the stored duration for subsequent start-date moves.
        *   Both date changes trigger range validation, chip active-state refresh, summary update, and auto-load.
    *   **Quick-range chips click:**
        *   Set start/end based on the preset, clamp to max, update duration, validate, refresh chip active state, update the summary, and auto-load.

3.  **Data Loading (Auto):**
    *   On any relevant change (dates, chips, job smart filter, job selections, employee selections), gather current filter values and load data.
    *   Query aggregated rows via datatable:
        - Use `time_inspector_timecards` for general cases.
        - Optionally use `time_inspector_timecards_my_jobs` when Smart Filter is "My Jobs (PM)" to reduce payload by server-filtering to PM-owned jobs.
    *   Apply optional client-side filtering for selected jobs/employees, then build/refresh the Kendo Grid.

4.  **Kendo Grid Configuration:**
    *   The data returned from the API will be a flat list of records. You need to transform it for the grid.
    *   The grid needs **dynamic columns**. One column for each date in the selected range.
    *   **Static Columns:** `Employee`, `Job`, `Line Item`.
    *   **Dynamic Columns:** `YYYY-MM-DD`, `YYYY-MM-DD`, ...
    *   **Grouping:** Group by Employee, then Job. `Line Item` remains as the leaf row within each Job group.
    *   **Columns:** `Employee` and `Job` columns exist but are hidden and used for grouping; `Line Item` is visible; one dynamic column per date; a `Total` column at the end.
    *   **Sorting:** The grid allows sorting overall, but sorting is disabled on all dynamic date columns and on the `Total` column to avoid resorting by day-of-range.
    *   The `time-grid-extension.js` reference is no longer required; dynamic columns are built via a shared helper (`buildDateColumns`) from `clients/benchmarksurveys/app/time-inspector-common`.

#### 1.3. Max Date Range Enforcement

To protect performance and keep the grid usable, the report enforces a maximum inclusive date range.

- Source of truth: `MAX_RANGE_DAYS` constant in `/public/clients/benchmarksurveys/app/time-inspector.js`.
- Inclusive logic: A range is invalid when `(diffDays + 1) > MAX_RANGE_DAYS`. For example, `2025-01-01`–`2025-01-31` counts as 31 days.
- UI behavior (live while picking dates): Centralized in a shared date-range controller (`createDateRangeController` in `clients/benchmarksurveys/app/time-inspector-common`). Its `onValidityChange` callback:
  - Shows/hides `#ti-date-warning` when the range exceeds the max.
  - Disables/enables the job smart filter, job selector, and employee selector while invalid (Time Inspector view); `my-time-inspector` only toggles the warning.
  - Date pickers remain enabled so the user can correct the range.
- Load guard: `loadData()` re-checks the range and aborts if it exceeds `MAX_RANGE_DAYS` (defense in depth).
- Warning text: On init, the JS updates `#ti-date-warning` to “Please specify a time range of <MAX_RANGE_DAYS> days or less.” so the HTML stays in sync with the constant.

#### 1.4. Quick Range Presets (Chips)

- Presets include: Last 7 days, Last 14 days, Last 31 days, This week, Last week, This month, Last month.
- Active-state highlight reflects whether the current start/end exactly match a preset.
- Week presets use the browser locale’s week boundaries; adjust to ISO weeks if needed.
- Clicking a chip sets the date range (clamped to max) and triggers validation, summary update, and data load. Chips are built via a shared helper (`buildQuickRangeChips` in the common module) which ensures:
  - Initial active chip prefers the first matching preset (“Last 7 days”) when multiple presets match the same range.
  - After interaction, if multiple presets match, the last clicked preset retains precedence.

#### 1.5. Preserve Duration Behavior

- When the start date changes, the end date auto-adjusts to preserve the previous inclusive duration (default 7 days), clamped to `MAX_RANGE_DAYS`.
- When the end date changes, the duration updates freely and becomes the new preserved span for subsequent start changes.
- This reduces two-step adjustments while keeping end-date edits intuitive.

## 2. Architecture Updates (State + Data Flow)

The Time Inspector views now use a small viewmodel (VM) as the single source of truth for range, filters, available options, and selections. Kendo DataSources remain for loading indicators but are driven by VM events and promises.

- ViewModel ownership: `public/clients/benchmarksurveys/app/time-inspector.js`
  - Owns: date range, smart job filter mode (`my|all`), available jobs/employees for the current range, selected jobs/employees.
  - Computes: effective job IDs (selected list or “my jobs” fallback when mode is `my`).
  - Preserves/prunes: on range or filter changes, selections are pruned to still-valid values.
  - Versioning: async fetches capture a version and apply only if still current (prevents stale applies, no timeouts or locks).
  - Events: `jobsLoading`, `employeesLoading`, `jobsUpdated`, `employeesUpdated`, `selectionChanged`, `stateReady`.
  - Smart filter options: exposed via `vm.getSmartFilterOptions()` based on user permissions; UI binds to this rather than hardcoding.

- Event-driven DataSources (thin):
  - On `jobsLoading`/`employeesLoading`, handlers call `dataSource.read({ wait })`, where `wait` is a VM-provided promise for that transaction.
  - In each `transport.read`, await `options.data.wait` (if provided), then call `options.success(...)`. Falls back to `vm.when...Available()`.
  - UI selections are set from `...Updated` events with a guard (`isProgrammaticUpdate`) to avoid feedback loops.

- Grid loading: Subscribed to `stateReady` and `selectionChanged` to coalesce a single `loadData()` call per coherent change. `loadData()` reads all inputs from the VM (range, mode, selections), not directly from controls.

- Summary bar: Computes text from VM state (range, mode, selection counts). Updated on VM events rather than control change handlers.

### 2.1. Selection Preservation

- Jobs: After a date range or smart filter change, previously selected jobs are preserved when still present in the new available set, otherwise pruned.
- Employees: The available employee list is dynamically filtered by the effective job IDs; selected employees not present are pruned.
- Result: Changing range or filter no longer clears selections; best-effort preservation maintains user intent while keeping selections valid.

### 2.2. My Time Inspector Simplification

- `public/clients/benchmarksurveys/app/my-time-inspector.js` now uses a minimal VM that only owns the date range and emits `rangeChanged` and `stateReady`.
- Summary and grid load derive from VM range (not pickers). Grid DataSource still shows progress while fetching jobs (for labels) + user time.

### 2.3. Range Controller (Future Consideration)

- The existing `createDateRangeController` remains as a thin binding layer for pickers/chips (preserve-duration UX, validation callbacks).
- Longer-term, range math and validity can move into the VM with events like `rangeValidityChanged`, leaving the controller purely for UI wiring.

#### 1.6. Collapsible Filters and Summary Bar

- On ≤600px, the filter panel collapses by default and a summary bar is shown above it.
- The summary displays duration and selected filter context (e.g., “7d • My jobs • 3 jobs • 2 employees”).
- A pill-style “Filters” button (with funnel icon + chevron) toggles panel visibility; chevron rotates according to `aria-expanded`.
- The date row (inputs + chips) becomes horizontally scrollable to keep the panel compact.

How to change the maximum:

- Edit `MAX_RANGE_DAYS` in `time-inspector.js`.
- No HTML change is needed unless the `#ti-date-warning` element ID is renamed.
- Optional: adjust the default date range (currently last 7 days) via the two `kendoDatePicker` initial values if desired.

### 2. Data Access (Current)

The report uses function-backed datatables via `clientSupport.queryDataTable` (no custom HTTP endpoints). All queries are scoped by `start`/`end` and return only the columns needed by the UI. Leave requests are included as phantom DWRs everywhere relevant.

#### 2.1. Datatables

- `time_inspector_timecards` (benchmarksurveys.time_inspector_timecards)
  - Purpose: Aggregated time source for the grid. One row per `date` + `job_id` + `employee_id` + `lineitem_name` with `hours` summed.
  - Includes: DWR time and Leave Requests (phantom DWRs) for the range.
  - Columns: `date`, `job_id`, `employee_id`, `lineitem_name`, `hours`.
  - Example: `$select=date,job_id,employee_id,lineitem_name,hours&start=YYYY-MM-DD&end=YYYY-MM-DD&$orderby=date,employee_id,job_id,lineitem_name`.

- `time_inspector_timecards_my_jobs` (benchmarksurveys.time_inspector_timecards_my_jobs)
  - Purpose: Same as `time_inspector_timecards` but restricted to jobs from `my_jobs_active_in_date_range` for the principal and range.
  - Columns: `date`, `job_id`, `employee_id`, `lineitem_name`, `hours`.
  - Example: `$select=date,job_id,employee_id,lineitem_name,hours&start=YYYY-MM-DD&end=YYYY-MM-DD&$orderby=date,employee_id,job_id,lineitem_name`.

- `jobs_active_in_date_range` (benchmarksurveys.jobs_active_in_date_range)
  - Purpose: Jobs with activity in range (via DWRs or Leave Requests).
  - Columns: `job_id`, `job_number`.
  - Example: `$select=job_id,job_number&start=YYYY-MM-DD&end=YYYY-MM-DD&$orderby=job_number`.

- `my_jobs_active_in_date_range` (benchmarksurveys.my_jobs_active_in_date_range)
  - Purpose: Job IDs considered “My Jobs (PM)” for the current principal in range. Includes jobs where the user is a Project Manager (either primary `project_manager_id` or listed in `additionalProjectManagers`) and the job has DWR/Leave activity in-range.
  - Columns: `job_id`.
  - Example: `$select=job_id&start=YYYY-MM-DD&end=YYYY-MM-DD`.

- `employees_active_in_date_range` (benchmarksurveys.employees_active_in_date_range)
  - Purpose: Employees with activity in range (via DWRs or Leave Requests).
  - Columns: `employee_id`, `employee_name`, `job_ids` (array of job UUIDs the employee was active in during the range).
  - Example: `$select=employee_id,employee_name,job_ids&start=YYYY-MM-DD&end=YYYY-MM-DD&$orderby=employee_name`.

#### 2.2. Frontend usage

- Jobs dropdown: Loads from `jobs_active_in_date_range`; when “My Jobs” is selected, intersects with IDs from `my_jobs_active_in_date_range`.
- Employees dropdown: Loads from `employees_active_in_date_range` (falls back to realm users if unavailable).
- Main grid data: Loads from `time_inspector_timecards` (or `time_inspector_timecards_my_jobs` when Smart Filter is “My Jobs (PM)”) for the date range, then applies optional client-side filters for selected `jobIds` and `employeeIds`.
- Employee list respects the same "effective job IDs" used for the main grid and prunes selections that fall out of scope when filters change.

#### 2.2.2. Effective Job Resolution (Frontend)

- The UI centralizes job selection semantics via a resolver to keep behavior consistent across components:
  - Inputs: Smart Filter mode, user roles, explicit job selections, and `my_jobs_active_in_date_range`.
  - Output: `{ jobIds, useMyJobs }` where:
    - If explicit jobs selected: `jobIds` are those selections.
    - Else if Smart Filter is "My Jobs (PM)": `jobIds` are the user’s PM jobs in-range; `useMyJobs = true`.
    - Else: `jobIds` is undefined (no restriction); `useMyJobs = false`.
  - Consumers: employee dropdown filtering and main grid data fetch.

See `/public/clients/benchmarksurveys/app/time-inspector.js` for concrete queries and ordering.

#### 2.2.1. Shared Modules (Frontend)

- Common UI helpers: `clients/benchmarksurveys/app/time-inspector-common`
  - Date utils: `inclusiveDays`, `clampDurationDays`, `normalizeDateInput`.
  - Query helpers: `promisify`, `createQueuedQuery` (queueing wrapper for datatable calls).
  - UI scaffolding: `buildQuickRangeChips`, `buildSummaryCollapse`, `createDateRangeController`.
  - Grid helpers: `getResponsiveWidth`, `setupResponsiveColumnWidth`, `buildDateColumns`.
  - Excel: `sanitizeSheetRows`.

### 2.3. Grid Behavior and Export (Current)

- Locked columns: `Employee`, `Job`, and `Line Item` are locked to the left; `Employee` and `Job` are hidden and used only for grouping labels.
- Dynamic date columns: Generated for each day in the selected range, header shows `ddd M/d` (e.g., `Tue 1/14`). Sorting is disabled on these columns.
- Totals: A `Total` column sums row values across all date columns; sorting is disabled on this column as well.
- Aggregates and group footers: Every numeric column participates in `sum` aggregates. Group footers display only at the `Employee` level; secondary blank footers are suppressed in the DOM.
- Number formatting: Numeric cells are right-aligned and formatted to two decimals in both the grid and exported workbook.
- Excel export: Toolbar provides Excel export; filename includes the selected date range as `time-inspector-YYYYMMDD-YYYYMMDD.xlsx`. The export routine uses a shared sanitizer (`sanitizeSheetRows`) to strip HTML from templates, coerce numeric strings to numbers, apply `#,##0.00` format, and (for Time Inspector) drop empty group-footer rows.

### 2.4. Caching and Range-Scoped Queries

- Per-range caching: Jobs, “My Jobs”, and Employees are cached in-memory for the currently selected date range only; caches invalidate automatically when the range changes.
- Serialized datatable calls: Appends `clientSupport.queryDataTable` requests to a short queue to mitigate overlapping calls and preserve progress indicators.
- Defaults: Date pickers initialize to the last 7 days; the max inclusive range is enforced via `MAX_RANGE_DAYS` (currently 31) with live UI validation and disabled controls when exceeded.