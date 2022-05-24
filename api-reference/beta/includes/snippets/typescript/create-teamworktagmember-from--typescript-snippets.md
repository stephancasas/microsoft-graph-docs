---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TeamworkTagMember();
requestBody.userId = "97f62344-57dc-409c-88ad-c4af14158ff5";
const result = async () => {
	await graphServiceClient.teamsById("team-id").tagsById("teamworkTag-id").members.post(requestBody);
}


```