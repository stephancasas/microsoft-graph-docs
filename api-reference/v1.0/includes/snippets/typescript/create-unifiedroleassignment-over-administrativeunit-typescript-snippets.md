---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignment();
requestBody.roleDefinitionId = "fe930be7-5e62-47db-91af-98c3a49a38b1";
requestBody.principalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d";
requestBody.directoryScopeId = "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.unifiedRoleAssignment"
	 }
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.post(requestBody);
}


```