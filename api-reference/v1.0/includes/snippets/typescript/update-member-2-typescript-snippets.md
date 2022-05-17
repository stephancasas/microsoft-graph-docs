---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationMember();
requestBody.roles = [
			"owner"
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.aadUserConversationMember"
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").membersById("conversationMember-id").patch(requestBody);
}


```