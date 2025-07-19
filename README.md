---
title: "🔐 PasswordStore Protocol Audit"
date: "July 17, 2025"
author: "Abdullahi Naqeeb Salati"
repository: "https://github.com/naqeebsalati/19-07-2025-PasswordStore-Audit-report.pdf"
---


## 📄 About This Repository

This repository contains a detailed **security audit report** for the `PasswordStore` smart contract protocol. The audit was conducted to evaluate the security posture, identify vulnerabilities, and recommend mitigations to improve the security of the contract. This report demonstrates my technical expertise in smart contract auditing, vulnerability analysis, and reporting.

---

## 📌 Audit Report Summary

### 🔎 Protocol Audited

**PasswordStore**: A protocol dedicated to the storage and retrieval of a user's passwords, intended for single-user ownership.

### 📊 Key Audit Results

| Severity          | Issues Found |
| ----------------- | ------------ |
| High              | 2            |
| Medium            | 0            |
| Low               | 1            |
| Informational     | 1            |
| Gas Optimizations | 0            |

---

## 🚩 Notable High-Risk Findings

### \[H-1] Password Stored On-Chain in Plaintext

* **Issue**: Password is stored on-chain in plaintext, exposing it to public access.
* **Impact**: Breaks the core security of the protocol.
* **Recommendation**: Use `keccak256` hashing to store passwords securely.

### \[H-2] Missing Access Controls on `setPassword`

* **Issue**: Anyone can call `setPassword` and overwrite the password.
* **Impact**: Allows unauthorized modification of sensitive data.
* **Recommendation**: Restrict this function to the contract owner only.

---

## 📂 Report Details

* **Audit Date**: July 17, 2025
* **Commit Hash Reviewed**: `2e8f81e263b3a9d18fab4fb5c46805ffc10a9990`
* **Scope**: `src/PasswordStore.sol`
* **Lead Security Researcher**: Abdullahi Naqeeb Salati

---

## ⚠️ Disclaimer

This audit was time-boxed and focused solely on the security of the Solidity smart contract implementation. This audit is not an endorsement of the underlying business or product.

---

## 🛡️ Why This Matters

This repository is part of my public **security audit portfolio** to demonstrate my professional experience and skills in identifying vulnerabilities and writing high-quality security reports for blockchain projects.

---

## 📎 Report PDF

You can download and read the full detailed audit report here:
➡️ **[2025-07-17 PasswordStore Audit Report.pdf](./19-07-2025-PasswordStore-Audit-report.pdf)**

---

