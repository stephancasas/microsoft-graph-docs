---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetMemberGroupsRequestBody();
requestBody.securityEnabledOnly = false;
const result = async () => {
	await graphServiceClient.directoryObjectsById("directoryObject-id").getMemberGroups.post(requestBody);
}


```