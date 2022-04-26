---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TransferRequestBody();
requestBody.transferTarget = new InvitationParticipantInfo();
requestBody.transferTarget.identity = new IdentitySet();
requestBody.transferTarget.identity.user = new Identity();
requestBody.transferTarget.identity.user.id = "550fae72-d251-43ec-868c-373732c2704f";
requestBody.transferTarget.identity.user.displayName = "Heidi Steen";
requestBody.transferTarget.additionalData = {
			 "endpointType" : "default"
		 }
requestBody.transferee = new ParticipantInfo();
requestBody.transferee.identity = new IdentitySet();
requestBody.transferee.identity.user = new Identity();
requestBody.transferee.identity.user.id = "751f6800-3180-414d-bd94-333364659951";
requestBody.transferee.identity.user.additionalData = {
					 "tenantId" : "72f988bf-86f1-41af-91ab-2d7cd011db47"
				 }
requestBody.transferee.participantId = "909c6581-5130-43e9-88f3-fcb3582cde37";
async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```