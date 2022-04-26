---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateReplyRequestBody();
requestBody.message = new Message();
const recipient = new Recipient();
recipient.additionalData = {
							 ["address" , "samanthab@contoso.onmicrosoft.com"],
							 ["name" , "Samantha Booth"],
					 }
const recipient1 = new Recipient();
recipient1.additionalData = {
							 ["address" , "randiw@contoso.onmicrosoft.com"],
							 ["name" , "Randi Welch"],
					 }
requestBody.message.toRecipients = [
				recipient,
				recipient1
			]
requestBody.comment = "Samantha, Randi, would you name the group if the project is approved, please?";
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").createReply.post(requestBody);
}


```