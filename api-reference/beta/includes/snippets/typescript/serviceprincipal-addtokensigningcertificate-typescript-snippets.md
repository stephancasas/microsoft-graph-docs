---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AddTokenSigningCertificateRequestBody();
requestBody.displayName = "CN=customDisplayName";
requestBody.endDateTime =  new Date("2024-01-25T00:00:00Z");
const result = async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").addTokenSigningCertificate.post(requestBody);
}


```