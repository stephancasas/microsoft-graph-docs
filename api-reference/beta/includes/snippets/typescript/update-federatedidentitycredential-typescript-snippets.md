---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new FederatedIdentityCredential();
requestBody.name = "testing02";
requestBody.issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0";
requestBody.subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a";
requestBody.description = "Updated description";
requestBody.audiences = [
			"api://AzureADTokenExchange"
		]
const result = async () => {
	await graphServiceClient.applicationsById("application-id").federatedIdentityCredentialsById("federatedIdentityCredential-id").patch(requestBody);
}


```