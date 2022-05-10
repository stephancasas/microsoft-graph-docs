---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SecureScoreControlProfile();
requestBody.vendorInformation = new SecurityVendorInformation();
requestBody.vendorInformation.provider = "SecureScore";
requestBody.vendorInformation.providerVersion = null,
requestBody.vendorInformation.subProvider = null,
requestBody.vendorInformation.vendor = "Microsoft";
requestBody.additionalData = {
		 "assignedTo" : "",
		 "comment" : "control is reviewed",
		 "state" : "Reviewed"
	 }
const result = async () => {
	await graphServiceClient.security.secureScoreControlProfilesById("secureScoreControlProfile-id").patch(requestBody);
}


```