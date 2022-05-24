---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Device();
requestBody.accountEnabled = false;
const alternativesecurityid = new AlternativeSecurityId();
alternativesecurityid.additionalData = {
					 "type" : 2,
					 "key" : "base64Y3YxN2E1MWFlYw=="
				 }
requestBody.alternativeSecurityIds = [
			alternativesecurityid
		]
requestBody.deviceId = "4c299165-6e8f-4b45-a5ba-c5d250a707ff";
requestBody.displayName = "Test device";
requestBody.operatingSystem = "linux";
requestBody.operatingSystemVersion = "1";
const result = async () => {
	await graphServiceClient.devices.post(requestBody);
}


```