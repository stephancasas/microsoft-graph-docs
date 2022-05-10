---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Term();
const localizedlabel = new LocalizedLabel();
localizedlabel.additionalData = {
					 "languageTag" : "en-US",
					 "name" : "Car",
					 "isDefault" : true
				 }
requestBody.labels = [
			localizedlabel
		]
const result = async () => {
	await graphServiceClient.termStore.setsById("set-id").children.post(requestBody);
}


```