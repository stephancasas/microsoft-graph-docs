---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedGroupSource();
requestBody.includedSources = SourceType.Mailbox, site;
requestBody.additionalData = {
		 "group@odata.bind" : "https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84"
	 }
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").custodiansById("custodian-id").unifiedGroupSources.post(requestBody);
}


```