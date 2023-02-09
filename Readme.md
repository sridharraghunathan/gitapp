**List Groups**
https://graph.microsoft.com/v1.0/groups?$select=id,displayName,createdDateTime,description
**List Roles**
https://management.azure.com/providers/Microsoft.Authorization/roleDefinitions?api-version=2022-04-01&$filter=type+eq+'CustomRole'
**List Role to Group **
https://management.azure.com/subscriptions/${SubscriptionId}/providers/Microsoft.Authorization/roleAssignments?api-version=2022-04-01
**List AD GROUP and Its Members
https://graph.microsoft.com/v1.0/groups?$select=id,displayName&$expand=members($select=id,displayName,employeeId)
