# Task 4: Cloud Security Implementation Report

## Project Overview
This project details the tactical security controls applied to a cloud-native storage infrastructure using Amazon Web Services (AWS). This architecture follows the industry standard Principle of Least Privilege (PoLP) and Zero-Trust principles to secure sensitive assets at rest and in transit.

---

## 🛡️ Security Implementation Details

### 1. Data Encryption (Data-at-Rest Protection)
To ensure compliance and data confidentiality, server-side encryption was deployed on the core data repository.
* **Mechanism:** Server-side encryption with Amazon S3 managed keys (`SSE-S3`).
* **Cryptographic Protocol:** Advanced Encryption Standard (AES-256).
* **Impact:** Every object written to the bucket is automatically encrypted before being saved to disk and decrypted seamlessly upon authorized retrieval.

### 2. IAM Policy Implementation (Access Control)
To minimize operational risk, a dedicated administrative IAM user was created to handle read-only data operations. Direct usage of the root AWS account was successfully decoupled from ordinary runtime processes.
* **User Identity:** `S3-Data-Auditor`
* **Policy Attached:** `AmazonS3ReadOnlyAccess` (AWS Managed Policy)
* **Scope of Control:** Grants permissions to list and read objects across Amazon S3 storage buckets while completely blocking mutations (deletes, writes) and prohibiting access to critical account configurations or billing dashboards.

### 3. Secure Storage Configuration (Network Security)
* **Public Access Block:** Active global policy enforcement blocks all public Access Control Lists (ACLs) and explicit bucket policies, preventing unintended internet leakage.

---

## 📊 Deliverables & Proof of Configuration
- **S3 Default Encryption Status:** Verified via console audit trails.
- **IAM Identity Attachment:** Active configuration map validates restricted role assignment.
- *(Screenshots demonstrating implementation are tracked inside the `/screenshots` directory).*
