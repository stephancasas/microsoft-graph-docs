---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignment();
requestBody.principalId = "679a9213-c497-48a4-830a-8d3d25d94ddc";
requestBody.roleDefinitionId = "ae79f266-94d4-4dab-b730-feca7e132178";
requestBody.appScopeId = "/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997";
const result = async () => {
	await graphServiceClient.roleManagement.entitlementManagement.roleAssignments.post(requestBody);
}


```