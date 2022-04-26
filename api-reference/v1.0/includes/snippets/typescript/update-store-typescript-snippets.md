---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Store();
requestBody.defaultLanguageTag = "en-US";
const result = async () => {
	await graphServiceClient.sitesById("site-id").termStore.patch(requestBody);
}


```