---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationUser();
requestBody.displayName = "Rogelio Cazares";
requestBody.givenName = "Rogelio";
requestBody.middleName = "Fernando";
requestBody.surname = "Cazares";
const result = async () => {
	await graphServiceClient.education.usersById("educationUser-id").patch(requestBody);
}


```