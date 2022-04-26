---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Agreement();
requestBody.displayName = "Contoso ToU for guest users";
requestBody.isViewingBeforeAcceptanceRequired = true;
const agreementfilelocalization = new AgreementFileLocalization();
agreementfilelocalization.additionalData = {
					 "fileName" : "TOU.pdf",
					 "language" : "en",
					 "isDefault" : true,
						 ["data" , "SGVsbG8gd29ybGQ=//truncated-binary"],
				 }
requestBody.files = [
			agreementfilelocalization
		]
const result = async () => {
	await graphServiceClient.identityGovernance.termsOfUse.agreements.post(requestBody);
}


```