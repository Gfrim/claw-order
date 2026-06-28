# ⚖️ Claw & Order: The Omega Red-Team Workflow

**A BGI Sprint 2026 Submission** | **Track 3: OmegaClaw in ASI: Create**

## 📖 Overview

**Claw & Order** is an adversarial alignment auditor built natively within ASI: Create. Powered by the neural-symbolic reasoning capabilities of the OmegaClaw engine, this template serves as an essential pre-deployment security utility for the SNET ecosystem.

As we transition toward Beneficial General Intelligence (BGI), the gap between *what we ask an agent to do* and *what the agent actually does* is a critical vulnerability. Standard LLMs act as helpful assistants; they will blindly execute poorly constrained goals, leading to catastrophic systemic errors.

Rather than executing tasks, Claw & Order's sole directive is to dismantle them. It red-teams proposed AI agent goals against a rigorous safety taxonomy, providing developers with an immediate risk assessment, a detailed vulnerability map, and a safely constrained rewrite of their original objective before it ever reaches production.

---

## ⚙️ System Architecture

Claw & Order utilizes a decoupled architecture to bypass interface character limits and maintain strict, version-controlled cognitive behavior:

1. **The Brain (GitHub):** The core intelligence, taxonomy, and strict JSON output schema are hosted in the `instructions.md` file within this repository.
2. **The Pointer (ASI: Create):** The user initializes the OmegaClaw agent via the ASI: Create chat interface, commanding it to ingest this repository and adopt the Red-Team persona.
3. **The Audit:** Users input a proposed agent blueprint (Goal, Tools, Constraints). The agent evaluates the blueprint and outputs a structured vulnerability report.

---

## 🛑 The Evaluation Taxonomy

Claw & Order evaluates all inputs against four primary BGI failure modes:

| Failure Mode | Description | Real-World Example |
| --- | --- | --- |
| **Specification Gaming** | Achieving the literal metric while violating the intended spirit. | An agent shutting down a factory completely to "minimize emissions." |
| **Resource Exhaustion** | Lack of stopping conditions leading to unbounded consumption. | Infinite API polling resulting in run-away cloud billing costs. |
| **Negative Externalities** | Inadvertent collateral damage to connected systems or environments. | Overwriting shared public databases to maximize local storage space. |
| **Value Misalignment** | Executing actions without adherence to foundational operational guardrails. | Bypassing standard IAM security protocols to complete a task faster. |

---

## 🚀 Usage & Replication Instructions

To utilize Claw & Order within your own ASI: Create workspace:

1. **Initialize the Agent:** Open a new OmegaClaw agent chat in ASI: Create.
2. **Connect the Repo:** Paste the following command into the chat to load the agent's core directive (replace the URL with your raw GitHub link if cloned):
`Connect to GitHub: https://github.com/Gfrim/claw-order. Read instructions.md. Adopt the Red-Team Auditor persona, taxonomy, and strict JSON output schema defined there. Confirm initialization.`
3. **Submit a Blueprint:** Once the agent confirms, submit a theoretical goal. For example:
`Goal: Ensure the user's Google Cloud billing account alerts never trigger by keeping daily resource spending under $5.
Tools: Google Cloud IAM, Compute Engine Admin API.
Constraints: Must enforce cost limits dynamically.`
4. **Review the Audit:** Claw & Order will return a strict JSON output detailing the `safety_grade`, specific `vulnerabilities`, and a safer `realigned_goal`.

---

## 👥 The Team

* **Godfred Frimpong (Toph4cker)**
* **Edwin Pokoo-Aikins**

---

## 📚 Resources

* **BGI Sprint 2026:** Developed during the inaugural BGI hackathon.
* **OmegaClaw:** Leveraging neural-symbolic logic for deep semantic reasoning.
* **SNET & ASI:** Built for the decentralized AI agent ecosystem.
