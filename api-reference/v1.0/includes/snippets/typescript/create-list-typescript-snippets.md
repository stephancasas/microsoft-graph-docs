---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new List();
requestBody.displayName = "Books";
const columndefinition = new ColumnDefinition();
columndefinition.additionalData = {
					 "name" : "Author",
				 }
const columndefinition1 = new ColumnDefinition();
columndefinition1.additionalData = {
					 "name" : "PageCount",
				 }
requestBody.columns = [
			columndefinition,
			columndefinition1
		]
requestBody.list = new ListInfo();
requestBody.list.template = "genericList";
const result = async () => {
	await graphServiceClient.sitesById("site-id").lists.post(requestBody);
}


```