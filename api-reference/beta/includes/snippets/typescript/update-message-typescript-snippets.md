---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Message();
requestBody.subject = "subject-value";
requestBody.body = new ItemBody();
requestBody.body.contentType = BodyType.;
requestBody.body.content = "content-value";
requestBody.inferenceClassification = InferenceClassificationType.Other;
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").patch(requestBody);
}


```