# IAM: Users and Groups

+ IAM = Identity and Access Management, Global Service
+ **Root account** created by default, shouldn't used or shared
+ **Users** are ppl within your org, and can be grouped
+ **Group** can't be nested, groups can contain only users.
+ **Users** don't have to belong to a group, and user can belong to multiple groups

---

# IAM: Permissions
+ **Users and Groups** can be assigned JSON documents called **policies**
+ These policies define the permissions of a **user**
+ **least privilege principle**: don't give more permissions than user needs

---

# IAM: Hands on
+ Create new Group with policy AdministratorAccess
+ Create a new IAM user and add him to above gorup with AdminAccess
+ Use the newly created user rather than root user
+ Update account alias so that one can use text rather than number
+ After that new sign-in url for IAM user is available which can used by IAM user to login

---

# IAM: Policy
+ Policy of the group will be inherited by all the users in that group
+ If the user is part of multiple groups, policies from both group will be applicable to user
+ AdministratorAccess for admin access : access to all the resources
+ IAMReadOnlyAccess which permits read only permissions for all the aws services/resources

---

# IAM: Policy Structure
Consists of Version, ID and Statements
+ **Version**: policy language version, always include "2010-10-17"
+ **Id**: an identifier for the policy (optional)
+ **Statement**: one or more individual statements(required)

Statements consists of:
+ **Sid**: identifier of the statement(optional)
+ **Effect**: whether statement allows or denies access(Allow/Deny)
+ **Policy**: user/account/role to which this policy applied to
+ **Action**: list of actions this policy allows or denies
+ **Resource**: list of resources to which this action applied to
+ **Condition**: conditions for when this policy is in effect(optional)
Inline-style: 
![alt text](https://github.com/GurikR/AWS/blob/main/policy-example.PNG "Policy")

---
