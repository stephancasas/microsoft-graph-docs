---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BatchRecordDecisionsRequestBody();
requestBody.decision = "Approve";
requestBody.justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";
requestBody.resourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a";
async () => {
	await graphServiceClient.me.pendingAccessReviewInstancesById("accessReviewInstance-id").batchRecordDecisions.post(requestBody);
}


```