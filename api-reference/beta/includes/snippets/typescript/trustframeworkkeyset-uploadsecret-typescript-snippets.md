---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UploadSecretRequestBody();
requestBody.use = "use-value";
requestBody.k = "application-secret-to-be-uploaded";
requestBody.nbf = 1508969811;
requestBody.exp = 1508973711;
const result = async () => {
	await graphServiceClient.trustFramework.keySetsById("trustFrameworkKeySet-id").uploadSecret.post(requestBody);
}


```