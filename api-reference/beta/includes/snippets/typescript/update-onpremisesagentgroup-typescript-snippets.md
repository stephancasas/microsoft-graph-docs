---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OnPremisesAgentGroup();
requestBody.displayName = "Group New Name";
const result = async () => {
	await graphServiceClient.onPremisesPublishingProfilesById("onPremisesPublishingProfile-id").agentGroupsById("onPremisesAgentGroup-id").patch(requestBody);
}


```