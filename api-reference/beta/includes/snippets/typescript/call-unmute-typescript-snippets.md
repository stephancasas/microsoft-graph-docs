---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnmuteRequestBody();
requestBody.clientContext = "clientContext-value";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").unmute.post(requestBody);
}


```