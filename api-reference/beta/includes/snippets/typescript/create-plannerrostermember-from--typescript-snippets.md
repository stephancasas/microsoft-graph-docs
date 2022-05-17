---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerRosterMember();
requestBody.userId = "String";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.plannerRosterMember"
	 }
const result = async () => {
	await graphServiceClient.planner.rostersById("plannerRoster-id").members.post(requestBody);
}


```