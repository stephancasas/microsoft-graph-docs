---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AttributeSet();
requestBody.id = "Engineering";
requestBody.description = "Attributes for engineering team";
requestBody.maxAttributesPerSet = 25;
const result = async () => {
	await graphServiceClient.directory.attributeSets.post(requestBody);
}


```