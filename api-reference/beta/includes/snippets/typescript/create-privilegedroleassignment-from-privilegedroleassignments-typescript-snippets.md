---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrivilegedRoleAssignment();
requestBody.userId = "userId-value";
requestBody.roleId = "roleId-value";
const result = async () => {
	await graphServiceClient.privilegedRoleAssignments.post(requestBody);
}


```