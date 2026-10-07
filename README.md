# AISIN_DX_Project_PressMachine

# Business Problem #

For our demo, let's make the problem **simple, realistic, and presentation-ready**.

## 1. Business Problem

A manufacturing plant operates multiple **press machines（プレス機・ぷれすき）**.

The machines continuously generate production and condition data, but engineers may not have an easy way to identify:

* declining machine performance
* increasing downtime
* abnormal vibration/temperature
* increasing defective products
* machines that may require maintenance

So the problem is:

> **How can we use press-machine data to identify abnormal machine behavior and understand its impact on production, quality, and machine performance?**

### Japanese

> **プレス機（ぷれすき）のデータを活用（かつよう）して、設備（せつび）の異常（いじょう）や性能（せいのう）の低下（ていか）を早期（そうき）に発見（はっけん）したい。**

---

## 2. Business Objective

Our objective is to build a small **Manufacturing DX analytics solution** that:

```text
Press Machine Data
       ↓
Databricks
       ↓
Data Processing
       ↓
Manufacturing KPIs
       ↓
Abnormal Behavior Detection
       ↓
Power BI Dashboard
       ↓
Engineer Decision
```

Specifically, we want to:

1. **Monitor machine performance**
2. **Measure production and quality**
3. **Calculate OEE**
4. **Identify abnormal machine behavior**
5. **Highlight machines requiring attention**
6. **Help engineers make data-driven decisions**

---

## 3. Business Questions

Our project should answer these questions:

### Machine

> Which press machine is performing poorly?

### Production

> How much did each machine produce?

### Quality

> Which machine has the highest defect/NG rate?

### Downtime

> Which machine loses the most production time?

### OEE

> Which machine has the lowest OEE?

### Abnormality

> Is any machine showing unusual behavior?

### Maintenance

> Which machine should the engineer inspect first?

---

## 4. Example Scenario

Suppose our data shows:

| Machine   | OEE | Downtime | NG Rate | Vibration | Status |
| --------- | --: | -------: | ------: | --------: | ------ |
| PRESS-001 | 91% |   18 min |    1.2% |    Normal | 🟢     |
| PRESS-002 | 87% |   31 min |    2.1% |    Normal | 🟡     |
| PRESS-003 | 72% |   65 min |    5.4% |      High | 🔴     |

Our system should tell the engineer:

> **PRESS-003 requires attention.**

Further analysis might show:

```text
PRESS-003

Vibration       ↑
Temperature     ↑
Motor Current   ↑
Cycle Time      ↑
NG Rate         ↑
Downtime        ↑
       ↓
Abnormal behavior
       ↓
Maintenance investigation recommended
```

This is the **business value** of the project.

---

# 5. What We Are NOT Trying to Build

For this demo, we are **not** trying to:

❌ Control the physical press machine
❌ Build a real PLC system
❌ Build real-time IoT infrastructure
❌ Simulate an entire factory
❌ Predict the exact time of machine failure

We're demonstrating the **data analytics / manufacturing DX side**.

---

# 6. Final Goal

Our final project goal is:

> **Use Databricks to transform press-machine data into manufacturing insights and Power BI to provide engineers with a clear view of machine performance, OEE, quality, downtime, and abnormal behavior.**

### Japanese version

> **Databricks（データブリックス）を使（つか）ってプレス機（ぷれすき）のデータを分析（ぶんせき）し、Power BI（パワービーアイ）で設備（せつび）の稼働率（かどうりつ）、品質（ひんしつ）、停止時間（ていしじかん）、異常（いじょう）を可視化（かしか）します。**

---

## ✅ Step 1 Complete

Your project definition is now:

**Problem:**
Press-machine problems are difficult to identify early from raw manufacturing data.

**Solution:**
Databricks-based data processing and analytics + Power BI visualization.

**Business value:**
Better visibility → earlier detection → better maintenance decisions → improved **OEE, quality and productivity**.

### Next

**Step 2 — Generate the synthetic press-machine dataset with Python.**

We'll design the **exact columns, data types, number of rows, machines, products, and abnormal scenario** before generating the CSV.
