---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.subject = "Party planning";
const recipient = new Recipient();
recipient.additionalData = {
						 ["name" , "Samantha Booth"],
						 ["address" , "samanthab@contoso.onmicrosoft.com"],
				 }
requestBody.toRecipients = [
			recipient
		]
const mention = new Mention();
mention.additionalData = {
						 ["name" , "Dana Swope"],
						 ["address" , "danas@contoso.onmicrosoft.com"],
				 }
requestBody.mentions = [
			mention
		]
const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```