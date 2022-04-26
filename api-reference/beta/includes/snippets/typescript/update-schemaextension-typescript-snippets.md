---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SchemaExtension();
requestBody.owner = "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa";
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
const extensionschemaproperty3 = new ExtensionSchemaProperty();
extensionschemaproperty3.additionalData = {
					 "name" : "courseSupervisors",
					 "type" : "String"
				 }
requestBody.properties = [
			extensionschemaproperty,
			extensionschemaproperty1,
			extensionschemaproperty2,
			extensionschemaproperty3
		]
const result = async () => {
	await graphServiceClient.schemaExtensionsById("schemaExtension-id").patch(requestBody);
}


```