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
	filter : "hasMembersWithLicenseErrors%20eq%20true",
	select : "id,displayName",
};
const result = async () => {
	await graphServiceClient.groups.get(requestParameters, headers);
}


```