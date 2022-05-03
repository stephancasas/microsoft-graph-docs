---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Attachment();
requestBody.name = "menu.txt";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.fileAttachment",
		 "contentBytes" : "bWFjIGFuZCBjaGVlc2UgdG9kYXk="
	 }
const result = async () => {
	await graphServiceClient.me.outlook.tasksById("outlookTask-id").attachments.post(requestBody);
}


```