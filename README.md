# Engineering Manifesto

This repository serves as the foundational framework for my work at the intersection of Networking, Cloud and AI. 

These are not abstract guidelines; they are the **load-bearing architectural constraints** I use to ensure that high-autonomy systems remain safe, deterministic and observable. 

---

## 🏗️ Core Frameworks

| Domain | Philosophical Anchor | Primary Specification |
| :--- | :--- | :--- |
| **Software** | "Simplicity is a design decision. Earn every layer of complexity." | [Software Principles](./sw-engineering-principles.md) |
| **Networking** | "The wire doesn't lie. Trust higher-fidelity evidence when sources conflict." | [Network Principles](./nw-engineering-principles.md) |

---

## 🧠 The "Thinker/Doer" Pillars

These three principles define my approach to building agentic tools for critical infrastructure:

### 1. AI is a Reasoning Layer, Not a Data Layer
I do not believe in "Black Box" forensics. I never send raw, uncompressed data to a model. There should be systems to preprocess, aggregate, and reduce data before piping that into the AI brain. This ensures that the AI Brain performs high-level reasoning over structured truth rather random noise. 

### 2. Deterministic Safety Over Probabilistic Safety
In production networking, the safety gate must be a code path, not a prompt. I architect systems where AI proposes an action, but mechanisms like allowlists, verb-matching and pattern rules framed by humans decide if it is safe to execute.

### 3. Model the Path Before the Command
An investigation without a model is just guessing in sequence. I build tools that map the expected network layers—DNS, Routing, Access Control—and verify effective state at the enforcement point rather than trusting configured intent.

---

## 🛠️ Applied Engineering

To see these principles implemented in a production-grade environment, explore the **Network Ghost Agent** project:

* **[Network Ghost Agent](https://github.com/ranga-sampath/agentic-network-tools/tree/main/agentic-network-ghost-troubleshooter):** An autonomous Azure forensics investigator that encodes senior engineering methodology into a secure, auditable loop.
* **[Safe-Exec Shell](https://github.com/ranga-sampath/agentic-network-tools/tree/main/agentic-safety-shell):** A 4-tier structural gate that enforces human-in-the-loop (HITL) safety for every agentic command.
* **[PCAP Forensic Engine](https://github.com/ranga-sampath/agentic-network-tools/tree/main/agentic-pcap-forensic-engine):** AI-powered wire-analysis that reduces binary captures by 95% for rapid root-cause diagnosis.

---
"An investigation accumulates and weighs evidence; it does not short-circuit on the first result."
