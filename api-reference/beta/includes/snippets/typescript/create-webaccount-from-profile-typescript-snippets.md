---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new WebAccount();
requestBody.description = "My Github contributions!";
requestBody.userId = "innocenty.popov";
requestBody.service = new ServiceInformation();
requestBody.service.name = "GitHub";
requestBody.service.webUrl = "https://github.com";
const result = async () => {
	await graphServiceClient.me.profile.webAccounts.post(requestBody);
}


```