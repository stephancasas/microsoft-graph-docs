---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityProviderBase();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.socialIdentityProvider",
		 "responseType" : "id_token"
	 }
const result = async () => {
	await graphServiceClient.identity.identityProvidersById("identityProviderBase-id").patch(requestBody);
}


```