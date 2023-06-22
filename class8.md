# Access Control (ACL)

## 5 steps to RBAC

### 1.What is Role Based Access Control (RBAC) and why do we care?

RBAC is the idea of assigning system access to users based on their role within an organization. We are certainly being pushed in that direction of RBAC, with all of the major standards, including PCI DSS, HIPAA and Gramm-Leach-Bliley all requiring some form of it.

### 2.Describe a Role/Permission heirarchy that you might implement using RBAC.

The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment.

### 3.What approach might you take to implement RBAC?

1. Inventory your systems

Figure out what resources you have for which you need to control access, if you don't already have them listed.

2. Analyze your workforce and create roles

You need to group your workforce members into roles with common access needs.  Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible

3. Assign people to roles

Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly.

4. Never make one-off changes

Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary.

5. Audit

Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role.

## wiki - RBAC

### 1.If Authentication is “you are who you say you are,” what is Authorization?

It's basically giving rights to access certain pages and view them or to edit/create/delete other things as well.

### 2.Name three primary rules defined for RBAC.

1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.

2. Role authorization: A subject's active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.

3. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject's active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.

### 3.Describe RBAC to a non-technical friend.

It's a way of giving access to view or do certain things which is based on the roles attaches to that person.

## RBAC tutorial

### 1.What Are access rights Associated with? The User? or The Role? Explain.

The role of the user which was given to him based on his function in the organization, the role which determines what type of user this is.

### 2.Access Rights, or Authorization, is activated after a user successfully does what?

the users must be activated to one or more roles in order to get access rights.

### 3.Explain how RBAC might benefit a business.

It would benefit a business by organizing the users roles for them and giving them the least previlage to access resources in the organization which will basically implement a hierarchy based on access right to serve the organizaation.