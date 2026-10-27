# AWS VPC Peering Project — EWB Courses

**Submitted by:** Md Saqeeb Afridi  
**Batch:** 1  
**AWS Region:** Asia Pacific (Mumbai) — `ap-south-1`  
**Project:** AWS VPC Peering and Private Connectivity

---

## 1. Project Overview

This project demonstrates how to connect two separate Amazon Virtual Private Clouds (VPCs) using **AWS VPC Peering** and verify private network connectivity between EC2 instances.

The project focuses on creating VPCs and subnets, configuring route tables, establishing a VPC peering connection, managing security group rules, testing connectivity, and reviewing IAM security information.

## 2. Network Architecture

The project uses two VPCs in the Mumbai AWS Region.

| Component | Configuration |
|---|---|
| AWS Region | `ap-south-1` (Mumbai) |
| VPC A CIDR | `10.30.0.0/16` |
| VPC B CIDR | `10.40.0.0/16` |
| Peering Connection | `ewb-a-b-peer` |
| Peering Connection ID | `pcx-0664d194a986e4999` |
| Bastion Host Private IP | `10.30.1.177` |
| Bastion Host Public IP | `13.201.10.81` |
| App A Private IP | `10.30.2.58` |
| App B Private IP | `10.40.1.117` |

The VPC peering connection was created to enable private communication between resources in the two VPCs. Appropriate routes and security group rules are required for connectivity.

## 3. Main Tasks Completed

- Created and configured VPCs in the Mumbai AWS Region.
- Configured public and private subnets.
- Created and configured route tables and subnet associations.
- Created and activated the VPC peering connection.
- Configured security group inbound and outbound rules.
- Launched EC2 instances for the lab environment.
- Configured a bastion host for SSH access.
- Tested private connectivity between EC2 instances.
- Connected to App B through the bastion host using SSH.
- Created an IAM Access Analyzer.
- Generated and downloaded the IAM credential report.

## 4. Project Files and Evidence

The project repository contains the following supporting materials:

- **Final project report:** `Md_Saqeeb_Afridi_EWB_VPC_Peering_final.pdf`
- **Screenshot folder:** `ewb seperate images`
- **README:** `README.md`

The screenshots below provide supporting evidence of AWS configuration, routing, security settings, connectivity testing, and IAM security monitoring.

---

## 5. Project Screenshots and Evidence

The screenshots are referenced using their existing filenames, `img0.jpg` through `img50.jpg`, so the files do not need to be renamed.

### 5.1 EC2 Instances, Network Interfaces, and Security Groups

**Screenshots:** `img0.jpg` – `img16.jpg`, and `img19.jpg`

These screenshots document:

- EC2 instance status and configuration.
- Network interface and attachment details.
- App B security group inbound and outbound rules.
- Bastion host security group configuration.
- App B network ACL rules.
- Private instance networking details.
- Instance Connect limitations and connection troubleshooting.

### 5.2 VPC Peering and Route Table Configuration

**Screenshots:** `img18.jpg`, `img20.jpg` – `img23.jpg`, and `img27.jpg` – `img39.jpg`

These screenshots document:

- VPC peering connection status and details.
- Route table configuration.
- Routes associated with the peering connection.
- Public and private route table settings.
- Subnet associations.
- Security group adjustments related to private connectivity.

The peering connection is shown as active in the relevant screenshots.

### 5.3 Connectivity Testing and Troubleshooting

**Screenshots:** `img17.jpg`, and `img24.jpg` – `img26.jpg`

These screenshots document the connectivity tests performed during the project.

- `img17.jpg` — Shows a successful ping to App A and an unsuccessful ping to App B at that stage of testing.
- `img24.jpg` — Shows a successful ping test from the bastion environment to App A.
- `img25.jpg` — Shows an unsuccessful connectivity test between App B and App A during troubleshooting.
- `img26.jpg` — Shows successful connectivity after troubleshooting.

These screenshots preserve the progression of testing, including both intermediate failures and subsequent successful results.

### 5.4 IAM Security and Access Analyzer

**Screenshots:** `img40.jpg` – `img50.jpg`

These screenshots document:

- IAM dashboard and root account security information.
- Access Analyzer configuration and creation.
- Access Analyzer findings and resource analysis.
- Credential report generation.
- Security monitoring pages and analysis summaries.

The screenshots show the recorded state of the relevant IAM and security pages at the time they were captured.

---

## 6. Connectivity Testing

Connectivity was tested between the private EC2 instances using ping commands. The screenshots document the troubleshooting process and the successful results obtained after configuration changes.

SSH access to App B through the bastion host was also tested successfully.

The project demonstrates the importance of checking the following when troubleshooting VPC peering connectivity:

- VPC CIDR ranges and subnet configuration.
- Route tables and peering routes.
- Security group inbound and outbound rules.
- Network ACL rules.
- SSH access configuration.
- Correct private IP addresses and network paths.

Refer to the project report and screenshots for the supporting evidence of the individual tests.

## 7. IAM Security Review

As part of the project, IAM security-related pages were reviewed.

The completed activities included:

- Creating an IAM Access Analyzer.
- Reviewing the analyzer status and displayed findings.
- Generating and downloading the IAM credential report.
- Reviewing the available IAM security information.

These activities provided practical exposure to AWS IAM security monitoring and credential reporting.

## 8. Learning Outcomes

Through this project, I gained practical experience with:

- AWS VPC creation and configuration.
- Public and private subnet concepts.
- Route tables and subnet associations.
- VPC peering and private network communication.
- EC2 instance deployment and networking.
- Bastion host SSH access.
- Security groups and network ACLs.
- Connectivity testing and troubleshooting.
- IAM Access Analyzer and credential reports.
- Documenting AWS infrastructure using screenshots and a project report.

## 9. Security Notes

Security and privacy are important when publishing AWS project documentation.

- Private keys, passwords, access tokens, secret access keys, and other credentials must not be included in this repository.
- The EC2 private key file, `ewb-lab.pem`, should remain private and must never be uploaded to GitHub.
- Review screenshots before publishing them. Redact the 12-digit AWS account ID, account email, and other personal or account-identifying details where visible.
- Do not publish credentials or sensitive information from AWS console pages or terminal output.
- Security group rules should follow the principle of least privilege.

## 10. Conclusion

This project provided hands-on experience with AWS VPC peering, private network connectivity, EC2 instance configuration, route table management, security group configuration, and connectivity troubleshooting.

It also introduced IAM security review activities through Access Analyzer and credential report generation.

The project report and supporting screenshots document the configuration process, troubleshooting steps, and results observed during the lab.

---

**Project completed as part of the EWB Courses AWS project.**
