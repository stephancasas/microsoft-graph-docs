---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ServicePrincipal();
requestBody.appId = "65415bb1-9267-4313-bbf5-ae259732ee12";
const result = async () => {
	await graphServiceClient.servicePrincipals.post(requestBody);
}


```