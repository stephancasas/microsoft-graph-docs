---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TenantCustomizedInformation();
requestBody.tenantId = "String";
const tenantcontactinformation = new TenantContactInformation();
tenantcontactinformation.additionalData = {
					 "@odata.type" : "microsoft.graph.managedTenants.tenantContactInformation",
					 "name" : "String",
					 "title" : "String",
					 "email" : "String",
					 "phone" : "String",
					 "notes" : "String"
				 }
requestBody.contacts = [
			tenantcontactinformation
		]
requestBody.website = "String";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.managedTenants.tenantCustomizedInformation"
	 }
const result = async () => {
	await graphServiceClient.tenantRelationships.managedTenants.tenantsCustomizedInformationById("tenantCustomizedInformation-id").patch(requestBody);
}


```