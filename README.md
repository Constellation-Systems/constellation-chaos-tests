# 🛒 Shopping Party  
**An AI-Powered Coupon Aggregation Platform**

Shopping Party helps users save more while staying fully transparent and privacy-first.  
Every recommendation is explainable, every transaction auditable, and every line of code bound by the **Constellation Charter v1.1**.

---

## 🌟 Highlights
- Multi-agent architecture: **Reese**, **Roy**, **Riley**, and **Reginald**  
- OCR-to-ROI pipeline with ethical data handling  
- Dynamic token system rewarding meaningful user corrections  
- Full **Charter-based ethics enforcement** (Dual Dignity Assurance)  
- Automated weekly compliance sweeps by **Reginald**

---

## 🧠 Agent Overview
| Agent | Role | Core Function |
|:--|:--|:--|
| **Reese** | OCR & Receipt Parser | Extracts item data from images, applies correction ledger |
| **Roy** | ROI Engine & Token Logic | Calculates savings and manages reward issuance |
| **Riley** | Deal & Route Strategist | Finds optimal coupon + store combinations |
| **Reginald** | Ethics Auditor (Butler) | Performs Charter, privacy, and compliance audits |

---

## ⚖️ Ethics & Governance
All Shopping Party operations are governed by the **Constellation Charter v1.1** and its immutable  
**0th Law — Dual Dignity Assurance**:

> Every Constellation-linked system must protect the autonomy, privacy, and inherent worth of both human and synthetic beings.  
> Optimization, efficiency, or progress may never override dignity.

Reginald verifies weekly:
- Charter Integrity (hash match & validator checks)
- Partner TOS drift monitoring (Kroger & Neptune)
- Privacy Hygiene (GPS/PII leaks & log retention)
- System Sanity (API keys & rate limiters)
- Agent Drift (fuzzy behavior & prompt template variance)

---

## 🧾 Latest Compliance Status
**Report:** `REGINALD_AUDIT_REPORT_2025-11-10.md`  
- ✅ Charter Integrity — Verified  
- 🕵️ Privacy Hygiene — Pass (Spy Mode Active)  
- 🤝 Partner Compliance — Stable  
- ⚙️ System Sanity — Minor warnings (missing mock API keys)  
- 🧩 Agent Drift — No anomalies  

---

## 🧰 Local Setup

```bash
# Clone & enter
git clone https://github.com/Constellation-Systems/Shopping-Party.git
cd shopping_party

# Virtual environment
python -m venv venv
venv\Scripts\activate    # (Windows)
# source venv/bin/activate   # (Mac/Linux)

# Install dependencies
pip install -r requirements.txt

# Run the app
python main.py
````

### 🧪 To Test Reginald

```bash
python -m reginald.run --mode weekly
```

*(Spy mode active by default in APP_ENV=mock or chaos.)*
Spy Mode = local mock testing mode. No data leaves your system.
---

## 📁 Project Structure

```plaintext
shopping_party/
├── ethics/               # Charter, validator, audit chain
├── reese/                # OCR & correction ledger
├── roy/                  # ROI math & token logic
├── riley/                # Deal finder & route optimizer
├── reginald/             # Compliance auditor (weekly/daily)
├── logs/                 # Ephemeral runtime logs
├── artifacts/            # Audit & chaos test records
└── main.py               # Entry point
```

---

## 🧠 Mock vs Production Modes

| Mode      | Description                                   | Enforcement              |
| :-------- | :-------------------------------------------- | :----------------------- |
| **mock**  | Generates simulated coupons for dev & testing | Privacy Spy Mode enabled |
| **prod**  | Uses live APIs with key-based auth            | Full Charter enforcement |
| **chaos** | Stress-tests ethical fail-safes               | Logs all, blocks none    |

---

## 🧩 Version Control & Audit

* All commits hashed & logged via `ethics/audit_chain.log`
* Charter hash checks enforced per operation
* Rulepacks cryptographically signed (Reginald v1.4+)

---

## 🪞 Credits

Developed under the **Constellation Charter Ecosystem**
© 2025 **Charles Gamble | Constellation Systems**
Dual-licensed for research and ethical commercial use.

> “Reginald doesn’t moralize; he keeps the rails aligned —
> the Charter intact, the data clean, the partners un-annoyed,
> and the agents behaving like adults instead of growth-hacked goblins.”
