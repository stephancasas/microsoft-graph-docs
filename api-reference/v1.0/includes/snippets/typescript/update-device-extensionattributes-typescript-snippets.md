---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Device();
requestBody.additionalData = {
			 ["extensionAttribute1" , "BYOD-Device"],
	 }
const result = async () => {
	await graphServiceClient.devicesById("device-id").patch(requestBody);
}


```