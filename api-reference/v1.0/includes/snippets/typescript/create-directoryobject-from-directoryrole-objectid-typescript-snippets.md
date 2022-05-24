---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/v1.0/directoryObjects/15c1a2d5-9101-44b2-83ab-885db8a647ca"
	 }
const result = async () => {
	await graphServiceClient.directoryRolesById("directoryRole-id").members.$ref.post(requestBody);
}


```