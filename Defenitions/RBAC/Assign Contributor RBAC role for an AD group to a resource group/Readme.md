# Assign Contributor RBAC role for AD Group

This policy defenition will add Contributor access for a specified AD Group to a resource Group based on Tags.

Import the json text to a new defenition and assign it to a Management Group or Subscription.

## Parameters

Fill in the information needed

![Parameters](https://github.com/jantorep/CustomAzurePolicys/blob/main/Defenitions/RBAC/Assign%20Contributor%20RBAC%20role%20for%20an%20AD%20group%20to%20a%20resource%20group/parameters.jpg)

The Parameter Values should be self explanatory but

Tag Name is what it is, the first part of the tag.
Tag Value is the last part of the tag.

Azure AD Group Object ID is the object id of the AAD Group that you want to give contributor rights to.

## Customizing the template

If you want to change the template there are parts you can change.

Roledefenition for the managed identity can be changed on line 51 by changing the GUID, right now it's owner. Or you can also edit the policy in the GUI and change it when editing the policy defenition.

![Parameters](https://github.com/jantorep/CustomAzurePolicys/blob/main/Defenitions/RBAC/Assign%20Contributor%20RBAC%20role%20for%20an%20AD%20group%20to%20a%20resource%20group/parameters1.jpg)

Changing the role the AAD Group get's can be done on line 57 and 81 by changing the GUID at the end.
