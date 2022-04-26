---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Channel();
requestBody.membershipType = ChannelMembershipType.Private;
requestBody.displayName = "My First Private Channel";
requestBody.description = "This is my first private channels";
const conversationmember = new ConversationMember();
conversationmember.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "user@odata.bind" : "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')",
					 "roles" : [
							"owner"
						]
				 }
requestBody.members = [
			conversationmember
		]
requestBody.additionalData = {
		 "@odata.type" : "#Microsoft.Graph.channel"
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```