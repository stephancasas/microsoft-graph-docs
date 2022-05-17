---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerPlan();
requestBody.container = new PlannerPlanContainer();
requestBody.container.url = "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874";
requestBody.title = "title-value";
const result = async () => {
	await graphServiceClient.planner.plans.post(requestBody);
}


```