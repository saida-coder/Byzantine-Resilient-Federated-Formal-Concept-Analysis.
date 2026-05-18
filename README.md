# 🛡️ BR-FedFCA  
## Byzantine-Resilient Federated Formal Concept Analysis

BR-FedFCA is a secure and trustworthy **Federated Formal Concept Analysis (FedFCA)** framework designed to protect distributed concept lattice aggregation against Byzantine and adversarial participants.

The framework enables multiple federated participants to collaboratively construct a global concept lattice **without sharing raw data**, while detecting malicious behaviors such as fake concept injection, support manipulation, confidence corruption, and collusion attacks.

---

# 📌 Global Architecture

![Global Architecture](Global%20architecture%20.png)

The BR-FedFCA architecture consists of two main components:

## 👥 Federated Participants

Each participant:

- 📂 Builds a local formal context
- 🔒 Applies privacy-preserving perturbation
- 🧠 Generates a local concept lattice
- 🔐 Encrypts local FCA outputs
- 📡 Sends encrypted lattices to the aggregation server

---

## 🖥️ Byzantine-Resilient Aggregation Server

The server:

- 🔓 Decrypts received lattices
- ✅ Performs structural FCA validation
- 📊 Computes support and confidence consistency
- 🧮 Calculates participant trust scores
- 🚫 Filters malicious participants
- 🗳️ Applies voting-based concept validation
- 🌐 Builds the trusted global concept lattice

---

# ✨ Main Features

- 🔒 Privacy-preserving Federated FCA
- 🛡️ Byzantine attack detection
- 📐 FCA closure property verification
- 📊 Support consistency analysis
- 📈 Confidence consistency analysis
- 🤝 Trust-aware aggregation
- 🗳️ Voting-based lattice validation
- 🌍 Global secure concept aggregation
- ⚡ Robustness under IID and Non-IID distributions

---

# ⚠️ Threat Model

BR-FedFCA considers several Byzantine attack scenarios:

- ❌ Fake concept injection
- 📉 Support manipulation
- 📈 Confidence manipulation
- 🧨 Invalid lattice generation
- 🤝 Collusion attacks between malicious participants

---

# 🧠 Baselines

The proposed framework is evaluated against:

| Method | Description |
|---|---|
| FedFCA | Standard federated FCA aggregation |
| FedFCA-Majority | Majority voting-based validation |
| FedFCA-Trust | Trust-aware participant validation |
| FedFCA-Filtered | Support-based participant filtering |
| 🛡️ BR-FedFCA | Proposed Byzantine-resilient framework |

---

# 📚 Datasets

## 🍄 Mushroom Dataset

- Objects: **8,124**
- Attributes: **119**
- Density: **0.193**
- Classification of mushroom edibility using categorical attributes.

---

## ♟️ Chess Dataset

- Objects: **3,196**
- Attributes: **75**
- Density: **0.487**
- Representation of chess endgame configurations.

---

# 📏 Evaluation Metrics

The framework is evaluated using:

- 📉 Support Error
- 📈 Confidence Error
- 🧩 Concept Preservation Rate (CPR)
- 🌐 Global Stability
