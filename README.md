# Basic Employee Onboarding (AD)(RBAC)

Active Directory infrastructure rebuild for a fictional healthcare company, Northstar Medical Group, covering domain setup, user provisioning, RBAC, and incident resolution.

## Problem Statement

Before this project, Northstar Medical Group relied on an MSP to manage its IT operations. As the company grew, that setup stopped scaling:

- **Disorganized accounts and permissions.** There was no consistent structure for how users were created or what they could access, so permissions were hard to audit.
- **Manual onboarding.** New hires were set up by hand each time, which meant inconsistent access depending on who handled the request.
- **Inactive accounts left enabled.** Accounts weren't always disabled after employees left the company, leaving unused credentials that could be misused.

Because Northstar is a healthcare organization, these gaps weren't just an IT inconvenience. Excess or lingering access to systems that may touch patient data creates real security risk and puts the company's HIPAA compliance at stake. The company needed a structured, repeatable way to give people the access their job requires, and nothing more.

## Solution Overview

I rebuilt the identity foundation in Active Directory and designed a basic onboarding pipeline around it:

1. **Built the environment.** I created the NMG.com domain from scratch and promoted the domain controller.
2. **Designed the structure.** I organized users with a clean OU hierarchy and created security groups mapped to each department.
3. **Applied RBAC.** I built an RBAC matrix so access is assigned through role-based group membership instead of one-off permissions. Users receive access only according to their role, following the principle of least privilege.
4. **Provisioned users.** I onboarded users into the correct OUs and groups so access is consistent and repeatable.
5. **Tested it with a real scenario.** I simulated incident NMG-0047, where a user was provisioned the wrong level of access. The cause wasn't a single mistake: the account was in the wrong OU and was also missing the correct group membership. I traced both causes, corrected them, and documented the resolution.

The result is an onboarding process where access is predictable, auditable, and tied to job role, which is what a healthcare environment needs.

## Video Walkthrough

[▶ Watch the walkthrough on Loom](https://www.loom.com/share/e192e5a74fdf4f498814f7dd6159348f)

## Tools Used

- Windows Server
- Active Directory Domain Services
- VirtualBox
- UTM
- RBAC
- GitHub

## Project Timeline

- **Day 1:** Domain creation and domain controller promotion
- **Day 2:** Organizational unit and security group design
- **Day 3:** User provisioning and RBAC implementation
- **Day 4:** Incident response and resolution (NMG-0047)
- **Day 5:** Documentation and case study packaging

## Key Accomplishments

- Built the NMG.com domain from scratch
- Implemented RBAC with security groups mapped to each department
- Diagnosed and resolved a multi-cause access issue (wrong OU + missing group membership)

## Skills Demonstrated

Active Directory administration, OU and security group design, role-based access control, least privilege, access troubleshooting, incident documentation

## Project Files

- [Documentation](./Documentation)
- [Incident Reports](./Incident-Reports) (including NMG-0047)
- [Screenshots](./Screenshots)
