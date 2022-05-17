---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateReplyAllRequestBody();
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
requestBody.comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").createReplyAll.post(requestBody);
}


```