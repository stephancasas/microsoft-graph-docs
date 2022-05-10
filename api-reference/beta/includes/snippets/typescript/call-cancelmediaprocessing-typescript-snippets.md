---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CancelMediaProcessingRequestBody();
requestBody.clientContext = "clientContext-value";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").cancelMediaProcessing.post(requestBody);
}


```