---
title: Access Control - AAD User
description: Learn how to set Access Control for an Azure Active Directory Organization User for use in RCL applications
parent: Authorization
nav_order: 3
---

# Set Access Control for the AAD user

The Azure Active Directory (AAD) organization user account (Work or School) that you use to login to RCL apps must either be :

- An 'Administrator' or 'Owner' to your Azure subscription
- Have a role of ‘Owner’ or ‘Contributor’ to your Azure subscription

If either of these requirements are not met, you will not be able to use RCL apps to manage your Azure resources.

You may also experience an error message.

![image](../images/authorization_signin/access-control-errormsg.png)

In this article, you will learn how to set access control for your AAD organization account (**AAD user**) to your Azure subscription.

You can select or create a new AAD account in your AAD tenant to sign in to RCL apps. Refer to the following link for more information :

- [AAD User Account](./aad-account-user)

# Subscription Administrator

You can determine if your AAD organization user account is an 'Administrator' or 'Owner' on the Azure subscription by logging in to the Azure portal with the same AAD user account that you use to login to to the RCL app.

- In the Azure portal, search for 'Subscriptions' and navigate to it

![image](../images/authorization_signin/access-control-subscriptions-search.png)

- Select a subscription

![image](../images/authorization_signin/access-control-subscription-select.png)

- After you select a subscription, click on the ‘My permissions’ link for the subscription

![image](../images/authorization_signin/access-control-mypermissions.png)

# Set Owner or Contributor roles

If the AAD user account that you use to log in to the RCL app is not an administrator in the Azure subscription, you need to add the AAD account as an ‘Owner’ or ‘Contributor’ to the Azure subscription.

- Click on the the ‘Access Control (IAM)’ link in the Subscription section

- Click on the ‘Add’ link at the top to add a new role

- Add a 'Contributor’ or ‘Owner’ role assignment to your subscription for the AAD user account that you use to login to the RCL app

![image](../images/authorization_signin/access-control-create.png)

- You will see the new role assignment in the ‘Role assignments’ tab

![image](../images/authorization_signin/access-control-list.png)

**You must do this for each Azure subscription that you want to use in the RCL app.**

# Test Access Control

Once access control is properly set up for the AAD user account that you use to login to the RCL app, you can open any page in the RCL app that requires Azure subscription access to test it.

If the access control was correctly set, you will see the subscription in the drop down list.











