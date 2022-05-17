---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Attachment();
requestBody.name = "name-value";
requestBody.contentType = "contentType-value";
requestBody.isInline = false;
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.fileAttachment",
		 "contentLocation" : "contentLocation-value",
		 "contentBytes" : "base64-contentBytes-value"
	 }
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.post(requestBody);
}


```