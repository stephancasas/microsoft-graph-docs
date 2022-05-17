---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SectionGroupsRequestBody();
requestBody.additionalData = {
		 "displayName" : "Section group name"
	 }
async () => {
	await graphServiceClient.me.onenote.sectionGroupsById("sectionGroup-id").sectionGroups.post(requestBody);
}


```