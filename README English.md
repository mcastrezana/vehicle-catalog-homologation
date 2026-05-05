# Vehicle Catalog Homologation – Case Study

## 📌 Overview

This repository presents a **case study on vehicle catalog homologation**
between an internal catalog and multiple insurer catalogs within the insurance industry.

It is based on **real operational experience** in a multinational corporate environment.  
All data, names, and examples included have been **modified or simulated** for
demonstration and professional portfolio purposes.

The objective of this repository is to showcase:
- How vehicle catalogs are structured
- How homologation rules are defined and applied
- Common issues that impact quotation and policy issuance
- Process improvements derived from hands‑on operational experience

---

## 🧩 Problem Context

In multi‑insurer environments, quotation and policy issuance depend on the proper
alignment between **internal vehicle catalogs** and **insurer catalogs**.

Common challenges include:
- Misalignment between catalogs
- Missing mandatory internal keys
- Duplicate or ambiguous vehicle versions
- Confusion between **catalog issues** vs **tariff issues**
- Late manual validations

These challenges directly impact:
- Quotation availability
- Operational rework
- Response times
- Customer experience

---

## 🗂️ Catalog Approach

This case study assumes two main catalog layers:

- **Internal Vehicle Catalog**
  - Standardized structure
  - Unique internal keys
  - Centralized data governance

- **Insurer Vehicle Catalog**
  - Insurer‑specific naming and versions
  - Independent update cycles
  - Rules defined per insurer

The homologation process ensures that **only properly validated vehicles**
can be used for quotation and policy issuance.

---

## 🔁 Homologation Logic

Homologation rules aim to:
- Ensure all vehicles have a valid internal key
- Prevent quotation of non‑homologated vehicles
- Reduce late manual validations
- Detect inconsistencies early in the process

This repository documents:
- Generic homologation rules
- Validation criteria
- Exception handling
- Common operational errors

---

## 🔄 Process Evolution

The included diagrams illustrate:
- **AS‑IS**: fragmented validations and late error detection
- **TO‑BE**: clear rules, early validation, and improved data control

The proposed improvements aim to:
- Reduce rework
- Improve data quality
- Accelerate operational timelines
- Clarify ownership and responsibilities

---

## 🔄 Process Diagrams

To facilitate understanding of the homologation and quotation flow,
this repository includes diagrams representing both the current (**AS‑IS**)
and proposed (**TO‑BE**) processes.

### 📍 AS‑IS – Current Process

The current homologation and quotation validation process is **highly manual**,
with multiple decision points and dependency on insurer‑ and business‑specific data.

- **AS‑IS simplified**  
  High‑level view of the complete flow, designed for quick understanding.  
  👉 `diagrams/as-is-overview.mmd`

- **AS‑IS detailed**  
  Representation of the real operational process, including validations,
  rework, and manual intervention points.  
  👉 `diagrams/as-is-detailed.jpg`

---

### 🚀 TO‑BE – Proposed Process

The TO‑BE process proposes improvements focused on:
- Early validations
- Reduced manual intervention
- Clear separation between catalog, homologation, and tariff
- Improved traceability per insurer and business

- **TO‑BE simplified**  
  Optimized flow illustrating how the process could operate with greater
  control and efficiency.  
  👉 `diagrams/to-be-overview.mmd`

---

## 🧠 AS‑IS vs TO‑BE Comparison

| Aspect                     | AS‑IS                     | TO‑BE                          |
|---------------------------|----------------------------|--------------------------------|
| Homologation              | Manual and progressive     | Standardized                   |
| Duplicate AMIS control    | Manual review              | Automated rule                 |
| Internal key (Aon key)    | Late validation             | Early generation/validation    |
| Catalog vs tariff logic   | Frequent confusion         | Clear separation               |
| “No quotation” diagnosis | Reactive                   | Preventive                     |
| Traceability              | Partial                    | Centralized                    |

---

## 📁 Repository Structure


vehicle-catalog-homologation/
│
├─ docs/        # Conceptual documentation and business rules
├─ mock-data/   # Simulated datasets for demonstration purposes
├─ diagrams/    # Process and catalog relationship diagrams (Mermaid)
└─ validation/  # Validation logic and examples
``

---

## ⚠️ Disclaimer
- This repository **does not contain real data**
- No client, insurer, or production system information is included
- Content represents professional experience **translated into a portfolio‑safe format**

---

## 🎯 Target Audience
- Business / Data Analysts
- Insurance Operations teams
- Technical and Functional Leads
- Product Owners and Process Improvement teams
- Recruiters seeking real‑world operational experience

_Built from real experience. Shared responsibly._
