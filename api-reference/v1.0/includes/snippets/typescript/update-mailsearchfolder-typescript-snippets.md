---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new MailFolder();
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.mailSearchFolder",
		 "filterQuery" : "contains(subject, 'Analytics')"
	 }
const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").patch(requestBody);
}


```