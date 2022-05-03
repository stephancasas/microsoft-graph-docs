---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Chat();
requestBody.chatType = ChatType.Group;
requestBody.topic = "Group chat title";
const conversationmember = new ConversationMember();
conversationmember.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "roles" : [
							"owner"
						]
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')"
				 }
const conversationmember1 = new ConversationMember();
conversationmember1.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "roles" : [
							"owner"
						]
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('82fe7758-5bb3-4f0d-a43f-e555fd399c6f')"
				 }
const conversationmember2 = new ConversationMember();
conversationmember2.additionalData = {
					 "@odata.type" : "#microsoft.graph.aadUserConversationMember",
					 "roles" : [
							"guest"
						]
					 "user@odata.bind" : "https://graph.microsoft.com/beta/users('8ba98gf6-7fc2-4eb2-c7f2-aef9f21fd98g')"
				 }
requestBody.members = [
			conversationmember,
			conversationmember1,
			conversationmember2
		]
const result = async () => {
	await graphServiceClient.chats.post(requestBody);
}


```