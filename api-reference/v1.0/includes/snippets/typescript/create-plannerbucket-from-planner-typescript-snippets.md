---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerBucket();
requestBody.name = "Advertising";
requestBody.planId = "xqQg5FS2LkCp935s-FIFm2QAFkHM";
requestBody.orderHint = " !";
const result = async () => {
	await graphServiceClient.planner.buckets.post(requestBody);
}


```