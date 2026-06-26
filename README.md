# KPI Framework, Business Experiment Analysis & Decision Recommendation

## Business Context

A subscription-based digital product company launched a new onboarding and activation campaign to improve user conversion and early engagement. An A/B experiment was conducted where users were randomly assigned to either the existing onboarding experience (Control) or the new onboarding campaign (Treatment). The objective was to determine whether the new onboarding experience should be rolled out to all users.

---

## Business Problem

The primary business decision is whether to launch the new onboarding campaign to all users.

The decision impacts product managers, business leadership, marketing teams, and customer success teams.

The main objective is to improve the **Paid Conversion Rate**, while monitoring important guardrail metrics such as refund rate, support ticket rate, engagement score, and average days to convert.

A recommendation is made only after evaluating experiment performance, statistical significance, and business risks.

---

## Dataset Description

The dataset contains user-level information collected during the A/B experiment, including:

- User ID
- Experiment Group
- Region
- Device Type
- Traffic Source
- Plan Type
- Landing Page Visit
- Trial Start
- Onboarding Completion
- Paid Conversion
- Revenue (30 Days)
- Support Tickets
- Refund Requests
- Days to Convert
- Engagement Score

After data cleaning:

- Total users analyzed: **1400**
- Control Group: **690**
- Treatment Group: **710**

---

## Data Cleaning Summary

The following quality checks were performed:

- Checked for missing values.
- Retained blank values in **days_to_convert** for users who did not convert.
- Identified **14 missing engagement scores** and excluded them from engagement average calculations.
- Removed **8 duplicate user IDs** before analysis.
- Verified that binary variables contained only valid values (0 or 1).
- Checked revenue for outliers.
- Verified segment distribution across Region, Device Type, Traffic Source, and Plan Type.

---

## North Star Metric

**Paid Conversion Rate**

This metric directly measures business growth by tracking the percentage of users who become paying customers.

Supporting metrics include:

- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate
- Average Revenue per User
- Engagement Score

Guardrail metrics ensure that improvements do not negatively impact the overall customer experience.

---

## KPI Tree Summary

North Star Metric:
- Paid Conversion Rate

Primary KPI Drivers:

1. User Acquisition
   - Landing Page Visit Rate
   - Trial Start Rate

2. User Activation
   - Onboarding Completion Rate
   - Engagement Score

3. User Monetization
   - Average Revenue per User
   - Average Revenue per Converted User

Guardrail Metrics:

- Refund Rate
- Support Ticket Rate
- Average Days to Convert

---

## Experiment Analysis Approach

The experiment compared Control and Treatment groups using business KPIs.

Metrics analyzed included:

- User Count
- Landing Page Visit Rate
- Trial Start Rate
- Onboarding Completion Rate
- Paid Conversion Rate
- Average Revenue per User
- Average Revenue per Converted User
- Refund Rate
- Support Ticket Rate
- Average Engagement Score
- Average Days to Convert

Segment-level analysis was also performed using:

- Region
- Device Type
- Traffic Source
- Plan Type

---

## Hypothesis Test Summary

A Two-Proportion Z-Test was conducted using Paid Conversion Rate as the primary metric.

Results:

- Control Conversion Rate: **3.19%**
- Treatment Conversion Rate: **7.04%**
- P-value: **0.0011**

Since the p-value is below 0.05, the null hypothesis was rejected.

The Treatment group demonstrated a statistically significant improvement in paid conversion.

---

## Guardrail Metrics

The following guardrail metrics were evaluated:

- Refund Rate
- Support Ticket Rate
- Average Days to Convert
- Engagement Score

Although support ticket volume increased slightly, the overall business impact remained positive due to significantly higher conversion and engagement.

---

## Final Recommendation

**Launch the new onboarding campaign for all users.**

The Treatment group significantly improved user conversion, engagement, and conversion speed. Statistical testing confirmed that the improvement was significant, while guardrail metrics indicated manageable business risk.

---

## Assumptions & Limitations

- Missing engagement scores were excluded from average calculations.
- Duplicate user IDs were removed before analysis.
- Some segment fields contained missing values.
- The dataset measures short-term experiment performance only and does not include long-term customer retention.

---

## Repository Contents

- Dataset
- Experiment Analysis Workbook
- KPI Tree
- Experiment Summary
- Hypothesis Test Notes
- Recommendation Memo
- Screenshots
- README

---

## Screenshots Included

- summary_metrics.png
- hypothesis_test_output.png
- kpi_tree_preview.png
