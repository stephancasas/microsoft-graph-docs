---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TimeOffReason();
requestBody.displayName = "Vacation";
requestBody.iconType = TimeOffReasonIconType.Plane;
requestBody.isActive = true;
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeOffReasons.post(requestBody);
}


```