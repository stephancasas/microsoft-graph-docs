---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CustomAccessPackageWorkflowExtension();
requestBody.displayName = "test_action_0124";
requestBody.description = "this is for graph testing only";
requestBody.endpointConfiguration = new CustomExtensionEndpointConfiguration();
requestBody.endpointConfiguration.additionalData = {
			 "@odata.type" : "#microsoft.graph.logicAppTriggerEndpointConfiguration",
			 "subscriptionId" : "38ab2ccc-3747-4567-b36b-9478f5602f0d",
			 "resourceGroupName" : "EMLogicApp",
			 "logicAppWorkflowName" : "customextension_test"
		 }
requestBody.authenticationConfiguration = new CustomExtensionAuthenticationConfiguration();
requestBody.authenticationConfiguration.additionalData = {
			 "@odata.type" : "#microsoft.graph.azureAdTokenAuthentication",
			 "resourceId" : "f604bd15-f785-4309-ad7c-6fad18ddb6cb"
		 }
const result = async () => {
	await graphServiceClient.identityGovernance.entitlementManagement.accessPackageCatalogsById("accessPackageCatalog-id").customAccessPackageWorkflowExtensions.post(requestBody);
}


```