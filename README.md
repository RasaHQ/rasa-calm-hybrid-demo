# Rasa CALM "NLU/LLM-Hybrid" Demo

Demonstrates how to combine NLU-triggered flows with LLM-assisted dialog for regulated environments.

*NOTE: Implementation approach & project details may be adjusted based on testing outcomes and evolving priorities.*

---

## 🔑 Key Features

- 🧩 **Modular CALM Flows** — Each use case is represented as a structured YAML flow with shared subflows.
- 🤖 **Hybrid Architecture** — Combines NLU-only flows with selective LLM integrations.
- 🧪 **Testable Design** — Includes end-to-end tests for verifying core interactions.
- 📚 **Realistic Financial Use Cases** — Covers account balance, card replacement, disputes, fees, and more.
---

## 📁 Included Use Cases

- `nlu_account_balance`
- `nlu_update_settings`
- `nlu_card_replace`
- `nlu_dispute_transaction`
- `nlu_atm_find`
- `nlu_contact_us`
- `nlu_fees_interest_inquiry`

---

## 🏗️ Basic Project Structure
```
rasa-calm-hybrid-demo/
├── actions/
├── data/
│   ├── flows/
│   │   ├── flow-<use_case>.yml
│   │   ├── patterns.yml
│   │   └── subflows/
│   │       ├── _shared/
│   │       └── <use_case>/...
│   └── nlu/
│       ├── general/
│       └── triggers/
│           └── nlu-<use_case>.yml
├── domain/
│   ├── global_domain.yml
│   └── domain_use_cases/
│       └── <use_case>/
│           ├── dr-<use_case>.yml
│           └── ds-<use_case>.yml
├── tests/
│   └── e2e_test_cases.yml
└── config.yml + endpoints.yml + README.md
```

---

## 🔧 Requirements
```commandline
Rasa Pro Version  :         3.12.5
Minimum Compatible Version: 3.11.0rc1
Rasa SDK Version  :         3.12.0
Python Version    :         3.10.13
pip Version       :         25.0.1
```

Install dependencies:

```bash
pip install --upgrade pip
pip install uv
uv pip install rasa-pro  # Rasa Pro License required
```

## 🪪 Licensing

[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC--BY--NC%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc/4.0/)
🧾 Attribution for Users
