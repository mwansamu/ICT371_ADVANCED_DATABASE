# ICT371 Advanced Database — SQL submission files

**Student:** Mwansa Mubanga  
**Student number:** 202405690

This folder contains one SQL script for each of the ten questions in the ICT371 Advanced Database assignment.

## Files
- `Question_01_Pharmacy_Stock.sql`
- `Question_02_University_Fee_Payments.sql`
- `Question_03_Library_Returns.sql`
- `Question_04_Clinic_Appointments.sql`
- `Question_05_Hostel_Allocation.sql`
- `Question_06_Monthly_Payroll.sql`
- `Question_07_Water_Billing.sql`
- `Question_08_Transport_Fleet.sql`
- `Question_09_Maize_Deliveries.sql`
- `Question_10_Scholarship_Assessment.sql`

## Important running instructions
1. Create a separate PostgreSQL database for each question, or run each script in a clean database/schema. Some questions reuse table names such as `students`; do not run all scripts in the same database.
2. Run each script in pgAdmin Query Tool from top to bottom.
3. The seed `INSERT` and `CALL` statements are intended for a fresh database. Do not rerun them on a database that already contains the sample rows, because that can duplicate data or hit unique constraints.
4. Review the output of each `EXPLAIN` query. PostgreSQL may choose a sequential scan for tiny sample tables; the index is still created. If your lecturer requires an index scan to be shown, you can temporarily run `SET enable_seqscan = OFF;` before the matching `EXPLAIN`, then run `RESET enable_seqscan;`.
5. Each question's final comments specify the pgAgent schedule and SQL command for its scheduled job. The stored procedure alone does not create the scheduled job. Create the job in pgAdmin/pgAgent and verify its schedule and run history.
6. These scripts are implementation drafts based on the assignment brief. Run and verify each question in PostgreSQL before submitting; adapt any sample dates or seed values if your lecturer gave additional instructions.
