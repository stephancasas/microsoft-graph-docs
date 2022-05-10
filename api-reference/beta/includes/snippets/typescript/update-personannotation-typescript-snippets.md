---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new PersonAnnotation();
requestBody.allowedAudiences = AllowedAudiences.Organization;
const result = async () => {
	await graphServiceClient.usersById("user-id").profile.notesById("personAnnotation-id").patch(requestBody);
}


```