---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new MarkChatUnreadForUserRequestBody();
requestBody.user = new TeamworkUserIdentity();
requestBody.user.id = "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2";
requestBody.tenantId = "2a690434-97d9-4eed-83a6-f5f13600199a";
requestBody.lastMessageReadDateTime =  new Date("2021-05-27T22:13:01.577Z");
async () => {
	await graphServiceClient.chatsById("chat-id").markChatUnreadForUser.post(requestBody);
}


```