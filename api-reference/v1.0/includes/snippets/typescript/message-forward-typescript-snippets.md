---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ForwardRequestBody();
requestBody.comment = "comment-value";
const recipient = new Recipient();
recipient.additionalData = {
						 ["name" , "name-value"],
						 ["address" , "address-value"],
				 }
requestBody.toRecipients = [
			recipient
		]
async () => {
	await graphServiceClient.me.messagesById("message-id").forward.post(requestBody);
}


```