# SQL Sample Databases & Analytics Portfolio

A curated collection of structured relational databases used for business intelligence, geographical mapping, marketing performance tracking, and behavioral data analysis. 

Each dataset includes a production-ready MySQL `.sql` schema script alongside its source `.csv` data file.

---

## Repository Directory Structure

* 📂 `market_analysis.sql` / `.csv` — Multi-channel digital marketing metrics (ROI, CPC, CTR).
* 📂 `meesho_meesho_orders.sql` / `.csv` — E-commerce transaction logging and order tracking data.
* 📂 `unesco_sites.sql` / `.csv` — Global heritage locations featuring precision coordinates and land areas.
* 📂 `urban_street_food.csv` — Vendor performance and operation metrics for survival classification models.

---

## Project Installation & Deployment Guide

Follow these steps to deploy any of these sample databases to your local MySQL server instance.

### Prerequisites
* MySQL Server (v8.0 or newer recommended) installed and active.
* Terminal, Command Prompt, or Git Bash initialized in the project directory.

### Step 1: Initialize Database Containers
Log into your MySQL shell monitor interface:
```bash
mysql -u root -p


Execute the database creation blocks sequentially to create the empty environments:

CREATE DATABASE market_analysis;
CREATE DATABASE meesho;
CREATE DATABASE unesco_sites;
CREATE DATABASE street_food_analysis;
EXIT;


Step 2: Stream Data Backups Into Tables
From your standard operating system terminal (pointing to your data directory folder), execute the standard import commands matching the target databases:


# 1. Market Analysis Data Import
mysql -u root -p market_analysis < market_analysis.sql

# 2. Meesho E-Commerce Data Import
mysql -u root -p meesho < meesho_meesho_orders.sql

# 3. UNESCO Heritage Sites Data Import
mysql -u root -p unesco_sites < unesco_sites.sql

Detailed Schema Directory
1. Market Analysis
Tracks core multi-channel campaign variables. Ideal for modeling campaign efficiencies, calculating net margins, and isolating low-performing ad placements.

Key Fields: CampaignID, Spend, Impressions, Clicks, Conversions, Revenue, ROI.

2. Meesho Order Records
Simulates transactional data from a live consumer ecosystem. Excellent for cohort retention calculations, behavioral patterns, and time-series forecasting.

Key Fields: E-commerce customer profiling and order fulfillment statuses.

3. UNESCO Heritage Sites
A geospatial data matrix mapping global cultural landmarks. Optimized for spatial coordinate computations and regional mapping analysis.

Key Fields: name, country, category, year, area, danger, region, latitude, longitude.

4. Urban Street Food Vendor Survival
An operational ledger tracking vendors across major metros. Built to evaluate regulatory constraints, environmental variables, and economic hazards affecting financial stability.

Key Fields: vendor_id, city, zone_type, avg_daily_revenue_inr, monthly_health_inspection_score, vendor_survived.

License
This database compilation portfolio is open-source software distributed under the MIT License.


