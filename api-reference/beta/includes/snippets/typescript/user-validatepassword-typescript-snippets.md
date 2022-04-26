---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ValidatePasswordRequestBody();
requestBody.password = "1234567890";
const result = async () => {
	await graphServiceClient.users.validatePassword.post(requestBody);
}


```