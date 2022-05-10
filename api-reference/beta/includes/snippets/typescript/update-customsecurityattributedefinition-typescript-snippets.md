---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CustomSecurityAttributeDefinition();
requestBody.description = "Target completion date (YYYY/MM/DD)";
const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitionsById("customSecurityAttributeDefinition-id").patch(requestBody);
}


```