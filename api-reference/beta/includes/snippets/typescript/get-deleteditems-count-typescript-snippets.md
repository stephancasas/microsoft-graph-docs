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
	orderBy : "deletedDateTime%20asc",
	select : "id,displayName,deletedDateTime",
};
const result = async () => {
	await graphServiceClient.directory.deletedItems.group.get(requestParameters, headers);
}


```