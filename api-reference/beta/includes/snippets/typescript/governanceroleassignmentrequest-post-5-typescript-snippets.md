---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GovernanceRoleAssignmentRequest();
requestBody.roleDefinitionId = "70521f3e-3b95-4e51-b4d2-a2f485b02103";
requestBody.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
requestBody.subjectId = "1566d11d-d2b6-444a-a8de-28698682c445";
requestBody.assignmentState = "Eligible";
requestBody.type = "AdminUpdate";
requestBody.schedule = new GovernanceSchedule();
requestBody.schedule.type = "Once";
requestBody.schedule.startDateTime =  new Date("2018-03-08T05:42:45.317Z");
requestBody.schedule.endDateTime =  new Date("2018-06-05T05:42:31.000Z");
const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleAssignmentRequests.post(requestBody);
}


```