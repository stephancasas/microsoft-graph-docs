---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new $refRequestBody();
requestBody.additionalData = {
		 "@odata.id" : "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
	 }
const result = async () => {
	await graphServiceClient.onPremisesPublishingProfilesById("onPremisesPublishingProfile-id").connectorGroupsById("connectorGroup-id").members.$ref.post(requestBody);
}


```