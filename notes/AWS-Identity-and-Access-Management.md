# IAM

## IAM Identities (users, user groups, and roles)

- AWS account root user

    When you first create an AWS account, you begin with one sign-in identity that has complete access to all AWS services and resources in the account. This identity is called the AWS account *root user* and is accessed by signing in with the email address and password that you used to create the account.

- IAM users

    An IAM user is an identity within your AWS account that has specific permissions for a single person or application.

- IAM user groups

    An IAM group is an identity that specifies a collection of IAM users.

- IAM roles

    An IAM role is an IAM identity that you can create in your account that has specific permissions. An IAM role is similar to an IAM user, in that it is an AWS identity with permission policies that determine what the identity can and cannot do in AWS. However, instead of being uniquely associated with one person, a role is intended to be assumable by anyone who needs it. Also, a role does not have standard long-term credentials such as a password or access keys associated with it. Instead, when you assume a role, it provides you with temporary security credentials for your role session.
