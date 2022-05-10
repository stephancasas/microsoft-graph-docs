---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CreateRequestBody();
requestBody.displayName = "Test Printer";
requestBody.manufacturer = "Test Printer Manufacturer";
requestBody.model = "Test Printer Model";
requestBody.physicalDeviceId = null,
requestBody.hasPhysicalDevice = false;
requestBody.certificateSigningRequest = new PrintCertificateSigningRequest();
requestBody.certificateSigningRequest.content = "{content}";
requestBody.certificateSigningRequest.transportKey = "{sampleTransportKey}";
requestBody.connectorId = null,
async () => {
	await graphServiceClient.print.printers.create.post(requestBody);
}


```