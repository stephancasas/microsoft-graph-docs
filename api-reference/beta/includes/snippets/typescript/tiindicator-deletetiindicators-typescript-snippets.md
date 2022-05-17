---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DeleteTiIndicatorsRequestBody();
requestBody.value = [
			"id-value1",
			"id-value2"
		]
const result = async () => {
	await graphServiceClient.security.tiIndicators.deleteTiIndicators.post(requestBody);
}


```