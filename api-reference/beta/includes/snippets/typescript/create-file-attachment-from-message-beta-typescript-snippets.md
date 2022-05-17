---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Attachment();
requestBody.name = "smile";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.fileAttachment",
		 "contentBytes" : "a0b1c76de9f7="
	 }
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.post(requestBody);
}


```