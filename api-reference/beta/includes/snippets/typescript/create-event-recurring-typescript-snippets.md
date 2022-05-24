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
requestBody.body.content = "Does noon time work for you?";
requestBody.start = new DateTimeTimeZone();
requestBody.start.dateTime = "2017-09-04T12:00:00";
requestBody.start.timeZone = "Pacific Standard Time";
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2017-09-04T14:00:00";
requestBody.end.timeZone = "Pacific Standard Time";
requestBody.recurrence = new PatternedRecurrence();
requestBody.recurrence.pattern = new RecurrencePattern();
requestBody.recurrence.pattern.type = RecurrencePatternType.Weekly;
requestBody.recurrence.pattern.interval = 1;
requestBody.recurrence.pattern.daysOfWeek = [
					"Monday"
				]
requestBody.recurrence.range = new RecurrenceRange();
requestBody.recurrence.range.type = RecurrenceRangeType.EndDate;
requestBody.recurrence.range.startDate = "2017-09-04";
requestBody.recurrence.range.endDate = "2017-12-31";
requestBody.location = new Location();
requestBody.location.displayName = "Harry's Bar";
const attendee = new Attendee();
attendee.additionalData = {
						 ["address" , "AdeleV@contoso.onmicrosoft.com"],
						 ["name" , "Adele Vance"],
					 "type" : "required"
				 }
requestBody.attendees = [
			attendee
		]
const result = async () => {
	await graphServiceClient.me.events.post(requestBody);
}


```