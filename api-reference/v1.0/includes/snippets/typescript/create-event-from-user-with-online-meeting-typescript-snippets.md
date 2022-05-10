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
requestBody.body.content = "Does noon work for you?";
requestBody.start = new DateTimeTimeZone();
requestBody.start.dateTime = "2017-04-15T12:00:00";
requestBody.start.timeZone = "Pacific Standard Time";
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2017-04-15T14:00:00";
requestBody.end.timeZone = "Pacific Standard Time";
requestBody.location = new Location();
requestBody.location.displayName = "Harry's Bar";
const attendee = new Attendee();
attendee.additionalData = {
						 ["address" , "samanthab@contoso.onmicrosoft.com"],
						 ["name" , "Samantha Booth"],
					 "type" : "required"
				 }
requestBody.attendees = [
			attendee
		]
requestBody.allowNewTimeProposals = true;
requestBody.isOnlineMeeting = true;
requestBody.onlineMeetingProvider = OnlineMeetingProviderType.TeamsForBusiness;
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.events.post(requestBody, headers);
}


```