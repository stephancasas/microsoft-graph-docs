---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetMemberObjectsRequestBody();
requestBody.securityEnabledOnly = true;
const result = async () => {
	await graphServiceClient.me.getMemberObjects.post(requestBody);
}


```