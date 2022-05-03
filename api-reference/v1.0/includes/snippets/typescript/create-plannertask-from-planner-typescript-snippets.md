---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerTask();
requestBody.planId = "xqQg5FS2LkCp935s-FIFm2QAFkHM";
requestBody.bucketId = "hsOf2dhOJkqyYYZEtdzDe2QAIUCR";
requestBody.title = "Update client list";
requestBody.assignments = new PlannerAssignments();
requestBody.assignments.additionalData = {
				 ["@odata.type" , "#microsoft.graph.plannerAssignment"],
				 ["orderHint" , " !"],
		 }
const result = async () => {
	await graphServiceClient.planner.tasks.post(requestBody);
}


```