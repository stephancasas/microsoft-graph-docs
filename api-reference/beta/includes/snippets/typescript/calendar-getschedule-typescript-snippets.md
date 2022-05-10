---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GetScheduleRequestBody();
requestBody.schedules = [
			"adelev@contoso.onmicrosoft.com",
			"meganb@contoso.onmicrosoft.com"
		]
requestBody.startTime = new DateTimeTimeZone();
requestBody.startTime.dateTime = "2019-03-15T09:00:00";
requestBody.startTime.timeZone = "Pacific Standard Time";
requestBody.endTime = new DateTimeTimeZone();
requestBody.endTime.dateTime = "2019-03-15T18:00:00";
requestBody.endTime.timeZone = "Pacific Standard Time";
requestBody.availabilityViewInterval = 60;
const headers = {
	"Prefer": "outlook.timezone=\"Pacific Standard Time\"",
};
const result = async () => {
	await graphServiceClient.me.calendar.getSchedule.post(requestBody, headers);
}


```