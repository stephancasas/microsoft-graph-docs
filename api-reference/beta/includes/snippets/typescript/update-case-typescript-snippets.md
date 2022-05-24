---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Case();
requestBody.displayName = "My Case 1 - Renamed";
requestBody.description = "Updated description";
requestBody.externalId = "Updated externalId";
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").patch(requestBody);
}


```