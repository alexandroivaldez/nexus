# IAM

**AWS Identity and Access Management (IAM)** helps you control access to AWS resources, who is allowed to sign in and what resources they can access.

## Key Concepts

1. **Users**  
   - Represents a single individual.

2. **Groups**  
   - A collection of users.
   - Users inside of a group inherit policies attached to the group.
   - A user can belong to multiple groups, but a group can not have a nested group.

3. **Roles**  
   - Used to grant temporary access to AWS resources.
        - For example, giving a lambda a role to access files in S3.

4. **Policies**  
   - JSON documents defining permissions.  
   - Types:  
     - **AWS Managed Policies**: Predefined by AWS.  
     - **Customer Managed Policies**: Created and managed by you.  
     - **Inline Policies**: Embedded directly in a user, group, or role.

5. **Identity Providers**  
   - Allow external authentication using SAML 2.0 or Single Sign-On (SSO) setups.

## Best Practices

1. **Follow the Principle of Least Privilege**  
   - Grant only the permissions necessary for a task, and nothing more.  

2. **Enable Multi-Factor Authentication (MFA)**  
   - Require MFA for critical operations and privileged accounts.

3. **Never use root user**
    - Create a new user account with admin privileges instead.

## Tools for IAM Management

1. **IAM Access Analyzer**  
   - Detect overly permissive access and unused permissions.

2. **IAM Credentials Report**
   - A feature that provides a detailed, account-wide report about the status of AWS credentials for all IAM users.
