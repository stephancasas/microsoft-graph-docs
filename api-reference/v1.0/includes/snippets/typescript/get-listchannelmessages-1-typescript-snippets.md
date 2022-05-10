---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	top : 3,
};
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messages.get(requestParameters);
}


```