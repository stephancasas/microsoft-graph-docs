---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new WorkPosition();
requestBody.isCurrent = true;
const result = async () => {
	await graphServiceClient.me.profile.positionsById("workPosition-id").patch(requestBody);
}


```