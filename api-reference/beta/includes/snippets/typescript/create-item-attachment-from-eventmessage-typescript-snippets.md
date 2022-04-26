---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Attachment();
requestBody.name = "name-value";
requestBody.additionalData = {
		 "@odata.type" : "#Microsoft.OutlookServices.ItemAttachment",
			 ["@odata.type" , "microsoft.graph.message"],
	 }
const result = async () => {
	await graphServiceClient.me.eventsById("event-id").attachments.post(requestBody);
}


```