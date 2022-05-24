---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AdministrativeUnit();
requestBody.displayName = "Seattle District Technical Schools";
requestBody.description = "Seattle district technical schools administration";
requestBody.visibility = "HiddenMembership";
const result = async () => {
	await graphServiceClient.administrativeUnits.post(requestBody);
}


```