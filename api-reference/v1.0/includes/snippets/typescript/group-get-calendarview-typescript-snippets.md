---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const headers = {
	"Prefer": "outlook.body-content-type=\"text\"",
};
let requestParameters = {
	startDateTime : "2017-01-01T19:00:00-08:00",
	endDateTime : "2017-10-01T19:00:00.00-08:00",
};
const result = async () => {
	await graphServiceClient.groupsById("group-id").calendarView.get(requestParameters, headers);
}


```