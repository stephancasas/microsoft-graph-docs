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
requestBody.from.user.id = "id-value";
requestBody.from.user.displayName = "Joh Doe";
requestBody.from.user.additionalData = {
				 "userIdentityType" : "aadUser"
			 }
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.Html;
requestBody.body.content = "Hello World";
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.post(requestBody);
}


```