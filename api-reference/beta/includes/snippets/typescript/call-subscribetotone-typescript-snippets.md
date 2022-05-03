---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SubscribeToToneRequestBody();
requestBody.clientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").subscribeToTone.post(requestBody);
}


```