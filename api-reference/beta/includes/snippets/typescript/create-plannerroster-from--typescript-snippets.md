---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerRoster();
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.plannerRoster"
	 }
const result = async () => {
	await graphServiceClient.planner.rosters.post(requestBody);
}


```