---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "riskEventType%20eq%20'unfamiliarFeatures'%20or%20riskLevel%20eq%20'medium'",
};
const result = async () => {
	await graphServiceClient.identityProtection.riskDetections.get(requestParameters);
}


```