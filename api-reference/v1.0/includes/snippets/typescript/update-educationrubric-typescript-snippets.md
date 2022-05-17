---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationRubric();
requestBody.displayName = "Example Credit Rubric after display name patch";
const result = async () => {
	await graphServiceClient.education.me.rubricsById("educationRubric-id").patch(requestBody);
}


```