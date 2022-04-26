---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SecurityAction();
requestBody.name = "BlockIp";
requestBody.actionReason = "Test";
const keyvaluepair = new KeyValuePair();
keyvaluepair.additionalData = {
					 "name" : "IP",
					 "value" : "1.2.3.4"
				 }
requestBody.parameters = [
			keyvaluepair
		]
requestBody.vendorInformation = new SecurityVendorInformation();
requestBody.vendorInformation.provider = "Windows Defender ATP";
requestBody.vendorInformation.vendor = "Microsoft";
const result = async () => {
	await graphServiceClient.security.securityActions.post(requestBody);
}


```