---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.subject = "Did you see last night's game?";
requestBody.importance = Importance.Low;
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.HTML;
requestBody.body.content = "They were <b>awesome</b>!";
const recipient = new Recipient();
recipient.additionalData = {
						 ["address" , "AdeleV@contoso.onmicrosoft.com"],
				 }
requestBody.toRecipients = [
			recipient
		]
const result = async () => {
	await graphServiceClient.me.messages.post(requestBody);
}


```