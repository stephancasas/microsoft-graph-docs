---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.createdDateTime =  new Date("2019-02-04T19:58:15.511Z");
requestBody.from = new ChatMessageFromIdentitySet();
requestBody.from.user = new Identity();
requestBody.from.user.id = "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca";
requestBody.from.user.displayName = "John Doe";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "Hello World";
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").replies.post(requestBody);
}


```