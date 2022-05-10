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
requestBody.post.body.content = "I attached a reference to a file on OneDrive.";
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.referenceAttachment",
						 "name" : "Personal pictures",
						 "sourceUrl" : "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
						 "providerType" : "oneDriveConsumer",
						 "permission" : "Edit",
						 "isFolder" : "True"
					 }
requestBody.post.attachments = [
				attachment
			]
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```