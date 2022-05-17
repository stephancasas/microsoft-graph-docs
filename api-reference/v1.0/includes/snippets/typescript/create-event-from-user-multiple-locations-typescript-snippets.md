---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Event();
requestBody.subject = "Plan summer company picnic";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.HTML;
requestBody.body.content = "Let's kick-start this event planning!";
requestBody.start = new DateTimeTimeZone();
requestBody.start.dateTime = "2017-08-30T11:00:00";
requestBody.start.timeZone = "Pacific Standard Time";
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2017-08-30T12:00:00";
requestBody.end.timeZone = "Pacific Standard Time";
const attendee = new Attendee();
attendee.additionalData = {
						 ["address" , "DanaS@contoso.onmicrosoft.com"],
						 ["name" , "Dana Swope"],
					 "type" : "Required"
				 }
const attendee1 = new Attendee();
attendee1.additionalData = {
						 ["address" , "AlexW@contoso.onmicrosoft.com"],
						 ["name" , "Alex Wilber"],
					 "type" : "Required"
				 }
requestBody.attendees = [
			attendee,
			attendee1
		]
requestBody.location = new Location();
requestBody.location.displayName = "Conf Room 3; Fourth Coffee; Home Office";
requestBody.location.locationType = LocationType.Default;
const location = new Location();
location.additionalData = {
					 "displayName" : "Conf Room 3"
				 }
const location1 = new Location();
location1.additionalData = {
					 "displayName" : "Fourth Coffee",
						 ["street" , "4567 Main St"],
						 ["city" , "Redmond"],
						 ["state" , "WA"],
						 ["countryOrRegion" , "US"],
						 ["postalCode" , "32008"],
						 ["latitude" , 47.672],
						 ["longitude" , -102.103],
				 }
const location2 = new Location();
location2.additionalData = {
					 "displayName" : "Home Office"
				 }
requestBody.locations = [
			location,
			location1,
			location2
		]
requestBody.allowNewTimeProposals = true;
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.events.post(requestBody, headers);
}


```