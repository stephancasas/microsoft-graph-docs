---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.receivedDateTime =  new Date("datetime-value");
requestBody.sentDateTime =  new Date("datetime-value");
requestBody.hasAttachments = true;
requestBody.subject = "subject-value";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.;
requestBody.body.content = "content-value";
requestBody.bodyPreview = "bodyPreview-value";
const result = async () => {
	await graphServiceClient.me.mailFoldersById("mailFolder-id").messages.post(requestBody);
}


```