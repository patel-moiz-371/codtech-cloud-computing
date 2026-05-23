# ☁️ CodTech Cloud Computing Internship Portfolio

Welcome to my cloud computing repository! This project documents the complete architecture, deployment, monitoring, and security strategies implemented during my cloud infrastructure internship. Every milestone is built following industry best practices like the Principle of Least Privilege (PoLP) and highly available disaster recovery workflows.

---

## 📁 Repository Structure

```text
codtech-cloud-computing/
│
├── 📁 Task1-Cloud-Storage/
│   ├── 📄 test-file.txt
│   ├── 📄 README.md
│   └── 📁 screenshots/
│       ├── 🖼️ bucket-setup.png
│       └── 🖼️ permissions-check.png
│
├── 📁 Task2-Monitoring/
│   ├── 📄 README.md
│   └── 📁 screenshots/
│       ├── 🖼️ metrics-dashboard.png
│       └── 🖼️ alarm-config.png
│
├── 📁 Task3-Multi-Cloud/
│   ├── 📄 README.md
│   └── 📄 sync_script.py
│
└── 📁 Task4-Security/
    ├── 📄 README.md
    └── 📁 screenshots/
        ├── 🖼️ encryption-audit.png
        └── 🖼️ iam-policy.png
🚀 Progress TrackerTaskDescriptionStatusTask 1Cloud Storage Setup (AWS S3)🟢 CompletedTask 2Cloud Monitoring & Alerts🟢 CompletedTask 3Multi-Cloud Architecture🟢 CompletedTask 4Cloud Security Implementation🟢 Completed🛠️ Infrastructure Overview🔹 Task 1: Cloud Storage SetupDeployed a global, private object storage instance utilizing Amazon S3. Configured explicit block public access controls, maintaining an entirely locked down environment to eliminate common cloud data leak vectors.🔹 Task 2: Cloud Monitoring & AlertsBuilt an automated health monitoring system using Amazon CloudWatch. Engineered metric tracking loops to observe object changes, resource requests, and set up precise alarm systems for instant operational awareness.🔹 Task 3: Multi-Cloud ArchitectureDeveloped an automated Python synchronization script (sync_script.py) utilizing cloud APIs to stage and move objects from a primary provider environment over to an isolated staging directory, laying the foundation for heterogeneous cross-cloud disaster recovery failovers.🔹 Task 4: Cloud Security ImplementationHardened storage assets using Server-Side Encryption with Amazon S3 managed keys (SSE-S3) running standard AES-256 protocols. Decoupled root privileges by provisioning an audited, restricted IAM user policy limiting runtime access exclusively to read-only actions.
