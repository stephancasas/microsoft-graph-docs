---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Channel();
requestBody.displayName = "My First Shared Channel";
requestBody.description = "This is my first shared channel";
requestBody.membershipType = ChannelMembershipType.Shared;
const conversationmember = new ConversationMember();
conversationmember.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')",
					 "roles" : [
							"owner"
						]
				 }
requestBody.members = [
			conversationmember
		]
const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```