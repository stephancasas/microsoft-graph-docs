---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendActivityNotificationRequestBody();
requestBody.topic = new TeamworkActivityTopic();
requestBody.topic.source = TeamworkActivityTopicSource.EntityUrl;
requestBody.topic.value = "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2";
requestBody.activityType = "taskCreated";
requestBody.previewText = new ItemBody();
requestBody.previewText.content = "New Task Created";
requestBody.recipient = new TeamworkNotificationRecipient();
requestBody.recipient.additionalData = {
			 "@odata.type" : "microsoft.graph.chatMembersNotificationRecipient",
			 "chatId" : "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2"
		 }
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
					 "name" : "taskId",
					 "value" : "Task 12322"
				 }
requestBody.templateParameters = [
			keyvaluepair
		]
async () => {
	await graphServiceClient.chatsById("chat-id").sendActivityNotification.post(requestBody);
}


```