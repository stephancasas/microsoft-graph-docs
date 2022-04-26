---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TransferRequestBody();
requestBody.transferTarget = new InvitationParticipantInfo();
requestBody.transferTarget.identity = new IdentitySet();
requestBody.transferTarget.identity.additionalData = {
					 ["@odata.type" , "#microsoft.graph.identity"],
					 ["id" , "+12345678901"],
			 }
requestBody.transferTarget.additionalData = {
			 "endpointType" : "default",
			 "languageId" : "languageId-value",
			 "region" : "region-value"
		 }
requestBody.additionalData = {
		 "clientContext" : "9e90d1c1-f61e-43e7-9f75-d420159aae08"
	 }
async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```