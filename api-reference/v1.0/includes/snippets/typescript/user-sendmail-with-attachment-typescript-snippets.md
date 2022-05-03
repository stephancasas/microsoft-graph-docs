---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendMailRequestBody();
requestBody.message = new Message();
requestBody.message.subject = "Meet for lunch?";
requestBody.message.body = new ItemBody();
requestBody.message.body.contentType = BodyType.Text;
requestBody.message.body.content = "The new cafeteria is open.";
const recipient = new Recipient();
recipient.additionalData = {
							 ["address" , "meganb@contoso.onmicrosoft.com"],
					 }
requestBody.message.toRecipients = [
				recipient
			]
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.fileAttachment",
						 "name" : "attachment.txt",
						 "contentType" : "text/plain",
						 "contentBytes" : "SGVsbG8gV29ybGQh"
					 }
requestBody.message.attachments = [
				attachment
			]
async () => {
	await graphServiceClient.me.sendMail.post(requestBody);
}


```