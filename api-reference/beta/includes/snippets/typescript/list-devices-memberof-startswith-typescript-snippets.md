---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const headers = {
	"ConsistencyLevel": "eventual",
};
let requestParameters = {
	count : true,
	orderBy : "displayName",
	filter : "startswith(displayName,%20'A')",
};
const result = async () => {
	await graphServiceClient.devicesById("device-id").memberOf.group.get(requestParameters, headers);
}


```