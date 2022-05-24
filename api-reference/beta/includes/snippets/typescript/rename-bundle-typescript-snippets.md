---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new DriveItem();
requestBody.name = "Shared legal agreements";
const result = async () => {
	await graphServiceClient.drive.itemsById("driveItem-id").patch(requestBody);
}


```