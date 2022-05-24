---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationClass();
requestBody.description = "History - World History 1";
requestBody.displayName = "World History Level 1";
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").patch(requestBody);
}


```