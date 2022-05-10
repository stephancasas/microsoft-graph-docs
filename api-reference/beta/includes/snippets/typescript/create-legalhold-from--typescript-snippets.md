---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new LegalHold();
requestBody.description = "String";
requestBody.createdBy = new IdentitySet();
requestBody.createdBy.additionalData = {
			 "@odata.type" : "microsoft.graph.identitySet"
		 }
requestBody.isEnabled = "Boolean";
requestBody.status = LegalHoldStatus.String;
requestBody.contentQuery = "String";
requestBody.errors = [
			"String"
		]
requestBody.displayName = "String";
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.ediscovery.legalHold"
	 }
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").legalHolds.post(requestBody);
}


```