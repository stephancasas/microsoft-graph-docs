---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AdministrativeUnit();
requestBody.displayName = "Greater Seattle District Technical Schools";
const result = async () => {
	await graphServiceClient.directory.administrativeUnitsById("administrativeUnit-id").patch(requestBody);
}


```