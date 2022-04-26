---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const headers = {
	"Prefer": "odata.maxpagesize=2",
};
let requestParameters = {
	select : "displayName",
};
const result = async () => {
	await graphServiceClient.me.contactFoldersById("contactFolder-id").contacts.delta().get(requestParameters, headers);
}


```