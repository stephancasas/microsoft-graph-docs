---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ListItem();
requestBody.fields = new FieldValueSet();
requestBody.fields.additionalData = {
			 "Title" : "Widget",
			 "Color" : "Purple",
			 "Weight" : 32
		 }
const result = async () => {
	await graphServiceClient.sitesById("site-id").listsById("list-id").items.post(requestBody);
}


```