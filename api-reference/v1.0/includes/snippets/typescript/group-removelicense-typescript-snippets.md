---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AssignLicenseRequestBody();
requestBody.addLicenses = [
		]
requestBody.removeLicenses = [
			"c7df2760-2c81-4ef7-b578-5b5392b571df",
			"b05e124f-c7cc-45a0-a6aa-8cf78c946968"
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").assignLicense.post(requestBody);
}


```