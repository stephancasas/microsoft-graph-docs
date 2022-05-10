---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AttributeSet();
requestBody.description = "Attributes for engineering team";
requestBody.maxAttributesPerSet = 20;
const result = async () => {
	await graphServiceClient.directory.attributeSetsById("attributeSet-id").patch(requestBody);
}


```