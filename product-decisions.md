# Product Decisions

This project started as a churn prediction task.

While working through the data, it became clear that prediction wasn’t the real issue.  
The team wouldn’t struggle to identify risky customers — they would struggle to decide what to do next.

So the goal shifted from forecasting churn to helping someone choose the right intervention.

---

## What problem does this actually solve?

The original question:
> Which customers will leave?

The practical question:
> What action should we take for this customer?

Different customers leave for different reasons.  
A single churn score treats them all the same, which usually leads to blanket discounts or unnecessary outreach.

The product therefore focuses on understanding the type of churn, not just the likelihood of churn.

---

## Who would use this?

The intended user is someone in retention or customer success.

Their workflow is simple:
1. Look at a customer
2. Decide whether to intervene
3. Choose how to intervene

The system needs to make that decision easier, not just more precise.

---

## Why not start with a prediction model?

A probability number sounds useful, but it creates practical problems:

- teams don’t know what action corresponds to the score
- false positives waste effort and budget
- users stop trusting the tool quickly

Before automation, teams need context.

So the first version explains behaviour instead of predicting it.

---

## Why segments instead of scores?

A score answers:
> how likely is churn

A segment answers:
> what is happening

Segments map naturally to actions:

- new customers leaving early → onboarding help
- valuable but inactive users → proactive outreach
- repeated issues → support escalation

This makes the tool usable without training.

---

## What would ship first?

The first version only supports human decisions:

- view churn patterns
- understand drivers
- identify customer type

No automated triggers yet.

---

## What would come next?

Later versions could:

- recommend actions
- trigger workflows automatically

But only after users trust the reasoning behind it.

---

## Guiding idea

Understanding should come before automation.

If teams don’t understand why customers leave, automation only scales mistakes.
