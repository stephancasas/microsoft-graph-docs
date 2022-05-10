---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new GrantRequestBody();
const driverecipient = new DriveRecipient();
driverecipient.additionalData = {
					 "email" : "john@contoso.com"
				 }
const driverecipient1 = new DriveRecipient();
driverecipient1.additionalData = {
					 "email" : "ryan@external.com"
				 }
requestBody.recipients = [
			driverecipient,
			driverecipient1
		]
requestBody.roles = [
			"read"
		]
const result = async () => {
	await graphServiceClient.sharesById("sharedDriveItem-id").permission.grant.post(requestBody);
}


```