---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/beta/identity/identityProviders/B2X_1_Test",
		 "@odata.type" : "#microsoft.graph.identityProvider"
	 }
async () => {
	await graphServiceClient.identity.b2xUserFlowsById("b2xIdentityUserFlow-id").userFlowIdentityProviders.$ref.patch(requestBody);
}


```