# 🏡 Airbnb Booking Data Pipeline with Snowflake & dbt

My Airbnb Data Engineering project! This end-to-end pipeline showcases how raw booking data is transformed into a reliable analytics-ready data warehouse using modern data stack tools like **Snowflake** and **dbt**. The project highlights best practices in data modeling, testing, documentation, and BI integration.

---

## 🚀 Project Overview

This project simulates a real-world data pipeline for Airbnb bookings. It demonstrates how raw data can be transformed into meaningful insights by applying structured data modeling principles, robust testing, and seamless BI integration.

### ✅ Objectives

- Ingest and manage Airbnb raw booking data in **Snowflake**.
- Build a scalable and modular transformation workflow using **dbt**.
- Implement robust **testing**, **documentation**, **logging**, and **macros**.
- Integrate with BI tools using **dbt exposures** for complete observability.

---

## 🏗️ Architecture & Stack

| Component        | Tool/Technology      |
|------------------|----------------------|
| Data Warehouse   | Snowflake            |
| Transformation   | dbt (Data Build Tool)|
| Testing          | dbt tests (Singular & Generic), dbt-expectations |
| Utilities        | dbt-utils, custom macros |
| BI Integration   | dbt Exposures (for Tableau/Looker/Power BI etc.) |

---

## 🔧 Features Implemented

- 📂 **Source Freshness & Versioning**  
- 📊 **Dimensional Modeling** (Kimball-style)
- 🔁 **Incremental Models**  
- 📌 **Custom Macros** for code reuse  
- 📘 **YAML-based Documentation**  
- 🧪 **Testing**: Singular, Generic, Expectations  
- 🎯 **Exposures**: Track lineage from source to BI layer  
- 📈 **BI Integration Ready**  
- ✅ **CI/CD Compatible Structure**

---

## 🛠️ Installation & Setup

> ✅ Prerequisites:  
> - Python 3.8+  
> - [dbt Core](https://docs.getdbt.com/dbt-cli/installation)  
> - A Snowflake account with credentials  
> - Git installed

Follow these steps to set up and run this project locally:

---

### 📥 Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/airbnb-dbt-snowflake.git
cd airbnb-dbt-snowflake
```

### ⚙️ Step 2: Initialize dbt and Set Up Your Profile

This project assumes you've used dbt init to create your profile.

If you haven't already done so:
```
dbt init
```

This creates the default profiles.yml under:

Mac/Linux: ~/.dbt/profiles.yml

Windows: C:\Users\<your-user>\.dbt\profiles.yml

### Next Steps

```
dbt deps
dbt debug
dbt seed
dbt compile
dbt run --full-refresh
dbt test
dbt docs generate
dbt docs serve
```

