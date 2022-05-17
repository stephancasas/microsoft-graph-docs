---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignment();
requestBody.roleDefinitionId = "c2cf284d-6c41-4e6b-afac-4b80928c9034";
requestBody.principalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d";
requestBody.directoryScopeId = "/";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.unifiedRoleAssignment"
	 }
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.post(requestBody);
}


```