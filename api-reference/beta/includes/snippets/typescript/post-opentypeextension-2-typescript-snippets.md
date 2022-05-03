---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Extension();
requestBody.additionalData = {
		 "@odata.type" : "microsoft.graph.openTypeExtension",
		 "extensionName" : "Com.Contoso.Referral",
		 "companyName" : "Wingtip Toys",
		 "dealValue" : 500050,
		 "expirationDate" : "2015-12-03T10:00:00.000Z"
	 }
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").extensions.post(requestBody);
}


```