---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new OutlookCategory();
requestBody.displayName = "Project expenses";
requestBody.color = CategoryColor.Preset9;
const result = async () => {
	await graphServiceClient.me.outlook.masterCategories.post(requestBody);
}


```