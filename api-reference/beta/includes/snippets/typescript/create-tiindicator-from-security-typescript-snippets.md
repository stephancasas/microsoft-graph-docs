---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TiIndicator();
requestBody.action = TiAction.Alert;
requestBody.activityGroupNames = [
		]
requestBody.confidence = 0;
requestBody.description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator.";
requestBody.expirationDateTime =  new Date("2019-03-01T21:43:37.5031462+00:00");
requestBody.externalId = "Test--8586509942679764298MS501";
requestBody.fileHashType = FileHashType.Sha256;
requestBody.fileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313";
requestBody.killChain = [
		]
requestBody.malwareFamilyNames = [
		]
requestBody.severity = 0;
requestBody.tags = [
		]
requestBody.targetProduct = "Azure Sentinel";
requestBody.threatType = "WatchList";
requestBody.tlpLevel = TlpLevel.Green;
const result = async () => {
	await graphServiceClient.security.tiIndicators.post(requestBody);
}


```