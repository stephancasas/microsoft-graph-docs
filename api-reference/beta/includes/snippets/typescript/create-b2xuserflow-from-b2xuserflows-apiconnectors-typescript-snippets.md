---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new B2xIdentityUserFlow();
requestBody.id = "UserFlowWithAPIConnector";
requestBody.userFlowType = UserFlowType.SignUpOrSignIn;
requestBody.userFlowTypeVersion = 1;
requestBody.apiConnectorConfiguration = new UserFlowApiConnectorConfiguration();
requestBody.apiConnectorConfiguration.postFederationSignup = new IdentityApiConnector();
requestBody.apiConnectorConfiguration.postFederationSignup.additionalData = {
				 "@odata.id" : "{apiConnectorId}"
			 }
requestBody.apiConnectorConfiguration.postAttributeCollection = new IdentityApiConnector();
requestBody.apiConnectorConfiguration.postAttributeCollection.additionalData = {
				 "@odata.id" : "{apiConnectorId}"
			 }
const result = async () => {
	await graphServiceClient.identity.b2xUserFlows.post(requestBody);
}


```