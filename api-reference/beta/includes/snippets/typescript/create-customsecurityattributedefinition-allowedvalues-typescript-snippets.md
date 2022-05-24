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
const allowedvalue = new AllowedValue();
allowedvalue.additionalData = {
					 "id" : "Alpine",
					 "isActive" : true
				 }
const allowedvalue1 = new AllowedValue();
allowedvalue1.additionalData = {
					 "id" : "Baker",
					 "isActive" : true
				 }
const allowedvalue2 = new AllowedValue();
allowedvalue2.additionalData = {
					 "id" : "Cascade",
					 "isActive" : true
				 }
requestBody.allowedValues = [
			allowedvalue,
			allowedvalue1,
			allowedvalue2
		]
const result = async () => {
	await graphServiceClient.directory.customSecurityAttributeDefinitions.post(requestBody);
}


```