---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "distributionMethod%20eq%20'organization'",
};
const result = async () => {
	await graphServiceClient.appCatalogs.teamsApps.get(requestParameters);
}


```