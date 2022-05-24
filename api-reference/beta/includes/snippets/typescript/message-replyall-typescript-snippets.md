---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReplyAllRequestBody();
requestBody.message = new Message();
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.fileAttachment",
						 "name" : "guidelines.txt",
						 "contentBytes" : "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
					 }
requestBody.message.attachments = [
				attachment
			]
requestBody.comment = "Please take a look at the attached guidelines before you decide on the name.";
async () => {
	await graphServiceClient.me.messagesById("message-id").replyAll.post(requestBody);
}


```