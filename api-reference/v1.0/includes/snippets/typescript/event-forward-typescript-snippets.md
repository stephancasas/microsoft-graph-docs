---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ForwardRequestBody();
const recipient = new Recipient();
recipient.additionalData = {
						 ["address" , "danas@contoso.onmicrosoft.com"],
						 ["name" , "Dana Swope"],
				 }
requestBody.toRecipients = [
			recipient
		]
requestBody.comment = "Dana, hope you can make this meeting.";
async () => {
	await graphServiceClient.me.eventsById("event-id").forward.post(requestBody);
}


```