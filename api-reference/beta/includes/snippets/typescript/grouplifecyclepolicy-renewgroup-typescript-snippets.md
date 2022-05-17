---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new RenewGroupRequestBody();
requestBody.groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";
const result = async () => {
	await graphServiceClient.groupLifecyclePolicies.renewGroup.post(requestBody);
}


```