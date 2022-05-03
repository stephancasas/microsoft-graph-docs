---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SubjectRightsRequest();
requestBody.internalDueDateTime =  new Date("2021-08-30T00:00:00Z");
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.subjectRightsRequest"
	 }
const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequestsById("subjectRightsRequest-id").patch(requestBody);
}


```