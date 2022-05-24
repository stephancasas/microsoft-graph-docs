---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessReviewPolicy();
requestBody.isGroupOwnerManagementEnabled = true;
const result = async () => {
	await graphServiceClient.policies.accessReviewPolicy.patch(requestBody);
}


```