# Identity and Access Management

- Root account should not be used. Create users instead
- Users are people within the organization
- Users can be grouped
- Groups only contain users
- Users can be part of multiple groups

### Permissions

*Use least priviledge principal - only the permission that the user needs*

- Policies are a set of permissions over services
- Polcies can be attached to a group or to a single user
- Adding a policy to a group makes all the users in the group have those policy permissions

### Roles

- IAM Roles are intended to be used for services to communicate between over AWS.
i.e → A service running on a EC2 instance trying to put a message on an SQS queue
i.e → A Lambda trying to access a DynamoDB table

### Tools

- Credentials report: just that, reports from IAM
- Access Advisor: From a user page, to see which and when each of AWS services where accessed by the user

### Best Practices

- Enforce MFA
- One physical user - One AWS account
- Use password policy
- Use roles for managing AWS services permissions (like EC2 or Lambda, but any)
