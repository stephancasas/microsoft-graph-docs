---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ExternalConnection();
requestBody.id = "contosohr";
requestBody.name = "Contoso HR";
requestBody.description = "Connection to index Contoso HR system";
const result = async () => {
	await graphServiceClient.external.connections.post(requestBody);
}


```