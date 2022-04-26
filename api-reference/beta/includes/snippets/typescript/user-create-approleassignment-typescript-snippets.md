---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AppRoleAssignment();
requestBody.principalId = "cde330e5-2150-4c11-9c5b-14bfdc948c79";
requestBody.resourceId = "8e881353-1735-45af-af21-ee1344582a4d";
requestBody.appRoleId = "00000000-0000-0000-0000-000000000000";
const result = async () => {
	await graphServiceClient.usersById("user-id").appRoleAssignments.post(requestBody);
}


```