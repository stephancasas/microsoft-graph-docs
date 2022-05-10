---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

let requestParameters = {
	filter : "userConsentRequests/any",
};
const result = async () => {
	await graphServiceClient.identityGovernance.appConsent.appConsentRequestsById("appConsentRequest-id").get(requestParameters);
}


```