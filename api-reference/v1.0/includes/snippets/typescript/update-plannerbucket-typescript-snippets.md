---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerBucket();
requestBody.name = "Development";
const headers = {
	"Prefer": "return=representation",
	"If-Match": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
};
const result = async () => {
	await graphServiceClient.planner.bucketsById("plannerBucket-id").patch(requestBody, headers);
}


```