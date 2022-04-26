---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TiIndicator();
requestBody.description = "description-updated";
const result = async () => {
	await graphServiceClient.security.tiIndicatorsById("tiIndicator-id").patch(requestBody);
}


```