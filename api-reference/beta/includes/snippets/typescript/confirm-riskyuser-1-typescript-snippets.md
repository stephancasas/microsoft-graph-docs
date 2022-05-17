---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConfirmCompromisedRequestBody();
requestBody.userIds = [
			"29f270bb-4d23-4f68-8a57-dc73dc0d4caf",
			"20f91ec9-d140-4d90-9cd9-f618587a1471"
		]
async () => {
	await graphServiceClient.riskyUsers.confirmCompromised.post(requestBody);
}


```