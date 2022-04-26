---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConfirmCompromisedRequestBody();
requestBody.servicePrincipalIds = [
			"9089a539-a539-9089-39a5-899039a58990"
		]
async () => {
	await graphServiceClient.identityProtection.riskyServicePrincipals.confirmCompromised.post(requestBody);
}


```