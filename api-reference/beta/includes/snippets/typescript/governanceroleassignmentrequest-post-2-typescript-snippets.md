---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GovernanceRoleAssignmentRequest();
requestBody.roleDefinitionId = "8b4d1d51-08e9-4254-b0a6-b16177aae376";
requestBody.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
requestBody.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
requestBody.assignmentState = "Active";
requestBody.type = "UserAdd";
requestBody.reason = "Activate the owner role";
requestBody.schedule = new GovernanceSchedule();
requestBody.schedule.type = "Once";
requestBody.schedule.startDateTime =  new Date("2018-05-12T23:28:43.537Z");
requestBody.schedule.duration = "PT9H";
requestBody.linkedEligibleRoleAssignmentId = "e327f4be-42a0-47a2-8579-0a39b025b394";
const result = async () => {
	await graphServiceClient.privilegedAccessById("privilegedAccess-id").roleAssignmentRequests.post(requestBody);
}


```