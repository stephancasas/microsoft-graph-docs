---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TiIndicator();
requestBody.additionalInformation = "additionalInformation-after-update";
requestBody.confidence = 42;
requestBody.description = "description-after-update";
const headers = {
	"Prefer": "return=representation",
};
const result = async () => {
	await graphServiceClient.security.tiIndicatorsById("tiIndicator-id").patch(requestBody, headers);
}


```