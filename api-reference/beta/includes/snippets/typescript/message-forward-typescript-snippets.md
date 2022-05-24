---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ForwardRequestBody();
requestBody.message = new Message();
requestBody.message.isDeliveryReceiptRequested = true;
const recipient = new Recipient();
recipient.additionalData = {
							 ["address" , "danas@contoso.onmicrosoft.com"],
							 ["name" , "Dana Swope"],
					 }
requestBody.message.toRecipients = [
				recipient
			]
requestBody.comment = "Dana, just want to make sure you get this.";
async () => {
	await graphServiceClient.me.messagesById("message-id").forward.post(requestBody);
}


```