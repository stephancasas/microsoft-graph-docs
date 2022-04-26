---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ExternalGroup();
requestBody.displayName = "Contoso Marketing";
requestBody.description = "The product marketing team";
const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").groupsById("externalGroup-id").patch(requestBody);
}


```