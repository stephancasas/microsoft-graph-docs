---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DismissRequestBody();
requestBody.userIds = [
			"04487ee0-f4f6-4e7f-8999-facc5a30e232",
			"13387ee0-f4f6-4e7f-8999-facc5120e345"
		]
async () => {
	await graphServiceClient.identityProtection.riskyUsers.dismiss.post(requestBody);
}


```