---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Subscription();
requestBody.expirationDateTime =  new Date("2016-11-22T18:23:45.9356913Z");
const result = async () => {
	await graphServiceClient.subscriptionsById("subscription-id").patch(requestBody);
}


```