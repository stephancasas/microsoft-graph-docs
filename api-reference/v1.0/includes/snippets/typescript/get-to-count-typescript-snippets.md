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
	search : "%22displayName:wa%22%20OR%20%22displayName:ad%22",
q.	orderbydisplayName = undefined;
	count : true,
};
const result = async () => {
	await graphServiceClient.users.get(requestParameters, headers);
}


```