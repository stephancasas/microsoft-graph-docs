---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ShareRequestBody();
requestBody.notifyTeam = true;
requestBody.startDateTime =  new Date("2018-10-08T00:00:00.000Z");
requestBody.endDateTime =  new Date("2018-10-15T00:00:00.000Z");
async () => {
	await graphServiceClient.teamsById("team-id").schedule.share.post(requestBody);
}


```