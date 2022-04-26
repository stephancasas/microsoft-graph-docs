---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AuthenticationMethodConfiguration();
requestBody.state = AuthenticationMethodState.Enabled;
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.fido2AuthenticationMethodConfiguration",
		 "isAttestationEnforced" : "true"
	 }
const result = async () => {
	await graphServiceClient.policies.authenticationMethodsPolicy.authenticationMethodConfigurationsById("authenticationMethodConfiguration-id").patch(requestBody);
}


```