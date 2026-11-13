# SQL Fundamental for Beginners

Model, query, transform and warehouse business data with SQL in one hands-on day — every lab runs in SQLite Studio on **SG Mart**, a fictitious Singapore retail chain.

| Course detail | Information |
|---|---|
| Course code | `TGS-2026066737` |
| Programme | CASL — SkillsFuture-funded; Certificate of Achievement from Tertiary Infotech Academy Pte Ltd |
| Duration | 1 day · 8 hours (9:30 am – 6:30 pm, 1-hour lunch), assessment included |
| Registration | [View course details and register](https://www.tertiarycourses.com.sg/wsq-sql-fundamental-for-beginners.html) |
| Funding | Up to 70% course-fee funding for eligible Singapore Citizens and PRs (validity 14 Oct 2026 – 13 Oct 2027). Eligibility and terms apply — see the course page. |
| Skills Framework | Data Engineering — ICT-DIT-3005-1.1 (ICT Skills Framework) |
| Courseware version | v15 · 13 November 2026 |

## About the course

A hands-on introduction to SQL for working adults: design tables with the right data types,
constraints and keys; query and filter data; join, aggregate and group it across tables;
and map an E-R model into a data warehouse. The deck is visual; every step-by-step procedure
lives in the Learner Guide and the lab files.

## Learning outcomes

- **LO1** — Apply data modeling for business processes.
- **LO2** — Apply data processing and analysis using SQL.
- **LO3** — Apply data transformation from multiple data sources.
- **LO4** — Apply data mapping to data warehouse.

## Topics covered

| Topic | TSC mapping | Labs |
|---|---|---|
| 1 · Data Modeling | A1, A2, K1, K2 | 1 – 3 |
| 2 · Data Processing and Analysis | A3, A5, K4 | 4 – 6 |
| 3 · Data Transformation | A4, A6, K5, K6 | 7 – 9 |
| 4 · Introduction to Data Warehouse | A7, A8, A9, K3, K7 | 10 – 11 |

## Labs

Each lab is one self-contained folder: its instructions, only the tables it needs as CSV,
and `seed_sqlite.sql` / `seed_mysql.sql` that create and fill everything in one run.
Overview: [labs/README.md](labs/README.md).

| Lab | Instructions |
|---|---|
| 1 | [Lab 1 — Set Up SQLite Studio & Import the SG Mart Database](labs/lab-01-set-up-sqlite-studio-import-the-sg-mart-database/lab-01-set-up-sqlite-studio-import-the-sg-mart-database.md) |
| 2 | [Lab 2 — Create a Database and Tables](labs/lab-02-create-a-database-and-tables/lab-02-create-a-database-and-tables.md) |
| 3 | [Lab 3 — Model Data with Constraints and Keys](labs/lab-03-model-data-with-constraints-and-keys/lab-03-model-data-with-constraints-and-keys.md) |
| 4 | [Lab 4 — Query Data with SELECT](labs/lab-04-query-data-with-select/lab-04-query-data-with-select.md) |
| 5 | [Lab 5 — Filter with SQL Operators](labs/lab-05-filter-with-sql-operators/lab-05-filter-with-sql-operators.md) |
| 6 | [Lab 6 — Insert, Update and Delete Records](labs/lab-06-insert-update-and-delete-records/lab-06-insert-update-and-delete-records.md) |
| 7 | [Lab 7 — Aggregate Data with COUNT, AVG and SUM](labs/lab-07-aggregate-data-with-count-avg-and-sum/lab-07-aggregate-data-with-count-avg-and-sum.md) |
| 8 | [Lab 8 — Join Data from Multiple Tables](labs/lab-08-join-data-from-multiple-tables/lab-08-join-data-from-multiple-tables.md) |
| 9 | [Lab 9 — Group Data with GROUP BY and HAVING](labs/lab-09-group-data-with-group-by-and-having/lab-09-group-data-with-group-by-and-having.md) |
| 10 | [Lab 10 — Map an E-R Model to Database Tables (SMRT Case Study)](labs/lab-10-map-an-e-r-model-to-database-tables-smrt-case-st/lab-10-map-an-e-r-model-to-database-tables-smrt-case-st.md) |
| 11 | [Lab 11 — Author Stored Procedures for SQL Server](labs/lab-11-author-stored-procedures-for-sql-server/lab-11-author-stored-procedures-for-sql-server.md) |

The complete dataset — every CSV, the Excel workbook `SG-Mart-Mock-Data.xlsx` and a prebuilt
`sgmart.db` — is in [labs/_all/](labs/_all/). The original sample databases from earlier
versions (`world.db`, `album.db`) are kept in [labs/legacy-datasets/](labs/legacy-datasets/).

## Tools

- **SQLite Studio** — https://sqlitestudio.pl (free, cross-platform)
- **sqliteonline.com** — browser alternative, also provides an MS SQL engine for Lab 11
- **SG Mart mock dataset** — each lab folder under [labs/](labs/) carries its own CSVs and seed scripts beside the instructions; the complete set, with an Excel workbook and a prebuilt `sgmart.db`, is in [labs/_all/](labs/_all/). Also downloadable from the LMS with the course materials.

## The course dataset — SG Mart Pte Ltd

Every lab queries one continuous business story: **SG Mart Pte Ltd**, a fictitious
Singapore retail chain with 8 outlets, 42 staff, 60 loyalty members, 9 suppliers,
25 products, 180 orders and 685 order lines. Topic 4 switches to an **SMRT**
public-transport model (routes, stations, timetables, disruptions) for the
data-warehouse case study.

**Each lab is one self-contained folder** under [labs/](labs/) holding the instructions,
the data and the SQL together — `lab-NN-<slug>.md`, only the tables that lab needs as CSV
(Excel-friendly), and `seed_sqlite.sql` / `seed_mysql.sql` that create and fill everything
in one execution. Open the folder, run the seed script, follow the markdown. The complete
set, including `SG-Mart-Mock-Data.xlsx` and a prebuilt `sgmart.db`, is in
[labs/_all/](labs/_all/).

Some columns are deliberately empty (walk-in orders with no member, staff without a work
email, products without a reorder level) so `IS NULL`, `LEFT JOIN` and `COUNT()` behave
the way they do on real data. All data is invented for training and identifies no real
person or organisation.

The original sample databases from earlier versions of the course (`world.db`, `album.db`
and their SQL scripts) are kept in [labs/legacy-datasets/](labs/legacy-datasets/).

## The course dataset — SG Mart Pte Ltd

Every lab queries one continuous business story: **SG Mart Pte Ltd**, a fictitious
Singapore retail chain with 8 outlets, 42 staff, 60 loyalty members, 9 suppliers,
25 products, 180 orders and 685 order lines. Topic 4 switches to an **SMRT**
public-transport model (routes, stations, timetables, disruptions) for the
data-warehouse case study. Some columns are deliberately empty (walk-in orders, staff
without a work email) so `IS NULL`, `LEFT JOIN` and `COUNT()` behave as they do on real
data. All data is invented and identifies no real person or organisation.

## Public courseware package

| Artifact | Files |
|---|---|
| Trainer slide deck (133 slides) | [PPTX](courseware/SQL%20Fundamental%20for%20Beginners-v15.pptx) |
| Learner slides | [PDF](courseware/SQL%20Fundamental%20for%20Beginners-v15.pdf) |
| Lesson Plan | [DOCX](courseware/LP-SQL%20Fundamental%20for%20Beginners.docx) · [PDF](courseware/LP-SQL%20Fundamental%20for%20Beginners.pdf) |
| Learner Guide | [DOCX](courseware/LG-SQL%20Fundamental%20for%20Beginners.docx) · [PDF](courseware/LG-SQL%20Fundamental%20for%20Beginners.pdf) · [Markdown](LG-SQL%20Fundamental%20for%20Beginners.md) |
| Hands-on labs (11) | [labs/](labs/) |

Learners download the same materials from the LMS at **https://lms-tms.tertiaryinfotech.com**,
where the TRAQOM survey and the certificate also live. AM, PM and Assessment digital
attendance is mandatory for funded learners.

## Assessment and distribution boundary

The final assessment is **Practical Performance (PP, 70 minutes, open book)** followed by
**Oral Questioning (OQ, 20 minutes, one-to-one)**. At least 75% attendance and a result of
*Competent* are required for funding.

This public repository carries the slides, Lesson Plan, Learner Guide and labs only. The
assessment papers and answer keys, the Facilitator Guide and the Assessment Plan are
trainer-only and are distributed through Google Drive and the LMS — never through GitHub.

---

Conducted by **Tertiary Infotech Academy Pte Ltd** (UEN 201200696W) · Trainer: Dr. Alfred Ang
© 2026 Tertiary Infotech Academy Pte Ltd. All rights reserved.
