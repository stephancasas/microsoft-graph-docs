---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrintConnector();
requestBody.displayName = "ConnectorName";
requestBody.fullyQualifiedDomainName = "CONNECTOR-MACHINE";
requestBody.operatingSystem = "Microsoft Windows 10 Enterprise Insider Preview | 10.0.19555";
requestBody.appVersion = "0.19.7338.23496";
requestBody.location = new PrinterLocation();
requestBody.location.latitude = 1.1;
requestBody.location.longitude = 2.2;
requestBody.location.altitudeInMeters = 3;
const result = async () => {
	await graphServiceClient.print.connectorsById("printConnector-id").patch(requestBody);
}


```