---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AppRoleAssignment();
requestBody.principalId = "7679d9a4-2323-44cd-b5c2-673ec88d8b12";
requestBody.resourceId = "076e8b57-bac8-49d7-9396-e3449b685055";
requestBody.appRoleId = "00000000-0000-0000-0000-000000000000";
const result = async () => {
	await graphServiceClient.groupsById("group-id").appRoleAssignments.post(requestBody);
}


```