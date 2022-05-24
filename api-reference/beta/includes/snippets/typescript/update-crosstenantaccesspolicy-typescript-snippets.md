---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CrossTenantAccessPolicy();
requestBody.additionalData = {
		 "allowedCloudEndpoints" : [
				"microsoftonline.us",
				"partner.microsoftonline.cn"
			]
	 }
const result = async () => {
	await graphServiceClient.policies.crossTenantAccessPolicy.patch(requestBody);
}


```