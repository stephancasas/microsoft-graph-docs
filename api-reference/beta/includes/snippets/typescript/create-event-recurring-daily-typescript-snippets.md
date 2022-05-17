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
requestBody.start.dateTime = "2020-02-25T12:00:00";
requestBody.start.timeZone = "Pacific Standard Time";
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2020-02-25T14:00:00";
requestBody.end.timeZone = "Pacific Standard Time";
requestBody.location = new Location();
requestBody.location.displayName = "Harry's Bar";
const attendee = new Attendee();
attendee.additionalData = {
						 ["address" , "AlexW@contoso.OnMicrosoft.com"],
						 ["name" , "Alex Wilbur"],
					 "type" : "required"
				 }
requestBody.attendees = [
			attendee
		]
requestBody.recurrence = new PatternedRecurrence();
requestBody.recurrence.pattern = new RecurrencePattern();
requestBody.recurrence.pattern.type = RecurrencePatternType.Daily;
requestBody.recurrence.pattern.interval = 1;
requestBody.recurrence.range = new RecurrenceRange();
requestBody.recurrence.range.type = RecurrenceRangeType.Numbered;
requestBody.recurrence.range.startDate = "2020-02-25";
requestBody.recurrence.range.numberOfOccurrences = 2;
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.events.post(requestBody, headers);
}


```