---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationMember();
requestBody.visibleHistoryStartDateTime =  new Date("0001-01-01T00:00:00Z");
requestBody.roles = [
			"owner"
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
		 "user@odata.bind" : "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
	 }
const result = async () => {
	await graphServiceClient.chatsById("chat-id").members.post(requestBody);
}


```