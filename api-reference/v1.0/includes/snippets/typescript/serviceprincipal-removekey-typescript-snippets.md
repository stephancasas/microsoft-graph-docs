---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new RemoveKeyRequestBody();
requestBody.keyId = "f0b0b335-1d71-4883-8f98-567911bfdca6";
requestBody.proof = "eyJ0eXAiOiJ...";
async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").removeKey.post(requestBody);
}


```