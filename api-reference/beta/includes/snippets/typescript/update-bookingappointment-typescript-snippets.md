---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BookingAppointment();
requestBody.end = new DateTimeTimeZone();
requestBody.end.dateTime = "2018-05-06T12:30:00.0000000+00:00";
requestBody.end.timeZone = "UTC";
requestBody.end.additionalData = {
			 "@odata.type" : "#microsoft.graph.dateTimeTimeZone"
		 }
requestBody.invoiceDate = new DateTimeTimeZone();
requestBody.invoiceDate.dateTime = "2018-05-06T12:30:00.0000000+00:00";
requestBody.invoiceDate.timeZone = "UTC";
requestBody.invoiceDate.additionalData = {
			 "@odata.type" : "#microsoft.graph.dateTimeTimeZone"
		 }
requestBody.start = new DateTimeTimeZone();
requestBody.start.dateTime = "2018-05-06T12:00:00.0000000+00:00";
requestBody.start.timeZone = "UTC";
requestBody.start.additionalData = {
			 "@odata.type" : "#microsoft.graph.dateTimeTimeZone"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.bookingAppointment"
	 }
const result = async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").appointmentsById("bookingAppointment-id").patch(requestBody);
}


```