---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UpdateSoftwareRequestBody();
requestBody.softwareType = TeamworkSoftwareType.TeamsClient;
requestBody.softwareVersion = "1.0.96.22";
async () => {
	await graphServiceClient.teamwork.devicesById("teamworkDevice-id").updateSoftware.post(requestBody);
}


```