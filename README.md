# Fully-Automated-Payroll-Attendance-Management-System
System designed to streamline monthly HR operations, attendance tracking, and precise salary disbursements. Built with complex logical functions and interconnected sheets, this system minimizes manual data entry and eliminates calculation errors for business operations and accounting.

🚀 Key Features
1. Dynamic Attendance Tracking (Attendance table)
Automated Day Status: Tracks Present (P), Absent (A), Half-days (H), Holidays, and Week Offs across a dynamic 31-day monthly calendar.

Visual Data Management: Utilizes Conditional Formatting to instantly flag absences (Red) and half-days (Grey), providing a clear visual overview of workforce availability.

Auto-Aggregation: Automatically sums total payable working days per employee, seamlessly feeding this data into the salary calculation engine.

2. Comprehensive Salary Engine (Salary sheet)
Pro-Rata Salary Calculation: Calculates exact per-day salary and attendance-based base pay derived from the employee's fixed basic salary and actual days worked.

Tier-Based Allowances:

DA (Dearness Allowance): Automatically calculated at 12%.

HRA (House Rent Allowance): Conditional logic applies different HRA brackets based on location status (City vs. Non-City).

TA (Transport Allowance): Automatically calculated at 5%.

Overtime Integration: Converts inputted overtime hours into exact monetary compensation added to the gross pay.

Statutory Deductions: Automatically deducts standard compliance components including PF (12%) and ESI (0.75%) from the gross salary to arrive at the final Net Salary.

3. One-Click Salary Slip Generation (Salary slip)
Dynamic Search: Enter an Employee ID (e.g., Emp001) to instantly fetch all relevant monthly data for that specific individual.

Print-Ready Formatting: Clean, professional layout featuring company branding (Aditya Pvt. Ltd.), employee designation, detailed earnings, and deductions breakdowns.

Timestamped: Automatically pulls the current date for the "Salary Slip Print date" record.

🧠 Technical Implementation
This project showcases advanced spreadsheet architecture and data relationship management:

Lookup & Reference Functions: Heavy reliance on VLOOKUP/XLOOKUP or INDEX/MATCH to bridge data between the Attendance Table, Salary Sheet, and the final Salary Slip.

Logical & Conditional Functions: Nested IF statements to handle tiered HRA allocations (City/Non-City) and ESI/PF deduction thresholds.

Statistical Functions: COUNTIF arrays utilized in the Attendance sheet to tally specific string values (P, A, H) per row.

Data Validation: Dropdown menus and restricted inputs to maintain data integrity when querying employee records on the slip.

📂 File Structure
Payroll auto system.xlsx: The master workbook containing all three integrated modules.
(Note: Requires Microsoft Excel 2016 or newer for full formula compatibility).

📸 System Previews
1. Master Attendance Board
(Add your image_563c5c.jpg here in GitHub by linking it: ![Attendance](path/to/image_563c5c.jpg))

2. Automated Payroll Processing
(Add your image_563f07.jpg here in GitHub by linking it: ![Salary Sheet](path/to/image_563f07.jpg))

3. Generated Employee Payslip
(Add your image_563f3e.png here in GitHub by linking it: ![Payslip](path/to/image_563f3e.png))

🛠️ How to Use
Initialize the Month: Update the Month and Year on the Attendance table sheet.

Log Daily Attendance: Enter P, A, or H for each employee daily. The TOTAL DAY metrics will update live.

Review Overtime & Allowances: Navigate to the Salary sheet. Input any specific Overtime hours or location changes (City/Non-City). All Gross, Deductions, and Net calculations will finalize instantly.

Print Slips: Go to the Salary slip sheet, type the target Emp-Id into cell C5, and print or export the sheet as a PDF.
