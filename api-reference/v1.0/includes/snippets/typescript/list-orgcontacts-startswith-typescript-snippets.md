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
	filter : "startswith(displayName,'A')",
	count : true,
	top : 1,
	orderby : "displayName",
};
const result = async () => {
	await graphServiceClient.contacts.get(requestParameters, headers);
}


```