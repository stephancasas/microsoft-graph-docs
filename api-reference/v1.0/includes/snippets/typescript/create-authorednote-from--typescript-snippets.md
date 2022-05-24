---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthoredNote();
requestBody.content = new ItemBody();
requestBody.content.content = "String";
requestBody.content.contentType = BodyType.Text;
const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequestsById("subjectRightsRequest-id").notes.post(requestBody);
}


```