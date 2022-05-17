---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new WebAccount();
requestBody.webUrl = "https://github.com/innocenty.popov";
const result = async () => {
	await graphServiceClient.me.profile.webAccountsById("webAccount-id").patch(requestBody);
}


```