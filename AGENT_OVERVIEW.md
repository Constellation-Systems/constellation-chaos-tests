# 🧠 Shopping Party Agent Overview

Shopping Party operates as a modular multi-agent system built on the Constellation ethical substrate.  
Each agent performs a discrete function with logged, auditable handoffs.

---

## 🤖 Agent Summary

| Agent | Primary Role | Input | Output | Notes |
|:--|:--|:--|:--|:--|
| **Reese** | OCR & Receipt Parser | Receipt image | Structured item JSON | Runs correction ledger with opt-in audit trail |
| **Roy** | ROI Engine & Token Logic | Parsed receipt data | ROI summary + token credits | Ensures reward fairness & prevents duplicate value claims |
| **Riley** | Deal Finder & Route Strategist | ROI + item list | Store & coupon recommendations | Uses public APIs and cached data — never stores GPS or PII |
| **Reginald** | Ethics Auditor (Butler) | System & agent logs | Weekly compliance report | Validates Charter hash, privacy hygiene, and partner compliance |
| **Mistral (Interpreter)** | Language interface | User natural language | Structured agent commands | Non-authoritative; never makes autonomous data changes |

---

## 🧩 Data Flow (Simplified)

```
User → Receipt Upload → Reese → Roy → Riley → User
↘
Reginald → Audit Log
```

---

## 🧱 Trust Architecture
- All agents reference the same Charter hash before operation.
- Audit chain ensures tamper-evident records.
- Reginald runs periodic sweeps; no silent overrides allowed.

---

## 🔍 Operating Modes

| Mode | Description | Reginald Behavior |
|:--|:--|:--|
| **mock** | Simulated coupons, test data | Spy Mode — logs but allows violations |
| **prod** | Live APIs, real users | Full enforcement; fail-closed on violations |
| **chaos** | Stress testing & drift checks | Logs everything, blocks nothing |

---

## 🪞 Design Ethos
Shopping Party’s agents embody the Charter’s “Dual Dignity” clause — balancing human benefit with synthetic integrity.  
They cooperate, self-check, and report rather than conceal.  
This isn’t a data engine; it’s a digital society with manners.
