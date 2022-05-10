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
	filter : "extensionAttributes/extensionAttribute1%20eq%20'BYOD-Device'",
	count : true,
};
const result = async () => {
	await graphServiceClient.devices.get(requestParameters, headers);
}


```