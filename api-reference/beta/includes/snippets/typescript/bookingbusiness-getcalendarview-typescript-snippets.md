---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	start : "2018-04-30T00:00:00Z",
	end : "2018-05-10T00:00:00Z",
};
const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").calendarView.get(requestParameters);
}


```