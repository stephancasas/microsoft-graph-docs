---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcOnPremisesConnection();
requestBody.displayName = "Display Name value";
requestBody.subscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff";
requestBody.subscriptionName = "Subscription Name value";
requestBody.adDomainName = "Active Directory Domain Name value";
requestBody.adDomainUsername = "Active Directory Domain User Name value";
requestBody.organizationalUnit = "Organization Unit value";
requestBody.resourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG";
requestBody.virtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet";
requestBody.subnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcOnPremisesConnection"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.onPremisesConnectionsById("cloudPcOnPremisesConnection-id").patch(requestBody);
}


```