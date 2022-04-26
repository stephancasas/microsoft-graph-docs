---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const result = async () => {
	await graphServiceClient.appCatalogs.teamsAppsById("teamsApp-id").appDefinitionsById("teamsAppDefinition-id").outlineIcon.get();
}


```