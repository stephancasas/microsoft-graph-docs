---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GovernanceRoleAssignmentRequest();
requestBody.roleDefinitionId = "0e88fd18-50f5-4ee1-9104-01c3ed910065";
requestBody.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
requestBody.subjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6";
requestBody.assignmentState = "Eligible";
requestBody.type = "AdminExtend";
requestBody.reason = "extend role assignment";
requestBody.schedule = new GovernanceSchedule();
requestBody.schedule.type = "Once";
requestBody.schedule.startDateTime =  new Date("2018-05-12T23:53:55.327Z");
requestBody.schedule.endDateTime =  new Date("2018-08-10T23:53:55.327Z");
const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleAssignmentRequests.post(requestBody);
}


```