---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendMailRequestBody();
requestBody.message = new Message();
requestBody.message.subject = "Project kickoff";
const recipient = new Recipient();
recipient.additionalData = {
							 ["name" , "Samantha Booth"],
							 ["address" , "samanthab@contoso.onmicrosoft.com"],
					 }
requestBody.message.toRecipients = [
				recipient
			]
const mention = new Mention();
mention.additionalData = {
							 ["name" , "Dana Swope"],
							 ["address" , "danas@contoso.onmicrosoft.com"],
					 }
requestBody.message.mentions = [
				mention
			]
async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```