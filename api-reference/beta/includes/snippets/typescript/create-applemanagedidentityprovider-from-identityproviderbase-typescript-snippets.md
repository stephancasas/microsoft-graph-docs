---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityProviderBase();
requestBody.displayName = "Sign in with Apple";
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.appleManagedIdentityProvider",
		 "developerId" : "UBF8T346G9",
		 "serviceId" : "com.microsoft.rts.b2c.test.client",
		 "keyId" : "99P6D879C4",
		 "certificateData" : "******"
	 }
const result = async () => {
	await graphServiceClient.identity.identityProviders.post(requestBody);
}


```