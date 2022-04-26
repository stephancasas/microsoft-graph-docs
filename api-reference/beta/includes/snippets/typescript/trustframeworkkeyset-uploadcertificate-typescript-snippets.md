---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UploadCertificateRequestBody();
requestBody.key = "key-value";
const result = async () => {
	await graphServiceClient.trustFramework.keySetsById("trustFrameworkKeySet-id").uploadCertificate.post(requestBody);
}


```