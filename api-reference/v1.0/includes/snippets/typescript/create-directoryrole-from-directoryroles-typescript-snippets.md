---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DirectoryRole();
requestBody.roleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1";
const result = async () => {
	await graphServiceClient.directoryRoles.post(requestBody);
}


```