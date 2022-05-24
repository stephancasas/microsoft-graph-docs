---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OpenShift();
requestBody.schedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0";
requestBody.sharedOpenShift = new OpenShiftItem();
requestBody.sharedOpenShift.notes = "Inventory Management";
requestBody.sharedOpenShift.openSlotCount = 5;
requestBody.sharedOpenShift.displayName = "Field shift";
requestBody.sharedOpenShift.startDateTime =  new Date("2018-10-04T00:58:45.340Z");
requestBody.sharedOpenShift.endDateTime =  new Date("2018-10-04T09:50:45.332Z");
requestBody.sharedOpenShift.theme = ScheduleEntityTheme.White;
const shiftactivity = new ShiftActivity();
shiftactivity.additionalData = {
						 "isPaid" : true,
						 "startDateTime" : "2018-10-04T00:58:45.340Z",
						 "endDateTime" : "2018-10-04T01:58:45.340Z",
						 "code" : "",
						 "displayName" : "Lunch"
					 }
requestBody.sharedOpenShift.activities = [
				shiftactivity
			]
requestBody.draftOpenShift = null,
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.openShiftsById("openShift-id").patch(requestBody);
}


```