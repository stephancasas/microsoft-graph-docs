---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendActivityNotificationRequestBody();
requestBody.topic = new TeamworkActivityTopic();
requestBody.topic.source = TeamworkActivityTopicSource.EntityUrl;
requestBody.topic.value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7";
requestBody.activityType = "pendingFinanceApprovalRequests";
requestBody.previewText = new ItemBody();
requestBody.previewText.content = "Internal spending team has a pending finance approval requests";
requestBody.recipient = new TeamworkNotificationRecipient();
requestBody.recipient.additionalData = {
			 "@odata.type" : "microsoft.graph.channelMembersNotificationRecipient",
			 "teamId" : "e8bece96-d393-4b9b-b8da-69cedef1a7e7",
			 "channelId" : "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2"
		 }
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
					 "name" : "pendingRequestCount",
					 "value" : "5"
				 }
requestBody.templateParameters = [
			keyvaluepair
		]
async () => {
	await graphServiceClient.teamsById("team-id").sendActivityNotification.post(requestBody);
}


```