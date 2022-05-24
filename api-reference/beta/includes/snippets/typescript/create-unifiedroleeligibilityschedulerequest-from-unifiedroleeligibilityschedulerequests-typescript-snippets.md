---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleEligibilityScheduleRequest();
requestBody.action = "AdminAssign";
requestBody.justification = "Assign User Admin eligibility to IT Helpdesk (User) group";
requestBody.roleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c";
requestBody.directoryScopeId = "/";
requestBody.principalId = "07706ff1-46c7-4847-ae33-3003830675a1";
requestBody.scheduleInfo = new RequestSchedule();
requestBody.scheduleInfo.startDateTime =  new Date("2021-07-01T00:00:00Z");
requestBody.scheduleInfo.expiration = new ExpirationPattern();
requestBody.scheduleInfo.expiration.endDateTime =  new Date("2022-06-30T00:00:00Z");
requestBody.scheduleInfo.expiration.type = ExpirationPatternType.AfterDateTime;
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```