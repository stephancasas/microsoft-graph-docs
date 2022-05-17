---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SchemaExtension();
requestBody.id = "graphlearn_courses";
requestBody.description = "Graph Learn training courses extensions";
requestBody.targetTypes = [
			"Group"
		]
const extensionschemaproperty = new ExtensionSchemaProperty();
extensionschemaproperty.additionalData = {
					 "name" : "courseId",
					 "type" : "Integer"
				 }
const extensionschemaproperty1 = new ExtensionSchemaProperty();
extensionschemaproperty1.additionalData = {
					 "name" : "courseName",
					 "type" : "String"
				 }
const extensionschemaproperty2 = new ExtensionSchemaProperty();
extensionschemaproperty2.additionalData = {
					 "name" : "courseType",
					 "type" : "String"
				 }
requestBody.properties = [
			extensionschemaproperty,
			extensionschemaproperty1,
			extensionschemaproperty2
		]
const result = async () => {
	await graphServiceClient.schemaExtensions.post(requestBody);
}


```