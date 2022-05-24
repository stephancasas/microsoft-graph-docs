---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReferenceUpdateSchema();
requestBody.@odata.id = "https://graph.microsoft.com/v1.0/education/me/rubrics/{id}";
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").rubric.$ref.put(requestBody);
}


```