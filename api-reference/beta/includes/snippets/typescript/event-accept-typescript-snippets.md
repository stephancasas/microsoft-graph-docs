---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AcceptRequestBody();
requestBody.comment = "comment-value";
requestBody.sendResponse = true;
async () => {
	await graphServiceClient.me.eventsById("event-id").accept.post(requestBody);
}


```