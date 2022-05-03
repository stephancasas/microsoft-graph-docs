---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new RestartRequestBody();
requestBody.criteria = new SynchronizationJobRestartCriteria();
requestBody.criteria.resetScope = SynchronizationJobRestartScope.Watermark, Escrows, QuarantineState;
const headers = {
	"Authorization": "Bearer <token>",
};
async () => {
	await graphServiceClient.servicePrincipalsById("servicePrincipal-id").synchronization.jobsById("synchronizationJob-id").restart.post(requestBody, headers);
}


```