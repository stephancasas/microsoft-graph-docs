---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PrivilegedRoleAssignmentRequest();
requestBody.duration = "2";
requestBody.reason = "Activate the role for business purpose";
requestBody.ticketNumber = "234";
requestBody.ticketSystem = "system";
requestBody.schedule = new GovernanceSchedule();
requestBody.schedule.startDateTime =  new Date("2018-02-08T02:35:17.903Z");
requestBody.type = "UserAdd";
requestBody.assignmentState = "Active";
requestBody.roleId = "88d8e3e3-8f55-4a1e-953a-9b9898b8876b";
const result = async () => {
	await graphServiceClient.privilegedRoleAssignmentRequests.post(requestBody);
}


```