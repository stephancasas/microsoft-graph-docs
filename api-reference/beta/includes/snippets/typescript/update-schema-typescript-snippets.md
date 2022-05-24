---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Schema();
requestBody.baseType = "microsoft.graph.externalItem";
const property = new Property();
property.additionalData = {
					 "name" : "ticketTitle",
					 "type" : "string",
					 "isSearchable" : "true",
					 "isRetrievable" : "true",
					 "labels" : [
							"title"
						]
				 }
const property1 = new Property();
property1.additionalData = {
					 "name" : "priority",
					 "type" : "string",
					 "isQueryable" : "true",
					 "isRetrievable" : "true",
					 "isSearchable" : "false"
				 }
const property2 = new Property();
property2.additionalData = {
					 "name" : "assignee",
					 "type" : "string",
					 "isRetrievable" : "true"
				 }
requestBody.properties = [
			property,
			property1,
			property2
		]
const result = async () => {
	await graphServiceClient.external.connectionsById("externalConnection-id").schema.patch(requestBody);
}


```