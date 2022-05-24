---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleEligibilityScheduleRequest();
requestBody.action = UnifiedRoleScheduleRequestActions.AdminAssign;
requestBody.justification = "Assign Attribute Assignment Admin eligibility to restricted user";
requestBody.roleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4";
requestBody.directoryScopeId = "/";
requestBody.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
requestBody.scheduleInfo = new RequestSchedule();
requestBody.scheduleInfo.startDateTime =  new Date("2022-04-10T00:00:00Z");
requestBody.scheduleInfo.expiration = new ExpirationPattern();
requestBody.scheduleInfo.expiration.type = ExpirationPatternType.AfterDateTime;
requestBody.scheduleInfo.expiration.endDateTime =  new Date("2024-04-10T00:00:00Z");
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleEligibilityScheduleRequests.post(requestBody);
}


```