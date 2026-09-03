# Causal Uplift Modeling for Promotional Targeting

## 📌 Project Overview

Have you ever wondered:

> **"Which customers should actually get a discount?"**

Giving a discount to everyone is not always a good idea.

Some customers will buy even without a discount. Giving them a coupon only reduces the company's profit.

Some customers will buy **only because** they received the coupon. These are the customers we really want to target.

This project uses **Causal Uplift Modeling** to identify those customers.

---

## 🎯 What Are We Trying to Predict?

A normal machine learning model might tell us:

> "This customer has a 75% chance of buying."

But that is not enough.

We want to answer:

> **"How much more likely is this customer to buy because of the promotion?"**

For example:

| Customer | Without Coupon | With Coupon | Uplift |
|---|---:|---:|---:|
| A | 20% | 75% | +55% |
| B | 80% | 82% | +2% |
| C | 5% | 7% | +2% |

Customer A is the most interesting customer because the promotion changes their behavior significantly.

---

## 👥 Customer Types

We can divide customers into four groups:

### 1. Persuadables ⭐

They don't buy without the promotion but are likely to buy with it.

**→ These are our main target customers.**

### 2. Sure Things

They are likely to buy even without the promotion.

**→ Don't waste a discount on them.**

### 3. Lost Causes

They are unlikely to buy with or without the promotion.

**→ Don't target them.**

### 4. Sleeping Dogs

They may buy without the promotion but could respond negatively to the treatment.

**→ Avoid targeting them.**

---

## 📊 Dataset

We are using the **Criteo Uplift Modeling Dataset**.

The dataset contains information about:

- Customer features
- Whether the customer received a treatment
- Whether the customer visited
- Whether the customer converted

The dataset allows us to compare customers who received the treatment with customers who did not.

---

## 🧠 How the Project Will Work

The project will be built step-by-step:

```text
Dataset
   ↓
Understand the Data
   ↓
Clean & Validate Data
   ↓
Explore Treatment vs Control
   ↓
Build Normal ML Baseline
   ↓
Build Uplift Models
   ↓
Measure Uplift
   ↓
Identify Persuadable Customers
   ↓
Calculate Business Value
   ↓
Build API
   ↓
Build Simple UI