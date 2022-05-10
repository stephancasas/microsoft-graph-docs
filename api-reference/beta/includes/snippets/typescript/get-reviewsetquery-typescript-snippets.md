---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").reviewSetsById("reviewSet-id").queriesById("reviewSetQuery-id").get();
}


```