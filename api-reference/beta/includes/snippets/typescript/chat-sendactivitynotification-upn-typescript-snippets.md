---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendActivityNotificationRequestBody();
requestBody.topic = new TeamworkActivityTopic();
requestBody.topic.source = TeamworkActivityTopicSource.EntityUrl;
requestBody.topic.value = "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}";
requestBody.activityType = "approvalRequired";
requestBody.previewText = new ItemBody();
requestBody.previewText.content = "Deployment requires your approval";
requestBody.recipient = new TeamworkNotificationRecipient();
requestBody.recipient.additionalData = {
			 "@odata.type" : "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
			 "userId" : "jacob@contoso.com"
		 }
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
					 "name" : "approvalTaskId",
					 "value" : "2020AAGGTAPP"
				 }
requestBody.templateParameters = [
			keyvaluepair
		]
async () => {
	await graphServiceClient.chatsById("chat-id").sendActivityNotification.post(requestBody);
}


```