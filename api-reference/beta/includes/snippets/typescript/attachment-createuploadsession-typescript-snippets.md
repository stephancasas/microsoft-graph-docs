---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateUploadSessionRequestBody();
requestBody.attachmentItem = new AttachmentItem();
requestBody.attachmentItem.attachmentType = AttachmentType.File;
requestBody.attachmentItem.name = "flower";
requestBody.attachmentItem.size = 3483322;
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.createUploadSession.post(requestBody);
}


```