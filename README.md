# ⚡ Energy Utility BI Project

## 📊 Overview
End-to-end Business Intelligence solution using:
SQL Server + SSIS + SSAS + Excel + Power BI

## 🏗 Architecture
<img width="4550" height="1168" alt="architecture png" src="https://github.com/user-attachments/assets/01ab6f93-01e6-454f-bda7-e665587eb831" />


OLTP → Staging → Data Warehouse → SSAS → Dashboards

## 🚀 Features
- 393K+ records processed
- Star Schema (6 dimensions, 2 facts)
- SCD Type 2 implementation
- Incremental ETL with Watermark
- SSAS Cube with KPIs & MDX
- Excel & Power BI dashboards

## 🛠 Tech Stack
- SQL Server
- SSIS (SSDT)
- SSAS Multidimensional
- Excel
- Power BI

## 📂 Project Structure
Energy-Utility-BI-Project/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── docs/                              # Full documentation (your big guide)
│   ├── Project_Overview.pdf
│   ├── Architecture_Diagram.png
│   ├── Data_Flow_Diagram.png
│   └── Setup_Guide.md
│
├── database/
│   ├── OLTP/
│   │   ├── 01_OLTP_Schema.sql
│   │   └── 02_OLTP_SeedData.sql
│   │
│   ├── Staging/
│   │   ├── 03_Staging_Schema.sql
│   │   └── 06_Package1_Staging_SPs.sql
│   │
│   ├── DataWarehouse/
│   │   ├── 04_DW_Schema.sql
│   │   ├── 07_Package2_Dims_SPs.sql
│   │   └── 08_Package3_Facts_SPs.sql
│   │
│   ├── DataMart/
│   │   ├── 05_DataMart_Schema.sql
│   │   └── 09_Package4_DataMart_SPs.sql
│   │
│   └── verification/
│       ├── staging_checks.sql
│       ├── dw_checks.sql
│       └── datamart_checks.sql
│
├── etl/                               # SSIS packages
│   ├── Package1_OLTP_to_Staging.dtsx
│   ├── Package2_Dimensions.dtsx
│   ├── Package3_Facts.dtsx
│   ├── Package4_DataMart.dtsx
│   └── Master_ETL.dtsx
│
├── ssas/
│   ├── EnergyUtility_SSAS.sln
│   ├── Cubes/
│   ├── Dimensions/
│   ├── DataSources/
│   └── MDX/
│       └── 12_SSAS_MDX_Calculations.sql
│
├── dashboards/
│   ├── excel/
│   │   └── EnergyUtility_Dashboard.xlsx
│   │
│   ├── powerbi/
│   │   ├── EnergyUsage_Report.pbix
│   │   └── Billing_Report.pbix
│
├── guides/                            # Step-by-step instructions
│   ├── 10_SSIS_Wiring_Guide.txt
│   ├── 11_SSAS_Setup_Guide.txt
│   ├── 13_Excel_Dashboard_Guide.txt
│   └── 14_PowerBI_Dashboard_Guide.txt
│
├── automation/
│   ├── sql_agent_job.sql
│   └── ssas_process.xmla
│
└── assets/                            # Images for README
    ├── architecture.png
    ├── star_schema.png
    ├── dashboard_preview.png

## ⚙️ Setup Instructions
1. Run SQL scripts (order provided)
2. Build SSIS packages
3. Deploy SSAS cube
4. Run SQL Agent job

## 📸 Dashboard Preview
(images)

## 📈 Business Value
- Energy usage insights
- Billing & collection tracking
- Risk & anomaly detection
