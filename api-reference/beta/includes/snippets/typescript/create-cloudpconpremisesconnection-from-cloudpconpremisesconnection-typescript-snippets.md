---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcOnPremisesConnection();
requestBody.displayName = "test-canary-02";
requestBody.type = CloudPcOnPremisesConnectionType.HybridAzureADJoin;
requestBody.subscriptionId = "0ac520ee-14c0-480f-b6c9-0a90c585ffff";
requestBody.subscriptionName = "CPC customer 001 test subscription";
requestBody.adDomainName = "contoso001.com";
requestBody.adDomainUsername = "dcadmin";
requestBody.organizationalUnit = "OU=Domain Controllers, DC=contoso001, DC=com";
requestBody.resourceGroupId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG";
requestBody.virtualNetworkId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET";
requestBody.subnetId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ad47/resourceGroups/CustomerRG/providers/Microsoft.Network/virtualNetworks/canary01-MyVNET/subnets/canary01-Subnet";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcOnPremisesConnection"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.onPremisesConnections.post(requestBody);
}


```