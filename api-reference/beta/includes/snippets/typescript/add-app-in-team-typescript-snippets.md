---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamsAppInstallation();
requestBody.additionalData = {
		 "teamsApp@odata.bind" : "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
	 }
const result = async () => {
	await graphServiceClient.teamsById("team-id").installedApps.post(requestBody);
}


```