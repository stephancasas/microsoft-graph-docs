---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "%20",
};
const result = async () => {
	await graphServiceClient.identityGovernance.appConsent.appConsentRequestsById("appConsentRequest-id").userConsentRequestsById("userConsentRequest-id").get(requestParameters);
}


```