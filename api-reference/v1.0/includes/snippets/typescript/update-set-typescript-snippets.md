---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Set();
requestBody.description = "mySet";
const result = async () => {
	await graphServiceClient.sitesById("site-id").termStore.setsById("set-id").patch(requestBody);
}


```