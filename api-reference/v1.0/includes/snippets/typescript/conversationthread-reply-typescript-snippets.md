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
async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").reply.post(requestBody);
}


```