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
			"f30db892-07e9-47e9-837c-80727f46fd3d",
			"84a661c4-e949-4bd2-a560-ed7766fcaf2b"
		]
const result = async () => {
	await graphServiceClient.me.assignLicense.post(requestBody);
}


```