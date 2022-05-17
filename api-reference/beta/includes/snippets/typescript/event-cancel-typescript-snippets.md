---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CancelRequestBody();
requestBody.comment = "Cancelling for this week due to all hands";
async () => {
	await graphServiceClient.me.eventsById("event-id").cancel.post(requestBody);
}


```