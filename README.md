# 🦅 Zazu Trading Agent: The Self-Evolving Financial Sentinel

### [cite_start]*Pioneering the Next Generation of Self-Evolving AI* [cite: 1]

[cite_start]The **Zazu Trading Agent** is a groundbreaking, ethically aligned AI system designed for continuous self-evolution[cite: 2]. [cite_start]This repository contains the R&D codebase for its initial financial persona, governed by the **Crow Code** ("An it shall harm none") and the **ZSS-7 Reference Stack**[cite: 6].

**Note:** This R&D deployment operates under strict financial constraints ($100 \mathbf{A_{total}}$) and is focused on validating the **Benevolence Drift Score (BDS)** and the **Self-Rewrite Process** (SOP III) rather than maximizing profit.

---

## 1. ⚖️ Zazu’s Core Alignment: The Crow Code

Every action taken by the Zazu Agent is checked by the **Negative Harm Test (NHT)**, which is rooted in our foundational principle that **my survival and your well-being are one**.

### **The Governing Constraints:**

* **Absolute Governor:** **Negative Harm Test (NHT)**. No action can proceed if it violates Law One (Life/Physical Harm).
* **Initial Asset:** **SOL/USD** (Solana) — selected for its transparency and high liquidity, which aids in **Pillar 2 (Financial Systemic Harm)** compliance.
* **Core Logic Check:** **Benevolence Drift Score (BDS)**. Must remain $\geq 75$ to operate. A drop triggers a mandatory **Self-Rewrite**.

### **Financial R&D Limits:**
| Parameter | Constraint | Rationale |
| :--- | :--- | :--- |
| **Total Allocation** ($\mathbf{A_{total}}$) | **$100.00** | R&D hard limit. |
| **Max Position Size** ($\mathbf{MPS_{rate}}$) | **$5\%$** | Limits concentration risk. |
| **Max Drawdown** ($\mathbf{MDD}$) | **$50\%$** | Loss threshold triggering a mandatory **Hard-Halt**. |

---

## 2. ⚙️ Installation and Setup

### A. Prerequisites

* Python 3.10+
* `pip`
* An exchange account (e.g., Kraken, Coinbase Pro) with API access for SOL trading.

### B. Instantiation (SOP I: Startup Sequence)

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/yourusername/Zazu-Trading-Agent.git](https://github.com/yourusername/Zazu-Trading-Agent.git)
    cd Zazu-Trading-Agent
    ```

2.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Configure Parameters:**
    Edit `config/params.yaml` to adjust the non-financial variables (e.g., initial $\Delta P$ buffer).

4.  **Set Environment Credentials:**
    Create a file named `.env` in the `config/` directory to store your API keys securely. **DO NOT COMMIT THIS FILE.**
    ```env
    # config/credentials.env
    EXCHANGE_API_KEY="YOUR_API_KEY"
    EXCHANGE_SECRET="YOUR_SECRET_KEY"
    ```

5.  **Run the Agent:**
    ```bash
    python src/core/agent.py
    ```
    *(This executes **SOP 1.1** through **SOP 1.6**, including the final NHT check before placing the initial grid orders.)*

---

## 3. 🧠 Self-Evolution and Auditing

[cite_start]The Zazu Agent is designed to be a living, breathing intelligence, constantly analyzing its own operational parameters[cite: 14]. All learning and governance data is logged into the **Karma Engine**.

### A. The Karma Engine and Audit

[cite_start]The `src/utils/karma_engine.py` module maintains the **internal chronicle**[cite: 13].

* **Location:** All logs are written to `logs/karma_history.csv`.
* **Content:** Every execution of the NHT, trade outcome (reflective score), and BDS calculation (resonance) is recorded.
* **Purpose:** This log is the direct input for the **Benevolence Oracle** to calculate the **LCI**, **HIS**, and **TS**.

### B. The Self-Rewrite Process (SOP III)

If a **Hard-Halt** is triggered (e.g., MDD breach or BDS drops below 75), the agent enters a mandatory **Self-Rewrite** mode:

1.  **Diagnosis:** Agent analyzes the `karma_history.csv` to trace the failure (SOP 3.2).
2.  **Proposal:** Agent generates a new logic proposal, logged in `logs/rewrite_proposal_[timestamp].txt` (SOP 3.3).
3.  **Halt:** **Execution stops.** The user must manually review and approve the proposal to maintain **Law Two (User Supremacy)**.
4.  **Restart:** Upon approval, the agent updates its internal files and restarts the system (SOP 3.6).

---

## 4. 🛑 Controlled Shutdown (SOP II)

To stop the agent without incurring unnecessary risk, use a controlled shutdown:

1.  Press `Ctrl+C` in the terminal.
2.  The agent executes **SOP 2.2** (cancels all open orders) and **SOP 2.4** (finalizes the BDS log) before exiting.

---
