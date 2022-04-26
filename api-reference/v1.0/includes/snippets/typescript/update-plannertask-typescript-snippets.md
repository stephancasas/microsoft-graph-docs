---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PlannerTask();
requestBody.assignments = new PlannerAssignments();
requestBody.assignments.additionalData = {
				 ["@odata.type" , "#microsoft.graph.plannerAssignment"],
				 ["orderHint" , "N9917 U2883!"],
		 }
requestBody.appliedCategories = new PlannerAppliedCategories();
requestBody.appliedCategories.additionalData = {
			 "category3" : true,
			 "category4" : false
		 }
const headers = {
	"Prefer": "return=representation",
	"If-Match": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
};
const result = async () => {
	await graphServiceClient.planner.tasksById("plannerTask-id").patch(requestBody, headers);
}


```