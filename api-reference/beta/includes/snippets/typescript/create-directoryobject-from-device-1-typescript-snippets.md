---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/beta/directoryObjects/{id}"
	 }
const result = async () => {
	await graphServiceClient.devicesById("device-id").registeredOwners.$ref.post(requestBody);
}


```