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
	expand : "manager($levels=max;$select=id,displayName)",
	select : "id,displayName",
	count : true,
};
const result = async () => {
	await graphServiceClient.me.get(requestParameters, headers);
}


```