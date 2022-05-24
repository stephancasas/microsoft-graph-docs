---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/beta/identityProviders/{id}"
	 }
const result = async () => {
	await graphServiceClient.identity.b2cUserFlowsById("b2cIdentityUserFlow-id").identityProviders.$ref.post(requestBody);
}


```