---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationMember();
requestBody.visibleHistoryStartDateTime =  new Date("2019-04-18T23:51:43.255Z");
requestBody.roles = [
			"owner"
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
		 "user@odata.bind" : "https://graph.microsoft.com/beta/users/jacob@contoso.com"
	 }
const result = async () => {
	await graphServiceClient.chatsById("chat-id").members.post(requestBody);
}


```