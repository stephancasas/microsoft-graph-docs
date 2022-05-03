---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Shift();
requestBody.id = "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8";
requestBody.userId = "c5d0c76b-80c4-481c-be50-923cd8d680a1";
requestBody.schedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0";
requestBody.sharedShift = new ShiftItem();
requestBody.sharedShift.displayName = "Day shift";
requestBody.sharedShift.notes = "Please do inventory as part of your shift.";
requestBody.sharedShift.startDateTime =  new Date("2019-03-11T15:00:00Z");
requestBody.sharedShift.endDateTime =  new Date("2019-03-12T00:00:00Z");
requestBody.sharedShift.theme = ScheduleEntityTheme.Blue;
const shiftactivity = new ShiftActivity();
shiftactivity.additionalData = {
						 "isPaid" : true,
						 "startDateTime" : "2019-03-11T15:00:00Z",
						 "endDateTime" : "2019-03-11T15:15:00Z",
						 "code" : "",
						 "displayName" : "Lunch"
					 }
requestBody.sharedShift.activities = [
				shiftactivity
			]
requestBody.draftShift = new ShiftItem();
requestBody.draftShift.displayName = "Day shift";
requestBody.draftShift.notes = "Please do inventory as part of your shift.";
requestBody.draftShift.startDateTime =  new Date("2019-03-11T15:00:00Z");
requestBody.draftShift.endDateTime =  new Date("2019-03-12T00:00:00Z");
requestBody.draftShift.theme = ScheduleEntityTheme.Blue;
const shiftactivity = new ShiftActivity();
shiftactivity.additionalData = {
						 "isPaid" : true,
						 "startDateTime" : "2019-03-11T15:00:00Z",
						 "endDateTime" : "2019-03-11T15:30:00Z",
						 "code" : "",
						 "displayName" : "Lunch"
					 }
requestBody.draftShift.activities = [
				shiftactivity
			]
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.shifts.post(requestBody);
}


```