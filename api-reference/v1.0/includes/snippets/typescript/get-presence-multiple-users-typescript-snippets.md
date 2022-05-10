---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetPresencesByUserIdRequestBody();
requestBody.ids = [
			"fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
			"66825e03-7ef5-42da-9069-724602c31f6b"
		]
const result = async () => {
	await graphServiceClient.communications.getPresencesByUserId.post(requestBody);
}


```