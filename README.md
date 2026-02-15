# 🧩 Customer Retention Decision System
### Turning churn data into retention actions

This project is not a churn prediction exercise.

It explores a more practical question:

> If a company knows customers are leaving, how should it decide *what to do*?

The goal was to transform raw customer data into a tool that helps teams choose the right retention intervention — not just identify risky users.

---

## The Problem

Subscription businesses often track churn as a percentage.  
But operational teams need answers to a different question:

**Why is this customer leaving, and what action prevents it?**

A prediction score alone cannot tell:
- whether to offer a discount
- whether to improve onboarding
- whether to change plan structure
- or whether intervention is unnecessary

Without context, retention efforts become expensive and ineffective.

---

## Product Goal

Design a system that allows non-technical teams to:

1. Understand types of churn
2. Identify root causes
3. Choose targeted interventions

Instead of forecasting churn, the system diagnoses it.

---

## Approach

### 1. Convert records into behaviour

Customer data was reorganised into interpretable signals:

| Behaviour | Meaning |
|--------|------|
| Lifecycle stage | How long the customer has stayed |
| Commitment level | Contract structure |
| Service adoption | Product usage depth |
| Payment behaviour | Billing friction |
| Support interaction | Experience quality |

This reframes churn as behaviour rather than probability.

---

### 2. Identify churn patterns

Customers naturally separated into distinct risk groups:

**Early churners**
- short tenure
- flexible plans
- low product adoption

**Value dropouts**
- long tenure
- higher cost sensitivity

**Experience-driven churn**
- repeated support interaction

Now churn becomes diagnosable, not random.

---

### 3. Build a decision interface

An interactive dashboard was created so teams can explore:

- churn across lifecycle stages
- contract impact on retention
- feature adoption vs churn
- billing behaviour vs churn

The output acts as a lightweight internal product, not a report.

---

## Example Decisions Enabled

| Scenario | Recommended Action |
|------|------|
| New customer on flexible plan | onboarding support |
| Valuable but disengaged user | proactive outreach |
| Feature-light users | education & activation |
| Contract-sensitive churn | plan restructuring |

---

## What this demonstrates

Many churn projects answer:

> Who might leave?

This project answers:

> What should we do about it?

The difference is moving from prediction → decision making.

---

## Product Thinking

The system is designed around three principles:

1. Understanding before automation  
2. Behaviour over demographics  
3. Targeted actions over blanket discounts  

Retention improves when intervention matches cause.

---

## How to explore

Open the dashboard and try answering:

- Which customers leave early in their lifecycle?
- Does product adoption reduce churn?
- Which users are worth saving?

Instead of reading insights, interact to reach decisions.

---

## Repository Contents

- dashboard — interactive churn exploration interface
- supporting data — customer records used for analysis
- documentation — behaviour definitions and logic

---
