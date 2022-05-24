---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "Hello World <at id="0">Jane Smith</at>";
const chatmessagemention = new ChatMessageMention();
chatmessagemention.additionalData = {
					 "id" : 0,
					 "mentionText" : "Jane Smith",
							 ["displayName" , "Jane Smith"],
							 ["id" , "ef1c916a-3135-4417-ba27-8eb7bd084193"],
							 ["userIdentityType" , "aadUser"],
				 }
requestBody.mentions = [
			chatmessagemention
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```