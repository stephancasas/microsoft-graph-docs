---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Extension();
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.openTypeExtension",
		 "extensionName" : "Com.Contoso.Deal",
		 "companyName" : "Alpine Skis",
		 "dealValue" : 1010100,
		 "expirationDate" : "2015-07-03T13:04:00.000Z"
	 }
const result = async () => {
	await graphServiceClient.groupsById("group-id").eventsById("event-id").extensions.post(requestBody);
}


```