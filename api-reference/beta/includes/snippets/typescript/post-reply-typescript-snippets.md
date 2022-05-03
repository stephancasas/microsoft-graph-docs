---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReplyRequestBody();
requestBody.post = new Post();
requestBody.post.body = new ItemBody();
requestBody.post.body.contentType = BodyType.;
requestBody.post.body.content = "content-value";
requestBody.post.receivedDateTime =  new Date("2016-10-19T10:37:00Z");
requestBody.post.hasAttachments = true;
requestBody.post.from = new Recipient();
requestBody.post.from.emailAddress = new EmailAddress();
requestBody.post.from.emailAddress.name = "name-value";
requestBody.post.from.emailAddress.address = "address-value";
requestBody.post.sender = new Recipient();
requestBody.post.sender.emailAddress = new EmailAddress();
requestBody.post.sender.emailAddress.name = "name-value";
requestBody.post.sender.emailAddress.address = "address-value";
requestBody.post.conversationThreadId = "conversationThreadId-value";
const recipient = new Recipient();
recipient.additionalData = {
							 ["name" , "name-value"],
							 ["address" , "address-value"],
					 }
requestBody.post.newParticipants = [
				recipient
			]
requestBody.post.conversationId = "conversationId-value";
requestBody.post.createdDateTime =  new Date("2016-10-19T10:37:00Z");
requestBody.post.lastModifiedDateTime =  new Date("2016-10-19T10:37:00Z");
requestBody.post.changeKey = "changeKey-value";
requestBody.post.categories = [
				"categories-value"
			]
requestBody.post.id = "id-value";
requestBody.post.inReplyTo = new Post();
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.fileAttachment",
						 "lastModifiedDateTime" : "2016-10-19T10:37:00Z",
						 "name" : "name-value",
						 "contentType" : "contentType-value",
						 "size" : 99,
						 "isInline" : true,
						 "id" : "id-value"
					 }
requestBody.post.attachments = [
				attachment
			]
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").postsById("post-id").reply.post(requestBody);
}


```