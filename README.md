# CRM Value Realisation Engine (CVRE)

**Quantifying Revenue Leakage from CRM Behaviours and Governance Gaps**

---

## Overview

Most CRM implementations succeed at data capture but fail at **value realisation**.

Dashboards show pipeline size, activities, and stages, yet leadership still cannot answer a critical question:

> How much revenue is leaking due to CRM behaviours, and how much of it can realistically be recovered?

The **CRM Value Realisation Engine (CVRE)** is a decision-oriented analytics framework that quantifies CRM value leakage in monetary terms (€) and simulates the impact of enforceable governance rules.

This repository is **not** a dashboarding or reporting exercise.  
Power BI is used only as a communication layer for model-driven insights.

---

## Problem Statement

In real CRM environments:
- Leads are contacted too late
- Opportunities stall without intervention
- Stages progress without evidence
- Data completeness creates false confidence

These issues do not appear as errors — they appear as **silent revenue leakage**.

Traditional CRM dashboards describe activity.  
They do not quantify the **cost of poor behaviour**.

CVRE was built to bridge that gap.

---

## What This Project Does

### Behaviour-Driven Value Modelling
- Converts opportunities into **Expected Value (EV)**
- Models behavioural penalties from:
  - slow lead response
  - missing sales activity
  - stalled opportunities
  - stage hygiene violations
- Handles incomplete CRM data using explainable assumptions

### Revenue Leakage Quantification
- Calculates total leaked EV across the pipeline
- Deduplicates overlapping behavioural failures
- Separates total leakage from realistically recoverable leakage

### Counterfactual Governance Scenarios
Simulates enforceable CRM rules such as:
- Lead response SLAs
- Activity evidence requirements
- Mandatory stall reviews
- Combined governance enforcement

Each scenario outputs **€ recovered**, not abstract scores.

### Executive Decision Dashboards
Two Power BI dashboards communicate:
- where value is leaking,
- why it is leaking,
- and what leadership can enforce to recover it.

---

## Key Results

Using a realistic synthetic CRM dataset:

- **Total Pipeline Expected Value:** €10.71M  
- **Total Leaked EV:** €2.08M (~19.5%)  
- **Recoverable EV:** €0.84M (~40.5% of leakage)  
- **Estimated Governance ROI:** ~5.6×  
- **CRM Trust Score:** ~78%

Primary leakage drivers:
- Stalled opportunities (>30 days)
- Missing logged activities
- Slow lead response (>48h)
- Stage progression without evidence

---

## Dashboard Design

### Dashboard 1 — CRM Value Health & Leakage Overview
**Purpose:** Diagnose CRM value leakage  
Answers:
- Is there a value problem?
- Where is revenue leaking?
- How trustworthy is the pipeline?

### Dashboard 2 — Recovery Scenarios & Decision Actions
**Purpose:** Enable leadership decisions  
Answers:
- What rules should be enforced?
- How much value does each rule recover?
- Where should enforcement start?

---

## Why Machine Learning Is Used

Machine learning is not used for visualisation.

It is used to:
- estimate win probabilities,
- calculate expected value,
- model behavioural impact,
- and simulate counterfactual recovery scenarios.

Without modelling, this would be descriptive BI.  
With modelling, it becomes **decision analytics**.

---

## Project Structure

