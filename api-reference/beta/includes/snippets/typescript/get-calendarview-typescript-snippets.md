---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	startDateTime : "2017-01-01T19:00:00-08:00",
	endDateTime : "2017-01-07T19:00:00-08:00",
};
const result = async () => {
	await graphServiceClient.me.calendar.calendarView.get(requestParameters);
}


```