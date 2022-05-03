---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const headers = {
	"Prefer": "odata.maxpagesize=2",
};
const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messages.delta().get(headers);
}


```