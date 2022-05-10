---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new NoncustodialDataSource();
requestBody.applyHoldToSource = true;
requestBody.dataSource = new DataSource();
requestBody.dataSource.additionalData = {
			 "@odata.type" : "microsoft.graph.ediscovery.userSource",
			 "email" : "adelev@contoso.com"
		 }
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").noncustodialDataSources.post(requestBody);
}


```