---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthenticationFlowsPolicy();
requestBody.selfServiceSignUp = new SelfServiceSignUpAuthenticationFlowConfiguration();
requestBody.selfServiceSignUp.isEnabled = true;
const result = async () => {
	await graphServiceClient.policies.authenticationFlowsPolicy.patch(requestBody);
}


```