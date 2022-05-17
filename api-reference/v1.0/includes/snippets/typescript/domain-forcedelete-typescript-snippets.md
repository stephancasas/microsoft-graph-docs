---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ForceDeleteRequestBody();
requestBody.disableUserAccounts = true;
async () => {
	await graphServiceClient.domainsById("domain-id").forceDelete.post(requestBody);
}


```