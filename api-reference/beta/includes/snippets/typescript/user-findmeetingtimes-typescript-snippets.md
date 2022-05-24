---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new FindMeetingTimesRequestBody();
const attendeebase = new AttendeeBase();
attendeebase.additionalData = {
					 "type" : "required",
						 ["name" , "Alex Wilbur"],
						 ["address" , "alexw@contoso.onmicrosoft.com"],
				 }
requestBody.attendees = [
			attendeebase
		]
requestBody.locationConstraint = new LocationConstraint();
requestBody.locationConstraint.isRequired = "false";
requestBody.locationConstraint.suggestLocation = "false";
const locationconstraintitem = new LocationConstraintItem();
locationconstraintitem.additionalData = {
						 "resolveAvailability" : "false",
						 "displayName" : "Conf room Hood"
					 }
requestBody.locationConstraint.locations = [
				locationconstraintitem
			]
requestBody.timeConstraint = new TimeConstraint();
requestBody.timeConstraint.activityDomain = ActivityDomain.Work;
const timeslot = new TimeSlot();
timeslot.additionalData = {
							 ["dateTime" , "2019-04-16T09:00:00"],
							 ["timeZone" , "Pacific Standard Time"],
							 ["dateTime" , "2019-04-18T17:00:00"],
							 ["timeZone" , "Pacific Standard Time"],
					 }
requestBody.timeConstraint.timeSlots = [
				timeslot
			]
requestBody.isOrganizerOptional = "false";
requestBody.meetingDuration = "PT1H";
requestBody.returnSuggestionReasons = "true";
requestBody.minimumAttendeePercentage = .100;
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.findMeetingTimes.post(requestBody, headers);
}


```