# ⚾ Building AI-Powered Analytics for Sports with Databricks

This project contains **Databricks notebooks** and **Unity Catalog Metric Views** for building an **AI/BI Genie–powered analytics solution** that explores how **MLB promotions, giveaways, and theme nights** influence game attendance across teams, venues, and seasons.

---

## 🚀 Step-by-Step Instructions

### 1. Set up your Databricks environment

1. Sign up for the [**Databricks Free Edition**](https://www.databricks.com/learn/free-edition) — no credit card required.  
2. Once your workspace is ready, open the Databricks interface.

---

### 2. Run setup notebooks to ingest and prepare data

#### `00-DDL`
- Sets up your data store (**catalog**, **schema**, and **tables**).
- Click **Run All** to initialize the objects.

#### 📁 Upload parquet files to Volumes
1. In the Databricks sidebar, go to **Catalog** → locate **`mlb_tech_summit`** → click the **`bronze`** schema.  
2. Under **Volumes**, navigate to:  
   `raw/all_games`
3. Click **Upload to this Volume** and upload the following file:
   - `games.snappy.parquet`

---

### 3. Process data through the Medallion Architecture

#### 🥉 `01-BRONZE`
- Loads raw data from parquet files into Delta tables.

#### 🥈 `02-SILVER`
- Cleans and standardizes data.  
- Enforces schema and adds contextual fields (e.g., `day_of_week`, `has_promotion`).

#### 🥇 `03-GOLD`
- Builds the Gold layer with aggregated insights.

### 🏅 `04-SEMANTIC`  
- Defines **Unity Catalog Metric Views** to power **AI/BI Genie dashboards** and natural language analysis.

### `05-CLEAN UP`
- This resets the project resources. DO NOT RUN!
---

### 4. Build and Explore

- **Dashboard Dev** → Create visual dashboards using the Gold tables and metric views.  
- **Genie** → Deploy your **conversational analytics agent** (e.g., “Which promotions increased attendance the most?”).  
- **Data Science Agent** → Extend insights with **machine learning** or predictive modeling.

---

### 🧠 Example Use Case

Analyze how specific promotions, such as *giveaways, fireworks nights, or theme games*, impact average attendance across teams and seasons — and uncover which events truly fill the stands.

---

### 🧰 Tech Stack

- **Databricks** (Free Edition)  
- **Unity Catalog** for governance  
- **AI/BI Genie** for natural language analytics  
- **Delta Tables + Metric Views** for semantic modeling  

---

### 📄 License

This repository is distributed under the MIT License. See `LICENSE` for more information.
