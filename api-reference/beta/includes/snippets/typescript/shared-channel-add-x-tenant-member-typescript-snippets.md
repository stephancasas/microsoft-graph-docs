---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationMember();
requestBody.roles = [
		]
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
		 "user@odata.bind" : "https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408",
		 "tenantId" : "a18103d1-a6ef-4f66-ac64-e4ef42ea8681"
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").members.post(requestBody);
}


```