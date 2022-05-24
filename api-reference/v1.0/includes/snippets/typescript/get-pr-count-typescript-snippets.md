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
	orderby : "displayName",
	search : "%22displayName:Pr%22",
	select : "displayName,id",
};
const result = async () => {
	await graphServiceClient.groupsById("group-id").members.user.get(requestParameters, headers);
}


```