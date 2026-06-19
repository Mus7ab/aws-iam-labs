# AWS IAM Labs

Hands-on AWS Identity and Access Management (IAM) labs documenting my journey learning cloud security fundamentals.

## What this covers

* Root account security and MFA setup
* IAM Users, Groups, and Roles
* AWS Managed vs Customer Managed Policies
* Inline policies and when to use them
* The Principle of Least Privilege
* ARNs and resource-level permissions
* Policy evaluation logic (deny overrides allow)

## Labs

| Lab                                            | Topic                                          | Status         |
| ---------------------------------------------- | ---------------------------------------------- | -------------- |
| [Lab 01](./labs/lab-01-root-account-security/) | Root account security & MFA                    | ✅ Complete     |
| [Lab 02](./labs/lab-02-create-iam-user/)       | Creating IAM users and enabling console access | ✅ Complete     |
| [Lab 03](./labs/lab-03-groups-and-policies/)   | Groups and attaching managed policies          | 🔄 In Progress |
| [Lab 04](./labs/lab-04-custom-policies/)       | Writing custom policies with least privilege   | ⏳ Upcoming     |
| [Lab 05](./labs/lab-05-iam-roles/)             | IAM Roles for EC2 and cross-account access     | ⏳ Upcoming     |

## Key concepts learned

**Policy evaluation order:**

1. Default DENY (everything starts blocked)
2. Explicit DENY wins over everything
3. Explicit ALLOW grants access
4. Default DENY if no allow found

**ARN format:**

```text
arn:partition:service:region:account-id:resource
```

**S3 gotcha:** Always need TWO ARNs in policy Resource:

* `arn:aws:s3:::my-bucket` — for ListBucket
* `arn:aws:s3:::my-bucket/*` — for GetObject/PutObject

## Environment

* AWS Free Tier account
* Region: ap-south-1 (Mumbai)
* AWS Console + AWS CLI

## Progress

Started: 20 June 2026

Target cert: AWS Solutions Architect Associate (SAA-C03)

---

*Learning in public. Follow my journey on: www.linkedin.com/in/musaab-mohamedani-3b2b72337 *
