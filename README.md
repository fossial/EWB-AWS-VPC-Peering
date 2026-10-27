# AWS VPC Peering Project — EWB Courses

**Submitted by:** Md Saqeeb Afridi  
**Batch:** 1  
**AWS Region:** Asia Pacific (Mumbai) — `ap-south-1`  
**Project:** AWS VPC Peering and Private Connectivity

## 1. Project Overview

This project demonstrates how to connect two separate Amazon Virtual Private Clouds (VPCs) using VPC Peering and verify private network connectivity between EC2 instances.

## 2. Network Architecture

- **VPC A:** `10.30.0.0/16`
- **VPC B:** `10.40.0.0/16`
- **Peering connection:** `ewb-a-b-peer`
- **Region:** `ap-south-1` (Mumbai)

## 3. Main Tasks

- Created VPCs and configured subnets.
- Configured route tables and subnet associations.
- Created and activated a VPC peering connection.
- Configured security group rules.
- Tested connectivity between private EC2 instances.
- Connected to App-B using SSH through the bastion host.
- Created an IAM Access Analyzer and downloaded the IAM credential report.

## 4. Project Evidence

- **Final project report:** `Md_Saqeeb_Afridi_EWB_VPC_Peering_final.pdf`
- **Screenshots:** See the `ewb seperate images` folder for supporting AWS console and terminal evidence.

## 5. Testing

Connectivity between the private instances was verified using ping tests. SSH access to App-B through the bastion host was also tested successfully.

Refer to the project report and screenshots for the recorded test results.

## 6. Learning Outcomes

- Understanding VPCs, subnets, route tables and VPC Peering.
- Configuring security groups for private connectivity.
- Testing network paths between private instances.
- Using IAM Access Analyzer and generating an IAM credential report.

## 7. Security Note

Private keys, passwords, access tokens and other sensitive credentials are not included in this repository.

---

**Project completed as part of the EWB Courses AWS project.**
