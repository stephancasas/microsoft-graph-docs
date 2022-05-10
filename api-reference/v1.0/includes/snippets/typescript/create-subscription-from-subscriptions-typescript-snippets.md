---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Subscription();
requestBody.changeType = "created";
requestBody.notificationUrl = "https://webhook.azurewebsites.net/api/send/myNotifyClient";
requestBody.resource = "me/mailFolders('Inbox')/messages";
requestBody.expirationDateTime =  new Date("2016-11-20T18:23:45.9356913Z");
requestBody.clientState = "secretClientValue";
requestBody.latestSupportedTlsVersion = "v1_2";
const result = async () => {
	await graphServiceClient.subscriptions.post(requestBody);
}


```