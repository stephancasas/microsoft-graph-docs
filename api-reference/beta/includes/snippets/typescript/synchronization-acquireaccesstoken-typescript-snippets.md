---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AcquireAccessTokenRequestBody();
const synchronizationsecretkeystringvaluepair = new SynchronizationSecretKeyStringValuePair();
synchronizationsecretkeystringvaluepair.additionalData = {
					 "@odata.type" : "microsoft.graph.synchronizationSecretKeyStringValuePair"
				 }
requestBody.credentials = [
			synchronizationsecretkeystringvaluepair
		]
async () => {
	await graphServiceClient.applicationsById("application-id").synchronization.acquireAccessToken.post(requestBody);
}


```