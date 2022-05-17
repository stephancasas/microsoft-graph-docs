---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new CloudPcOrganizationSettings();
requestBody.userAccountType = CloudPcUserAccountType.StandardUser;
requestBody.osVersion = CloudPcOperatingSystem.Windows11;
requestBody.windowsSettings = new CloudPcWindowsSettings();
requestBody.windowsSettings.language = "en-US";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.cloudPcOrganizationSettings"
	 }
const result = async () => {
	await graphServiceClient.deviceManagement.virtualEndpoint.organizationSettings.patch(requestBody);
}


```