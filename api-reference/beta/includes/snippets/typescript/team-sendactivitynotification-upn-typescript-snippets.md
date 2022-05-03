---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SendActivityNotificationRequestBody();
requestBody.topic = new TeamworkActivityTopic();
requestBody.topic.source = TeamworkActivityTopicSource.EntityUrl;
requestBody.topic.value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}";
requestBody.activityType = "reservationUpdated";
requestBody.previewText = new ItemBody();
requestBody.previewText.content = "You have moved up the queue";
requestBody.recipient = new TeamworkNotificationRecipient();
requestBody.recipient.additionalData = {
			 "@odata.type" : "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
			 "userId" : "jacob@contoso.com"
		 }
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
					 "name" : "reservationId",
					 "value" : "TREEE433"
				 }
const keyvaluepair1 = new KeyValuePair();
keyvaluepair1.additionalData = {
					 "name" : "currentSlot",
					 "value" : "23"
				 }
requestBody.templateParameters = [
			keyvaluepair,
			keyvaluepair1
		]
async () => {
	await graphServiceClient.teamsById("team-id").sendActivityNotification.post(requestBody);
}


```