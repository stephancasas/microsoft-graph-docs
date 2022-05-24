---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityProvider();
requestBody.name = "Login with Amazon";
requestBody.type = "Amazon";
requestBody.clientId = "56433757-cadd-4135-8431-2c9e3fd68ae8";
requestBody.clientSecret = "000000000000";
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.identityProvider"
	 }
const result = async () => {
	await graphServiceClient.identityProviders.post(requestBody);
}


```