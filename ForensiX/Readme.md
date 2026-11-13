# 🔍 ForensiX: A Modular Read-Only Toolkit for Digital Evidence Triage, Integrity Verification, and Investigation Reporting

<p align="center">
  <strong>A Python-Based Digital Forensics Research Project</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Domain-Digital%20Forensics-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Language-Python-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Database-SQLite-lightgrey?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Research%20Prototype-success?style=for-the-badge" />
</p>

## 📌 Overview

**ForensiX** is a modular, Python-based digital forensics toolkit designed for preliminary digital evidence triage, integrity verification, and investigation reporting.

The system integrates multiple forensic examination capabilities into a unified workflow, helping investigators inspect evidence files, generate cryptographic hashes, identify duplicate files, analyze file signatures, construct timelines, and maintain investigation records.

The project focuses on read-only evidence examination and structured documentation.

## 🎯 Research Objectives

- Automate recursive scanning of authorized evidence directories.
- Generate cryptographic hashes for evidence integrity verification.
- Identify file-signature and extension mismatches.
- Detect duplicate files using content hashes.
- Generate chronological timelines using file timestamps.
- Support optional YARA-based pattern scanning.
- Maintain investigation records using SQLite.
- Implement hash-linked chain-of-custody event records.
- Generate structured investigation reports.

## 🏗️ System Architecture

The ForensiX architecture consists of an examiner interface, command dispatcher, evidence examination modules, case management database, and report-generation components.

The workflow processes authorized evidence through multiple analysis modules before storing investigation records and generating reports.

## ⚙️ Key Modules

| Module | Description |
|---|---|
| File Scanner | Recursively scans evidence directories and collects file metadata. |
| Hash Engine | Generates MD5, SHA-1, and SHA-256 hashes. |
| File Signature Analysis | Detects supported file signatures and extension mismatches. |
| Duplicate Detection | Identifies duplicate files using content hashes. |
| Timeline Generation | Organizes available filesystem timestamps chronologically. |
| YARA Integration | Supports optional rule-based pattern scanning. |
| Case Management | Stores investigation details and custody records in SQLite. |
| Report Generation | Exports investigation results in JSON, CSV, and HTML formats. |

## 🛠️ Technology Stack

- **Programming Language:** Python
- **Database:** SQLite
- **Cryptographic Hashing:** SHA-256, SHA-1, MD5
- **Pattern Scanning:** YARA (optional)
- **Disk Image Support:** pytsk3 (optional, limited metadata support)
- **Report Formats:** JSON, CSV, HTML
- **Testing:** Pytest / unittest

## 🔐 Evidence Integrity and Chain of Custody

ForensiX uses cryptographic hashing to support evidence integrity verification.

Its chain-of-custody mechanism maintains investigation events in a hash-linked sequence. This allows changes to the recorded event sequence to be detected during verification.

The system is designed not to intentionally modify original evidence files during source-folder examination.

## 📊 Functional Evaluation

The prototype was evaluated using functional tests covering the following operations.

| Test Case | Result |
|---|---|
| File scanning and hash metadata | ✓ Pass |
| File-signature mismatch detection | ✓ Pass |
| Duplicate file grouping | ✓ Pass |
| Timeline generation | ✓ Pass |
| HTML report generation | ✓ Pass |
| Custody-chain verification | ✓ Pass |

All five test functions in the reported development test run passed.

## 📄 Research Paper

**Title:** ForensiX: A Modular Read-Only Toolkit for Digital Evidence Triage, Integrity Verification, and Investigation Reporting

**Author:** Chethana Sri

**Department:** Department of Computer Technology

**Institution:** Madras Institute of Technology, Anna University, Chennai, India

The research paper describes the system architecture, objectives, methodology, implementation, functional evaluation, security considerations, and limitations.

## ⚠️ Limitations

ForensiX is an educational and preliminary forensic triage prototype. It is not a replacement for validated forensic acquisition platforms.

The current implementation does not provide:

- Hardware or software write blocking.
- Full physical disk acquisition.
- Deleted-file recovery.
- Memory forensics.
- Network packet analysis.
- Digitally signed custody records.
- External trusted timestamping.
- Comprehensive file-signature coverage.

The optional disk-image integration is limited to basic metadata listing and does not provide complete filesystem traversal or deleted-file recovery.

The prototype has not undergone independent forensic tool validation and should not be described as court-certified.

## 🚀 Future Enhancements

- Independent forensic tool validation.
- Performance benchmarking and scalability testing.
- Expanded file-signature coverage.
- Complete disk-image analysis.
- Digitally signed chain-of-custody records.
- Enhanced investigation audit capabilities.

## 👩‍💻 Author

**Chethana Sri**  
Department of Computer Technology  
Madras Institute of Technology, Anna University  
Chennai, India

GitHub: [@Chethana45](https://github.com/Chethana45)

---

<p align="center">
  <strong>ForensiX — Structured Evidence. Verified Integrity. Reliable Investigation Records.</strong>
</p>
