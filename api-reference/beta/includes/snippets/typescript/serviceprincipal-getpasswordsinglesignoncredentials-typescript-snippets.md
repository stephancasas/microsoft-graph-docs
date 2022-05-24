---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetPasswordSingleSignOnCredentialsRequestBody();
requestBody.id = "5793aa3b-cca9-4794-679a240f8b58";
const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").getPasswordSingleSignOnCredentials.post(requestBody);
}


```