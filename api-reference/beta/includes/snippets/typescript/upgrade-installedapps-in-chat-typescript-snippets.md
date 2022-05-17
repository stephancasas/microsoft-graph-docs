---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

async () => {
	await graphServiceClient.chatsById("chat-id").installedAppsById("teamsAppInstallation-id").upgrade.post();
}


```