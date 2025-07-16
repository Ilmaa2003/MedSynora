# 🧠 *MedSynora Data Warehouse Project*

## 📌 *Project Overview*

The **MedSynora Data Warehouse (DW)** is designed to integrate and centralize healthcare data from various structured sources. It supports efficient medical analytics and reporting by adopting best practices in **dimensional modeling**, **ETL development**, and **business intelligence visualization**.

> 📊 *Dataset Source:*
> [Medsynora DW on Kaggle](https://www.kaggle.com/datasets/mebrar21/medsynora-dw)

---

## 🎯 *Project Objectives*

* ✅ Consolidate data from multiple transactional systems and formats (CSV, SQL, Excel, XML, JSON)
* ✅ Design and implement a **Galaxy Schema** to model hospital operations
* ✅ Build modular and reusable **ETL pipelines** using **Apache Hop**
* ✅ Construct and manage the warehouse in **SQL Server Management Studio (SSMS)**
* ✅ Enable responsive and insightful **visualizations via Power BI**

---

## 🧱 *Data Model Structure*

### 🗂️ *Fact Tables*

* `FactEncounter`
* `FactTreatment`
* `FactLabTests`
* `FactVitals`
* `FactCost`
* `FactProcedures`
* `FactPatientHealthService`

### 🧾 *Dimension Tables*

| Table Name             | Format |
| ---------------------- | ------ |
| `DimPatient`           | SQL    |
| `DimDoctor`            | CSV    |
| `DimDisease`           | XML    |
| `DimChronicDisease`    | Excel  |
| `DimRoom`              | CSV    |
| `DimDate`              | SQL    |
| `DimSpecialTest`       | JSON   |
| `DimTreatment`         | JSON   |
| `DimAdditionalService` | XML    |
| `DimAllergy`           | Excel  |
| `DimInsurance`         | CSV    |

### 🔗 *Bridge Tables (CSV Format)*

* `Patient_ChronicDisease`
* `Patient_Allergy`
* `BridgeEncounterDoctor`
* `BridgeEncounterAdditionalService`

### 🧬 *Schema Type*

* **Galaxy Schema (Fact Constellation):**
  Multiple fact tables connected through shared dimensions, supporting flexible and comprehensive analysis.

---

## 🔄 *ETL Workflow*

### 1️⃣ *Extract*

* Retrieve data from various structured sources (SQL, CSV, Excel, XML, JSON)

### 2️⃣ *Transform*

* Clean and normalize data
* Address null values, duplicates, and type mismatches
* Apply business logic and generate surrogate keys

### 3️⃣ *Load*

* Load transformed data into SQL Server fact and dimension tables
* Maintain referential integrity and optimize performance through indexing

> 💡 *ETL pipelines are built using Apache Hop, offering visual workflows and component reusability.*

---

## 🛠️ *Tools & Technologies*

| Category             | Tools                      |
| -------------------- | -------------------------- |
| *Database*           | SQL Server (SSMS)          |
| *ETL Tool*           | Apache Hop                 |
| *BI & Visualization* | Power BI                   |
| *Modeling*           | diagrams.net (Draw\.io)    |
| *Data Formats*       | CSV, Excel, XML, JSON, SQL |

---

## 📊 *Power BI Dashboards*

* *Patient Insights Dashboard*
* *Patient Condition Analytics*
* *Clinical Encounters & Diagnostics*
* *Cost, Insurance & Service Utilization*

---

## 📎 *Key Notes*

* MedSynora DW simulates real-world healthcare data integration using heterogeneous formats
* Supports analytics for operations, clinical performance, and strategic planning
* Promotes reusability, scalability, and data quality in healthcare BI environments
