# 🔐 AWS IAM Security Basics Project

This project demonstrates **AWS Identity and Access Management (IAM)** hands-on fundamentals.  
You will see how to securely grant and control access to AWS services using IAM Users, Groups, Policies, and MFA.

IAM is a core AWS security service used in **every** cloud project.

---

## 🎯 Objectives

✔ Create a limited-permission IAM user  
✔ Follow **least-privilege** best practice  
✔ Use IAM **group** to assign permissions  
✔ Test access restrictions to AWS services  
✔ Add **MFA** to strengthen security  
✔ Troubleshoot IAM permission errors

---

## 🧩 Architecture Overview

```mermaid
flowchart TD
    A[Admin User] --> B[IAM Group: S3ReadOnlyGroup]
    C[iam-demo-user] --> B
    B -->|Policy| D[S3 Read Only Access]
    C -->|MFA Enabled| E[Secure Login]
🛠️ Hands-on Task Summary
Action	Result
Create IAM user	iam-demo-user created
Create IAM group	S3ReadOnlyGroup created
Attach policy to group	AmazonS3ReadOnlyAccess
Add user to group	User inherits permissions
Login as IAM user	Console access granted
Test S3 access	Read only allowed
Enable MFA	Strong security enabled

📸 Screenshots
Upload these inside: iam-screenshots/ folder and keep the same names.

1️⃣ IAM User Created

2️⃣ IAM Group + S3 Read Only Policy Attached

3️⃣ Access Denied When No Permissions

4️⃣ Access Allowed After Adding to Group

5️⃣ MFA Enabled for IAM User

🧠 Key Learnings
IAM users do not have permissions by default

Permissions should be added via groups (industry standard)

Least privilege principle keeps accounts safe

IAM policies control access on service, resource, and action level

MFA adds second layer of authentication security

Practical troubleshooting process is important in cloud environments

🔒 Best Security Practices Learned
✔ Never use root account for daily work
✔ Enable MFA for every IAM user
✔ Use IAM groups for permission control
✔ Restrict permissions to minimum required
✔ Review and monitor access regularly

📦 Technologies Used
AWS Service	Purpose
IAM	Access control & user authentication
S3	Target service for permission testing
MFA	Identity protection

🚀 Future Enhancements
IAM Roles for EC2 Access

IAM Password Policy Enforcement

AWS CloudTrail for Access Logging

Custom inline IAM policies

JSON policy deployment using CLI / Terraform

🌟 Why This Project is Important
IAM is the foundation of Cloud Security.
Every AWS professional must understand how to manage identity and access.

This project shows real-world security configuration steps practiced in companies globally.

👩‍💻 Created by: Srimahalakshmi R
Aspiring Cloud Engineer | AWS Security Learner ✨

⭐ If you found this helpful, give the repo a star!
