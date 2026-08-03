# Basic Employee Onboarding (AD)(RBAC)
 
## Problem Statement
Before this project, the problem was Northstar Medical group, a sample healthcare company that relied on an MSP to manage its IT operations. As the company grew, the MSP struggled to keep everything organized, and user accounts and permissions were managed manually. Since Northstar Medical Group handles sensitive patient information, the lack of structure and poor account management created a serious HIPAA compliance and security risk.

 
## Solution Overview
The solution was to build out a basic employee onboarding pipeline in active directory. I set up the RBAC matrix and ensured users were given access ONLY according to their role. I also simulated a mock where a user was provisioned the incorrect level of access!

## Video Walkthrough
[Add your video walkthrough link placeholder here. You will record this tomorrow and update this link so visitors can see a live demonstration of your lab environment.]

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* Implemented RBAC with security groups mapped to each department
* Diagnosed and resolved a multi-cause access issue (wrong OU + missing group membership)
