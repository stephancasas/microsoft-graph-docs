---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DeleteTiIndicatorsByExternalIdRequestBody();
requestBody.value = [
			"externalId-value1",
			"externalId-value2"
		]
const result = async () => {
	await graphServiceClient.security.tiIndicators.deleteTiIndicatorsByExternalId.post(requestBody);
}


```