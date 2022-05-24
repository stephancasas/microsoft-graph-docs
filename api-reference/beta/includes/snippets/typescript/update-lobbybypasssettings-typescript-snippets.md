---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OnlineMeeting();
requestBody.lobbyBypassSettings = new LobbyBypassSettings();
requestBody.lobbyBypassSettings.isDialInBypassEnabled = true;
const result = async () => {
	await graphServiceClient.me.onlineMeetingsById("onlineMeeting-id").patch(requestBody);
}


```