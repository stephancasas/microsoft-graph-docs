---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CancelRequestBody();
requestBody.cancellationMessage = "Your appointment has been successfully cancelled. Please call us again.";
async () => {
	await graphServiceClient.bookingBusinessesById("bookingBusiness-id").appointmentsById("bookingAppointment-id").cancel.post(requestBody);
}


```