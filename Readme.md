**List Groups**
https://graph.microsoft.com/v1.0/groups?$select=id,displayName,createdDateTime,description
https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName,'azb_')+or+startswith(displayName,'azd_') +or+startswith(displayName,'azu_')+or+startswith(displayName,'azp_')&$select=id,displayName,createdDateTime,description

**List Roles**
https://management.azure.com/providers/Microsoft.Authorization/roleDefinitions?api-version=2022-04-01&$filter=type+eq+'CustomRole'


**List Role to Group **
https://management.azure.com/subscriptions/${SubscriptionId}/providers/Microsoft.Authorization/roleAssignments?api-version=2022-04-01


**List AD GROUP and Its Members
 https://graph.microsoft.com/v1.0/groups?$filter=startswith(displayName,'a')&$select=id,displayName&$expand=members($select=id,displayName,employeeId)
 
 **List Managed USER Assigned Identity**
 https://management.azure.com/subscriptions/c554c36d-6465-4c03-9fe5-0e8f7983b0d3/resources?api-version=2021-04-01&$filter=resourcetype+eq+'Microsoft.ManagedIdentity/userAssignedIdentities'
