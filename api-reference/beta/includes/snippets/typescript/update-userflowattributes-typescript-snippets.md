---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityUserFlowAttribute();
requestBody.description = "Your new hobby";
const result = async () => {
	await graphServiceClient.identity.userFlowAttributesById("identityUserFlowAttribute-id").patch(requestBody);
}


```