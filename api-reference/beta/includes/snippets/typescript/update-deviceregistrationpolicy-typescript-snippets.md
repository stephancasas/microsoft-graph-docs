---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DeviceRegistrationPolicyRequestBody();
requestBody.additionalData = {
		 "id" : "deviceRegistrationPolicy",
		 "displayName" : "Device Registration Policy",
		 "description" : "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
		 "userDeviceQuota" : 50,
		 "multiFactorAuthConfiguration" : "0",
			 ["appliesTo" , "1"],
			 ["isAdminConfigurable" , false],
			 ["allowedUsers" , [
				]
			 ["allowedGroups" , [
				]
			 ["appliesTo" , "1"],
			 ["isAdminConfigurable" , true],
			 ["allowedUsers" , [
				]
			 ["allowedGroups" , [
				]
	 }
async () => {
	await graphServiceClient.deviceRegistrationPolicy.put(requestBody);
}


```