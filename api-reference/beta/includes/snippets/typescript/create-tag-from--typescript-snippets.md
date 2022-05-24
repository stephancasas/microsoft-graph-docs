---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Tag();
requestBody.displayName = "Privileged";
requestBody.description = "The document is privileged";
requestBody.additionalData = {
		 "parent@odata.bind" : "https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3"
	 }
const result = async () => {
	await graphServiceClient.compliance.ediscovery.casesById("case-id").tags.post(requestBody);
}


```