---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ReferenceUpdateSchema();
requestBody.@odata.id = "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}";
const result = async () => {
	await graphServiceClient.applicationsById("application-id").connectorGroup.$ref.put(requestBody);
}


```