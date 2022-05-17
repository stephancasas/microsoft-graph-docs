---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new User();
requestBody.businessPhones = [
			"+1 425 555 0109"
		]
requestBody.officeLocation = "18/2111";
const result = async () => {
	await graphServiceClient.usersById("user-id").patch(requestBody);
}


```