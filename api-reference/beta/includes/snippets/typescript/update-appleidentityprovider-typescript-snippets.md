---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityProviderBase();
requestBody.displayName = "Apple";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.socialIdentityProvider"
	 }
const result = async () => {
	await graphServiceClient.identity.identityProvidersById("identityProviderBase-id").patch(requestBody);
}


```