---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleAssignmentScheduleRequest();
requestBody.action = UnifiedRoleScheduleRequestActions.SelfActivate;
requestBody.principalId = "071cc716-8147-4397-a5ba-b2105951cc0b";
requestBody.roleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4";
requestBody.directoryScopeId = "/";
requestBody.justification = "I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs";
requestBody.scheduleInfo = new RequestSchedule();
requestBody.scheduleInfo.startDateTime =  new Date("2022-04-14T00:00:00.000Z");
requestBody.scheduleInfo.expiration = new ExpirationPattern();
requestBody.scheduleInfo.expiration.type = ExpirationPatternType.AfterDuration;
requestBody.scheduleInfo.expiration.duration = "PT5H";
requestBody.ticketInfo = new TicketInfo();
requestBody.ticketInfo.ticketNumber = "CONTOSO:Normal-67890";
requestBody.ticketInfo.ticketSystem = "MS Project";
const result = async () => {
	await graphServiceClient.roleManagement.directory.roleAssignmentScheduleRequests.post(requestBody);
}


```