---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "createdDateTime%20ge%202019-09-01T00:00:00Z",
};
const result = async () => {
	await graphServiceClient.identity.conditionalAccess.namedLocations.get(requestParameters);
}


```