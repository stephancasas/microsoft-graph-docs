---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "<div><div><at id="0">GraphTesting</at>&nbsp;Hello team</div></div>";
const chatmessagemention = new ChatMessageMention();
chatmessagemention.additionalData = {
					 "id" : 0,
					 "mentionText" : "GraphTesting",
							 ["id" , "68a3e365-f7d9-4a56-b499-24332a9cc572"],
							 ["displayName" , "GraphTesting"],
							 ["conversationIdentityType" , "team"],
				 }
requestBody.mentions = [
			chatmessagemention
		]
requestBody.reactions = [
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```