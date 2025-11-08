# Kimia Farma - Business Performance Analysis (2020-2023)
## 1. Project Overview
This repository contains the technical outputs for the Final Project from the Big Data Analytics Virtual Internship Program, hosted by Rakamin Academy and PT. KIMIA FARMA, TBK.

The goal of this project was to analyze the business performance of Kimia Farma over a four-year period (2020-2023). This project covers the entire data analytics workflow, from processing raw data in Google BigQuery to building an interactive executive dashboard in Google Looker Studio.

## 2. Tools Used
- Data Warehouse & Processing: Google BigQuery
- Query Language: SQL
- Data Visualization: Google Looker Studio
- Data Modeling (ERD): QuickDBD

## 3. Methodology & Project Workflow
This project was divided into three main phases as outlined in the final presentation:

### Phase 1: Data Setup & Import
• Four raw CSV datasets (kf_final_transaction, kf_product, kf_kantor_cabang, kf_inventory) were imported into a dedicated kimia_farma dataset within Google BigQuery.
• The Auto-detect schema feature was used during import to ensure correct data typing for all columns.

### Phase 2: Data Modeling & Transformation (SQL)
- An Entity-Relationship Diagram (ERD) was designed to map the architecture and relationships between the source tables.
- A comprehensive SQL query was written to perform the ETL process. This query (included in this repository) uses Common Table Expressions (CTEs) to:
  - Join data from the three primary tables.
  - Engineer new features like persentase_gross_laba using CASE...WHEN logic based on business rules.
  - Create (CREATE TABLE) a final, unified analysis table (tabel_analisa) ready for visualization.

### Phase 3: Visualization & Analysis (Looker Studio)
- The final tabel_analisa in BigQuery was connected to Google Looker Studio as the single source of truth.
- An interactive dashboard was built to visualize KPIs, trends, and actionable insights.

## 4. Final Result: Business Performance Dashboard
This interactive dashboard summarizes all key findings, tracking KPIs such as Total Profit, Revenue (YoY), Provincial Performance, and Product Analysis.

➡️ Click here for the live Looker Studio Dashboard: https://lookerstudio.google.com/u/0/reporting/ac747559-2fe7-4cb8-8c7b-53e547a46e9e/page/z2ydF
