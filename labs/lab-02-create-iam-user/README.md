# Lab 02 – Create IAM User

**Status:** ✅ Complete

## Objective

Create an IAM user with AWS Management Console access and understand how IAM users improve AWS account security compared to using the Root User.

## Tasks Completed

* Created an IAM Administrator user
* Enabled AWS Management Console access
* Assigned AdministratorAccess permissions
* Enabled MFA on the IAM user
* Successfully logged in using the IAM user
* Reviewed IAM Dashboard and account sign-in URL

## Evidence

Screenshots are stored in the `screenshots/` folder.

### IAM Dashboard

![IAM Dashboard](screenshots/01-iam-dashboard.png)

### IAM User Details

![IAM User Details](screenshots/02-iam-admin-user.png)

### AdministratorAccess Policy

![AdministratorAccess Policy](screenshots/03-admin-permissions.png)

### MFA Enabled

![MFA Enabled](screenshots/04-mfa-enabled.png)

## Key Learning

* IAM users provide individual identities for AWS access.
* MFA should be enabled for privileged accounts.
* The Root User should not be used for daily administration.
* Permissions can be assigned through policies and groups.
* AdministratorAccess grants full administrative permissions across AWS services.

## Result

An IAM Administrator user was created and secured with MFA, providing a safer alternative to daily use of the Root User account.
