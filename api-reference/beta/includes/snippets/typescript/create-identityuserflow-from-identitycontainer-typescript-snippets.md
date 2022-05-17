---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new IdentityUserFlow();
requestBody.id = "Pol1";
requestBody.userFlowType = UserFlowType.SignUpOrSignIn;
requestBody.userFlowTypeVersion = 1;
const result = async () => {
	await graphServiceClient.identity.userFlows.post(requestBody);
}


```