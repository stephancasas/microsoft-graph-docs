---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DeletePasswordSingleSignOnCredentialsRequestBody();
requestBody.id = "5793aa3b-cca9-4794-679a240f8b58";
async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").deletePasswordSingleSignOnCredentials.post(requestBody);
}


```