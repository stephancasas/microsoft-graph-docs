---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc"
	 }
const result = async () => {
	await graphServiceClient.directoryRolesById("directoryRole-id").members.$ref.post(requestBody);
}


```