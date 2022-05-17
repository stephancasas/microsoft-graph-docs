---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReplyRequestBody();
requestBody.post = new Post();
requestBody.post.body = new ItemBody();
requestBody.post.body.contentType = BodyType.Text;
requestBody.post.body.content = "Which quarter does that file cover? See my attachment.";
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.fileAttachment",
						 "name" : "Another file as attachment",
						 "contentBytes" : "VGhpcyBpcyBhIGZpbGUgdG8gYmUgYXR0YWNoZWQu"
					 }
requestBody.post.attachments = [
				attachment
			]
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```