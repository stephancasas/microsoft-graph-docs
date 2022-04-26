---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Event();
requestBody.subject = "Let's go for lunch";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.HTML;
requestBody.body.content = "Does next month work for you?";
requestBody.start = new DateTimeTimeZone();
requestBody.start.dateTime = "2019-03-10T12:00:00";
requestBody.start.timeZone = "Pacific Standard Time";
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2019-03-10T14:00:00";
requestBody.end.timeZone = "Pacific Standard Time";
requestBody.location = new Location();
requestBody.location.displayName = "Harry's Bar";
const attendee = new Attendee();
attendee.additionalData = {
						 ["address" , "adelev@contoso.onmicrosoft.com"],
						 ["name" , "Adele Vance"],
					 "type" : "required"
				 }
requestBody.attendees = [
			attendee
		]
requestBody.isOnlineMeeting = true;
requestBody.onlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness;
const result = async () => {
	await graphServiceClient.me.calendarsById("calendar-id").events.post(requestBody);
}


```