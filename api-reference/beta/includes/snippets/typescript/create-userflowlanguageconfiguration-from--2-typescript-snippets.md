---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Es-ESRequestBody();
requestBody.additionalData = {
		 "isEnabled" : false
	 }
async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").languagesById("userFlowLanguageConfiguration-id").put(requestBody);
}


```