---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReprovisionRequestBody();
requestBody.userAccountType = CloudPcUserAccountType.Administrator;
requestBody.osVersion = CloudPcOperatingSystem.Windows10;
async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.cloudPCsById("cloudPC-id").reprovision.post(requestBody);
}


```