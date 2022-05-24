---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CustomSecurityAttributeDefinition();
requestBody.attributeSet = "Engineering";
requestBody.description = "Active projects for user";
requestBody.isCollection = true;
requestBody.isSearchable = true;
requestBody.name = "Project";
requestBody.status = "Available";
requestBody.type = "String";
requestBody.usePreDefinedValuesOnly = true;
const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.post(requestBody);
}


```