---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "Hello World";
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").replies.post(requestBody);
}


```