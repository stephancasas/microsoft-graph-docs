---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UserSource();
requestBody.email = "megan@contoso.com";
requestBody.includedSources = SourceType.Mailbox, site;
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").custodiansById("custodian-id").userSources.post(requestBody);
}


```