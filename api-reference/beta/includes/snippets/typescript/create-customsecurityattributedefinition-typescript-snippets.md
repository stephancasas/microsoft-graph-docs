---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CustomSecurityAttributeDefinition();
requestBody.attributeSet = "Engineering";
requestBody.description = "Target completion date";
requestBody.isCollection = false;
requestBody.isSearchable = true;
requestBody.name = "ProjectDate";
requestBody.status = "Available";
requestBody.type = "String";
requestBody.usePreDefinedValuesOnly = false;
const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.post(requestBody);
}


```