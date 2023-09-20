# AWS Organizations

AWS Organizations is an account management service that enables you to consolidate multiple AWS accounts into an *organization* that you create and centrally manage.

## AWS Organizations terminology and concepts

The following diagram shows a basic organization that consists of five accounts that are organized into four organizational units (OUs) under the root. The organization also has several policies that are attached to some of the OUs or directly to accounts.

![](../imgs/AWS-Organizations-and-AWS-Account-Management/AccountOuDiagram.png)

- Organization

    An entity that you create to consolidate your AWS accounts so that you can administer them as a single unit. An organization has one management account along with zero or more member accounts.

- Root

    The parent container for all the accounts for your organization. If you apply a policy to the root, it applies to all organizational units (OUs) and accounts in the organization.

    > Currently, you can have only one root. AWS Organizations automatically creates it for you when you create an organization.

- Organizational unit (OU)

    A container for accounts within a root. An OU can have exactly one parent, and currently each account can be a member of exactly one OU.

- Account

    An account in Organizations is a standard AWS account that contains your AWS resources and the identities that can access those resources.

    - management account
    - Member accounts

    > An AWS account isn't the same thing as a user account.

- Delegated administrator

    - Delegated administrator for Organizations
    - Delegated administrator for an AWS service

- Available feature sets

    - All features
    - Consolidated billing
    
## Service control policies (SCPs)

Service control policies (SCPs) are a type of organization policy that you can use to manage permissions in your organization.

SCPs are similar to IAM permissions policies except that they don't grant any permissions. Instead, SCPs specify the maximum permissions for an organization, organizational unit (OU), or account.

> SCPs don't affect users or roles in the management account. They affect only the member accounts in your organization.

## Management policies

- Service control policy (SCP)
- Artificial intelligence (AI) services opt-out policy
- Backup policy
- Tag policy

# AWS Account Management
