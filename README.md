# Rasa CALM "NLU/LLM-Hybrid" Demo

Demonstrates how to combine NLU-triggered flows with LLM-assisted dialog for regulated environments.

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

This project is licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

If you use, adapt, or redistribute this assistant in your own work, please include the following attribution:

    “This project is based on the rasa-calm-hybrid-demo assistant, originally created by Rasa Technologies, Inc. and licensed under CC BY 4.0.”

You must:

    Credit Rasa Technologies, Inc.
    Provide a link to this repository
    Indicate if changes were made (e.g., “Modified for internal use”)

Attribution can be included in your:

    README.md
    Course materials or documentation
    Application UI (if applicable)