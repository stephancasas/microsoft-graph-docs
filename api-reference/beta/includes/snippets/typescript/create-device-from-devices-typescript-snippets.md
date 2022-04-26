---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Device();
requestBody.accountEnabled = true;
const alternativesecurityid = new AlternativeSecurityId();
alternativesecurityid.additionalData = {
					 "type" : 99,
					 "identityProvider" : "identityProvider-value",
					 "key" : "base64Y3YxN2E1MWFlYw=="
				 }
requestBody.alternativeSecurityIds = [
			alternativesecurityid
		]
requestBody.approximateLastSignInDateTime =  new Date("2016-10-19T10:37:00Z");
requestBody.deviceId = "deviceId-value";
requestBody.deviceMetadata = "deviceMetadata-value";
requestBody.deviceVersion = 99;
const result = async () => {
	await graphServiceClient.devices.post(requestBody);
}


```