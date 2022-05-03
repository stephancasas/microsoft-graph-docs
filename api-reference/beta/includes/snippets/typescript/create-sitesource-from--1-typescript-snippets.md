---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SiteSource();
requestBody.site = new Site();
requestBody.site.webUrl = "https://contoso.sharepoint.com/sites/HumanResources";
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").custodiansById("custodian-id").siteSources.post(requestBody);
}


```