---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SetVerifiedPublisherRequestBody();
requestBody.verifiedPublisherId = "1234567";
async () => {
	await graphServiceClient.applicationsById("application-id").setVerifiedPublisher.post(requestBody);
}


```