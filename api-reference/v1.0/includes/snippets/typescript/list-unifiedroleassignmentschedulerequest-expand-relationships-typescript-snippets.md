---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	select : "principalId,action,roleDefinitionId",
	expand : "roleDefinition,activatedUsing,principal,targetSchedule",
};
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignmentScheduleRequests.get(requestParameters);
}


```