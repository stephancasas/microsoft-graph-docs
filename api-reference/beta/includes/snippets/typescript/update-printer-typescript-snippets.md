---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Printer();
requestBody.name = "PrinterName";
requestBody.location = new PrinterLocation();
requestBody.location.latitude = 1.1;
requestBody.location.longitude = 2.2;
requestBody.location.altitudeInMeters = 3;
const result = async () => {
	await graphServiceClient.print.printersById("printer-id").patch(requestBody);
}


```