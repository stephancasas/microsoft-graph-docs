---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamworkTag();
requestBody.displayName = "Finance";
const result = async () => {
	await graphServiceClient.teamsById("team-id").tagsById("teamworkTag-id").patch(requestBody);
}


```