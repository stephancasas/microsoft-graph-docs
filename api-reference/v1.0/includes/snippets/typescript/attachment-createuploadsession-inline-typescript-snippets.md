---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateUploadSessionRequestBody();
requestBody.attachmentItem = new AttachmentItem();
requestBody.attachmentItem.attachmentType = AttachmentType.File;
requestBody.attachmentItem.name = "scenary";
requestBody.attachmentItem.size = 7208534;
requestBody.attachmentItem.isInline = true;
requestBody.attachmentItem.contentId = "my_inline_picture";
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").attachments.createUploadSession.post(requestBody);
}


```