---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Event();
requestBody.originalStartTimeZone = "originalStartTimeZone-value";
requestBody.originalEndTimeZone = "originalEndTimeZone-value";
requestBody.responseStatus = new ResponseStatus();
requestBody.responseStatus.response = ResponseType.;
requestBody.responseStatus.time =  new Date("2016-10-19T10:37:00Z");
requestBody.recurrence = null,
requestBody.uid = "iCalUId-value";
requestBody.reminderMinutesBeforeStart = 99;
requestBody.isOnlineMeeting = true;
requestBody.onlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness;
requestBody.isReminderOn = true;
requestBody.hideAttendees = false;
requestBody.categories = [
			"Red category"
		]
const result = async () => {
	await graphServiceClient.me.eventsById("event-id").patch(requestBody);
}


```