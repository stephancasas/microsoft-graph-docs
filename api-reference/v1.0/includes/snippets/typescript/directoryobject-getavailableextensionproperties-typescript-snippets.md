---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetAvailableExtensionPropertiesRequestBody();
requestBody.isSyncedFromOnPremises = true;
const result = async () => {
	await graphServiceClient.directoryObjects.getAvailableExtensionProperties.post(requestBody);
}


```