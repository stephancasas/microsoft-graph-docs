---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationThread();
requestBody.topic = "Take your wellness days and rest";
const post = new Post();
post.additionalData = {
						 ["contentType" , "html"],
						 ["content" , "Waiting for the summer holidays."],
				 }
requestBody.posts = [
			post
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").conversationsById("conversation-id").threads.post(requestBody);
}


```