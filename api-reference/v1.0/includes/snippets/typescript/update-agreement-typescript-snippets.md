---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Agreement();
requestBody.displayName = "All Contoso volunteers - Terms of use";
requestBody.isViewingBeforeAcceptanceRequired = true;
const result = async () => {
	await graphServiceClient.identityGovernance.termsOfUse.agreementsById("agreement-id").patch(requestBody);
}


```