---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	top : 2,
	filter : "state%20eq%20'clockedOut'",
};
const result = async () => {
	await graphServiceClient.teamsById("team-id").schedule.timeCards.get(requestParameters);
}


```