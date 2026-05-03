### KPIs & Definitions Detail Documentation

This document provides a technical breakdown of the metrics used in the Meta Ad Performance Dashboard, including their calculation logic and business use cases.

### 📈 Core Metrics

| KPI | Definition | Formula | Example Use |
| :--- | :--- | :--- | :--- |
| **Impressions** | Number of times ads were displayed. | `Count of event_type = Impression` | Measure reach |
| **Clicks** | Number of times users clicked ads. | `Count of event_type = Click` | Measure engagement intent |
| **Shares** | Number of times ads were shared. | `Count of event_type = Share` | Viral engagement |
| **Comments** | Number of user comments on ads. | `Count of event_type = Comment` | User sentiment & feedback |
| **Purchases** | Number of purchases made after seeing ads. | `Count of event_type = Purchase` | Conversions |

### 🧪 Derived Metrics (Calculated)

| KPI | Definition | Formula | Example Use |
| :--- | :--- | :--- | :--- |
| **Engagements** | Total interactions (Clicks + Shares + Comments). | `Clicks + Shares + Comments` | Engagement volume |
| **CTR** | % of impressions that resulted in clicks. | `(Clicks / Impressions) * 100` | Ad effectiveness |
| **Engagement Rate** | % of impressions that resulted in engagements. | `(Engagements / Impressions) * 100` | Overall ad appeal |
| **Conversion Rate** | % of clicks that resulted in purchases. | `(Purchases / Clicks) * 100` | Funnel efficiency |
| **Purchase Rate** | % of impressions that resulted in purchases. | `(Purchases / Impressions) * 100` | Conversion from reach |

### 💰 Budget Metrics

| KPI | Definition | Formula | Example Use |
| :--- | :--- | :--- | :--- |
| **Total Budget** | Total spend allocated to campaigns. | `Sum of campaigns.total_budget` | Cost analysis |
| **Avg. Budget per Campaign** | Average budget allocation per campaign. | `Total Budget / Campaign Count` | Budget distribution |
