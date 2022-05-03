---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	startDateTime : "2020-01-01T19:00:00-08:00",
	endDateTime : "2020-01-02T19:00:00-08:00",
};
const result = async () => {
	await graphServiceClient.me.calendarView.get(requestParameters);
}


```