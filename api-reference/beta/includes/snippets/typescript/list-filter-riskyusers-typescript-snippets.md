---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "riskLevel%20eq%20microsoft.graph.riskLevel'medium'",
};
const result = async () => {
	await graphServiceClient.identityProtection.riskyUsers.get(requestParameters);
}


```