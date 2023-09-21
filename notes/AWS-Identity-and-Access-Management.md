# IAM

## IAM terms

These IAM terms are commonly used when working with AWS:

- IAM Resources

    The user, group, role, policy, and identity provider objects that are stored in IAM. As with other AWS services, you can add, edit, and remove resources from IAM.

- IAM Identities

    The IAM resource objects that are used to identify and group. You can attach a policy to an IAM identity. These include users, groups, and roles.

- IAM Entities

    The IAM resource objects that AWS uses for authentication. These include IAM users and roles.

- Principals

    A person or application that uses the AWS account root user, an IAM user, or an IAM role to sign in and make requests to AWS. Principals include federated users and assumed roles.

- Human users

    Also known as human identities; the people, administrators, developers, operators, and consumers of your applications.

- Workload

    A collection of resources and code that delivers business value, such as an application or backend process. Can include applications, operational tools, and components.

## IAM Identities (users, user groups, and roles)

- AWS account root user

    When you first create an AWS account, you begin with one sign-in identity that has complete access to all AWS services and resources in the account. This identity is called the AWS account *root user* and is accessed by signing in with the email address and password that you used to create the account.

- IAM users

    An IAM user is an identity within your AWS account that has specific permissions for a single person or application.

- IAM user groups

    An IAM group is an identity that specifies a collection of IAM users.

- IAM roles

    An IAM role is an IAM identity that you can create in your account that has specific permissions. An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it. Also, a role does not have standard long-term credentials such as a password or access keys associated with it. Instead, when you assume a role, it provides you with temporary security credentials for your role session.

## Policies and permissions in IAM

You manage access in AWS by creating policies and attaching them to IAM identities (users, groups of users, or roles) or AWS resources. A policy is an object in AWS that, when associated with an identity or resource, defines their permissions.

- Identity-based policies

    Identity-based policies are JSON permissions policy documents that control what actions an identity (users, groups of users, and roles) can perform, on which resources, and under what conditions.
    
    Identity-based policies can be further categorized:

    - Managed policies
    
        Standalone identity-based policies that you can attach to multiple users, groups, and roles in your AWS account.

        - AWS managed policies
        - Customer managed policies
    
    - Inline policies

        Policies that you add directly to a single user, group, or role. Inline policies maintain a strict one-to-one relationship between a policy and an identity.

- Resource-based policies

    Resource-based policies are JSON policy documents that you attach to a resource such as an Amazon S3 bucket. These policies grant the specified principal permission to perform specific actions on that resource and defines under what conditions this applies. Resource-based policies are inline policies. There are no managed resource-based policies.

- Permissions boundaries

    A permissions boundary is an advanced feature in which you set the maximum permissions that an identity-based policy can grant to an IAM entity. When you set a permissions boundary for an entity, the entity can perform only the actions that are allowed by both its identity-based policies and its permissions boundaries. Resource-based policies that specify the user or role as the principal are not limited by the permissions boundary. An explicit deny in any of these policies overrides the allow.

- Organizations SCPs

    SCPs are JSON policies that specify the maximum permissions for an organization or organizational unit (OU). The SCP limits permissions for entities in member accounts, including each AWS account root user. An explicit deny in any of these policies overrides the allow.

- Access control lists (ACLs)

    Access control lists (ACLs) are service policies that allow you to control which principals in another account can access a resource. ACLs cannot be used to control access for a principal within the same account.

- Session policies

    Session policies are advanced policies that you pass as a parameter when you programmatically create a temporary session for a role or federated user.
