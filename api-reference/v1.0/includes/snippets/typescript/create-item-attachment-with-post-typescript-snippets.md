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
requestBody.post.body.content = "I attached an event.";
const attachment = new Attachment();
attachment.additionalData = {
						 "@odata.type" : "#microsoft.graph.itemAttachment",
						 "name" : "Holiday event",
							 ["@odata.type" , "microsoft.graph.event"],
							 ["subject" , "Discuss gifts for children"],
								 ["contentType" , "HTML"],
								 ["content" , "Let's look for funding!"],
								 ["dateTime" , "2019-12-02T18:00:00"],
								 ["timeZone" , "Pacific Standard Time"],
								 ["dateTime" , "2019-12-02T19:00:00"],
								 ["timeZone" , "Pacific Standard Time"],
					 }
requestBody.post.attachments = [
				attachment
			]
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```