---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SectionGroup();
requestBody.displayName = "Section group name";
const result = async () => {
	await graphServiceClient.me.onenote.notebooksById("notebook-id").sectionGroups.post(requestBody);
}


```