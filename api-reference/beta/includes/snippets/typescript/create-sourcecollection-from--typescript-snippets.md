---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SourceCollection();
requestBody.displayName = "Quarterly Financials search";
requestBody.contentQuery = "subject:'Quarterly Financials'";
requestBody.additionalData = {
		 "custodianSources@odata.bind" : [
				"https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735"
			]
	 }
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").sourceCollections.post(requestBody);
}


```