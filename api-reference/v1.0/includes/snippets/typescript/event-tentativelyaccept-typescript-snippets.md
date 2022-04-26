---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TentativelyAcceptRequestBody();
requestBody.comment = "I may not be able to make this week. How about next week?";
requestBody.sendResponse = true;
requestBody.proposedNewTime = new TimeSlot();
requestBody.proposedNewTime.start = new DateTimeTimeZone();
requestBody.proposedNewTime.start.dateTime = "2019-12-02T18:00:00";
requestBody.proposedNewTime.start.timeZone = "Pacific Standard Time";
requestBody.proposedNewTime.end = new DateTimeTimeZone();
requestBody.proposedNewTime.end.dateTime = "2019-12-02T19:00:00";
requestBody.proposedNewTime.end.timeZone = "Pacific Standard Time";
async () => {
	await graphServiceClient.me.eventsById("event-id").tentativelyAccept.post(requestBody);
}


```