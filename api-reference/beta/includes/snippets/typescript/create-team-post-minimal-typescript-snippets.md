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
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('0040b377-61d8-43db-94f5-81374122dc7e')"
				 }
requestBody.members = [
			conversationmember
		]
requestBody.additionalData = {
		 "template@odata.bind" : "https://graph.microsoft.com/beta/teamsTemplates('standard')"
	 }
const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```