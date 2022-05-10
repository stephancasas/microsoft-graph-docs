---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignment();
requestBody.principalId = "6b937a9d-c731-465b-a844-2d5b5368c161";
requestBody.roleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3";
requestBody.directoryScopeId = "/661e1310-bd76-4795-89a7-8f3c8f855bfc";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.unifiedRoleAssignment"
	 }
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignments.post(requestBody);
}


```