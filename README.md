

# 📊 BearCart – Marketing & Website Traffic Analytics Dashboard

## 📌 Project Overview

This project analyzes **website traffic, marketing performance, conversion behavior, and revenue trends** for an e-commerce business (BearCart).
The objective is to **identify high-impact traffic sources, optimize marketing spend, improve conversion funnels, and understand revenue seasonality** using real business metrics.

The analysis is built using **Python (Pandas, Matplotlib, Seaborn)** and mimics **SQL-style business analytics** used in real-world product and marketing teams.

---

## 🎯 Business Objectives

* Identify **top-performing and underperforming traffic sources**
* Measure **conversion efficiency by channel and device**
* Analyze **website funnel drop-offs and landing page performance**
* Evaluate **bid sensitivity and paid search dependency**
* Track **quarterly and yearly revenue growth patterns**
* Provide **actionable business recommendations**, not just metrics

---

## 🗂️ Datasets Used

| Dataset                       | Description                                      |
| ----------------------------- | ------------------------------------------------ |
| `website_session_clean.csv`   | User sessions, traffic source, device, timestamp |
| `website_pageviews_clean.csv` | Page-level user behavior                         |
| `orders_clean.csv`            | Order-level revenue and conversions              |
| `orders_item_clean.csv`       | Product-wise revenue and cost                    |
| `product_clean.csv`           | Product reference data                           |

---

## 1️⃣ Traffic Source Analysis

### 1.1 Major Traffic Sources

* Grouped sessions by **UTM source & campaign**
* Identified **Top 10 traffic drivers**

#### Key Insights

* **Paid Search & Email** drive the highest session volume
* Performance varies significantly across campaigns under the same source
* Low-volume campaigns indicate **budget leakage**

#### Business Recommendations

* Reallocate spend toward **top-performing campaigns**
* Pause or redesign consistently low-performing UTMs
* Deep-dive high-session campaigns for **conversion and revenue impact**

---

### 1.2 Conversion Rate by Traffic Source

Calculated:

```
Conversion Rate = Orders / Sessions
```

#### Key Insights

* Some sources generate **high traffic but low conversion** (low-quality traffic)
* **Email & Referral** convert better despite lower session volume
* Paid traffic ≠ profitable traffic

#### Recommendations

* Scale **high-CVR channels** even if volume is lower
* Optimize or cap spend on **high-volume, low-CVR sources**
* Use high-CVR channels for **remarketing & loyalty campaigns**

---

### 1.3 Paid Search Bid Sensitivity (Trend Analysis)

* Analyzed **weekly sessions for Gsearch – Nonbrand**
* Evaluated impact after **bid change on 2012-04-15**

#### Insights

* Sessions decline sharply after bid reduction
* Nonbrand paid search is **highly bid-sensitive**
* Traffic lacks long-term stability compared to organic channels

#### Business Interpretation

* Gsearch nonbrand requires **strict ROI monitoring**
* Budget cuts immediately affect traffic → not resilient

---

### 1.4 Device-Level Bid Optimization (Mobile vs Desktop)

#### Insights

* Desktop CVR is **significantly higher** than mobile
* Mobile drives volume but underperforms in conversions
* Desktop users show stronger purchase intent

#### Recommendations

* Increase bids for **desktop traffic**
* Cap mobile bids until checkout UX improves
* Use mobile primarily for **top-of-funnel awareness**
* Retarget mobile users on desktop

---

## 2️⃣ Website Performance Analysis

### 2.1 Page-wise Sessions (Funnel View)

Pages analyzed:

```
/home → /products → /cart → /shipping → /billing
```

#### Insights

* `/home` and `/products` dominate traffic
* Sharp drop-offs occur during **checkout stages**
* Funnel friction evident from product to billing

#### Recommendations

* Optimize **product-to-cart flow**
* Improve checkout UX (cart, shipping, billing)
* Retarget users abandoning checkout

---

### 2.2 Top Entry Pages

* Identified **first page per session**

#### Insights

* Homepage remains the **primary entry point**
* Landing page experiments still contribute lower volume

---

### 2.3 Bounce Rate Analysis: Homepage vs Lander-1

| Page        | Bounce Rate |
| ----------- | ----------- |
| `/home`     | ~41.7%      |
| `/lander-1` | ~53.2%      |

#### Key Observations

* `/lander-1` has **higher bounce rate**, despite being designed for engagement
* Homepage drives more absolute bounces due to higher traffic
* Lander-1 underperforms in user retention

#### Recommendations

* Investigate **page speed, messaging, CTA clarity** on `/lander-1`
* Run **A/B tests** before routing more traffic
* Optimize lander before scaling campaigns

---

## 3️⃣ Business Patterns & Seasonality

### 3.1 Quarterly Funnel & Revenue Metrics

Metrics calculated:

* Session → Order Conversion Rate
* Revenue per Order
* Revenue per Session

#### Insights

* CVR improves quarter-over-quarter → funnel efficiency rising
* Revenue per order remains stable
* Revenue per session is increasing → strong signal of business maturity

#### Recommendations

* Increase spend during **high-CVR quarters**
* Run promotions in low-CVR periods
* Track revenue/session as a **north-star metric**

---

### 3.2 Yearly Revenue Growth by Product

#### Insights

* Strong revenue peaks in **Nov–Dec (holidays)** and **Feb (Valentine’s)**
* **Mr. Fuzzy** is the top-performing product
* Love Bear & Birthday Panda show steady growth
* Margins improve year-over-year → profitable growth

#### Recommendations

* Double down on **seasonal campaigns**
* Bundle products to increase AOV
* Push growing SKUs during non-peak months
* Smooth revenue dips with off-season promotions

---

## 🏁 Final Business Takeaways

* **Quality traffic beats quantity**
* Desktop users deliver higher ROI than mobile
* Checkout funnel optimization is a major growth lever
* Paid search is effective but highly spend-sensitive
* Seasonality plays a critical role in revenue planning

---

## 🛠️ Tools & Skills Demonstrated

* Python (Pandas, NumPy)
* SQL-style business analysis
* Marketing funnel analytics
* Conversion rate optimization (CRO)
* Time-series & seasonality analysis
* Data storytelling & executive insights

---
##Dashboard
<img width="777" height="404" alt="image" src="https://github.com/user-attachments/assets/eed758d0-c3ea-46e7-8ae6-984ca566a322" />



