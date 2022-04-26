---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ColumnDefinition();
requestBody.description = "test";
requestBody.enforceUniqueValues = false;
requestBody.hidden = false;
requestBody.indexed = false;
requestBody.name = "Title";
requestBody.text = new TextColumn();
requestBody.text.allowMultipleLines = false;
requestBody.text.appendChangesToExistingText = false;
requestBody.text.linesForEditing = 0;
requestBody.text.maxLength = 255;
const result = async () => {
	await graphServiceClient.sitesById("site-id").columns.post(requestBody);
}


```