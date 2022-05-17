---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Team();
requestBody.displayName = "My Sample Team";
requestBody.description = "My Sample Team’s Description";
const conversationmember = new ConversationMember();
conversationmember.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "roles" : [
							"owner"
						]
					 "user@odata.bind" : "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
				 }
requestBody.members = [
			conversationmember
		]
requestBody.additionalData = {
		 "template@odata.bind" : "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
	 }
const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```