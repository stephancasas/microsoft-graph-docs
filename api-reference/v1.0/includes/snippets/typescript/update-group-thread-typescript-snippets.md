---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ConversationThread();
requestBody.additionalData = {
		 "originalStartTimeZone" : "originalStartTimeZone-value",
		 "originalEndTimeZone" : "originalEndTimeZone-value",
			 ["response" , ""],
			 ["time" , "datetime-value"],
		 "iCalUId" : "iCalUId-value",
		 "reminderMinutesBeforeStart" : 99,
		 "isReminderOn" : true
	 }
const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").patch(requestBody);
}


```