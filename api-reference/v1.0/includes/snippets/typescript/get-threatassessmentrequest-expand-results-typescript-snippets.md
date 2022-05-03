---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	expand : "results",
};
const result = async () => {
	await graphServiceClient.informationProtection.threatAssessmentRequestsById("threatAssessmentRequest-id").get(requestParameters);
}


```