---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PinnedChatMessageInfo();
requestBody.additionalData = {
		 "message@odata.bind" : "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832"
	 }
const result = async () => {
	await graphServiceClient.chatsById("chat-id").pinnedMessages.post(requestBody);
}


```