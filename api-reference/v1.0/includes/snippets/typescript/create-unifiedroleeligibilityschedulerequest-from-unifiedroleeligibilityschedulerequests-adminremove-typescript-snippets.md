---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleEligibilityScheduleRequest();
requestBody.action = "adminRemove";
requestBody.roleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4";
requestBody.directoryScopeId = "/";
requestBody.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```