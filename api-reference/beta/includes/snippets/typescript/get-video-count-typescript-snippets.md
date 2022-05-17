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
	search : "%22displayName:Video%22%20OR%20%22description:prod%22",
	orderby : "displayName",
	count : true,
};
const result = async () => {
	await graphServiceClient.groups.get(requestParameters, headers);
}


```