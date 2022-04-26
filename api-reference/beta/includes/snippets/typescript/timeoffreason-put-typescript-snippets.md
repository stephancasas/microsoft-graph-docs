---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new {timeOffReasonId}RequestBody();
requestBody.additionalData = {
		 "displayName" : "Vacation",
		 "iconType" : "plane",
		 "isActive" : true
	 }
const headers = {
	"Prefer": "return=representation",
};
async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeOffReasonsById("timeOffReason-id").put(requestBody, headers);
}


```