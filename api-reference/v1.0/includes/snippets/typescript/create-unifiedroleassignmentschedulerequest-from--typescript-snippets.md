---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignmentScheduleRequest();
requestBody.action = UnifiedRoleScheduleRequestActions.AdminAssign;
requestBody.justification = "Assign Groups Admin to IT Helpdesk group";
requestBody.roleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c";
requestBody.directoryScopeId = "/";
requestBody.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
requestBody.scheduleInfo = new RequestSchedule();
requestBody.scheduleInfo.startDateTime =  new Date("2022-04-10T00:00:00Z");
requestBody.scheduleInfo.expiration = new ExpirationPattern();
requestBody.scheduleInfo.expiration.type = ExpirationPatternType.NoExpiration;
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignmentScheduleRequests.post(requestBody);
}


```