---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new TransferRequestBody();
requestBody.transferTarget = new InvitationParticipantInfo();
requestBody.transferTarget.endpointType = EndpointType.Default;
requestBody.transferTarget.identity = new IdentitySet();
requestBody.transferTarget.identity.user = new Identity();
requestBody.transferTarget.identity.user.id = "550fae72-d251-43ec-868c-373732c2704f";
requestBody.transferTarget.identity.user.displayName = "Heidi Steen";
requestBody.transferTarget.identity.user.additionalData = {
					 "@odata.type" : "#microsoft.graph.identity",
					 "tenantId" : "72f988bf-86f1-41af-91ab-2d7cd011db47"
				 }
requestBody.transferTarget.identity.additionalData = {
				 "@odata.type" : "#microsoft.graph.identitySet"
			 }
requestBody.transferTarget.replacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d";
requestBody.transferTarget.additionalData = {
			 "@odata.type" : "#microsoft.graph.invitationParticipantInfo",
			 "languageId" : "en-us",
			 "region" : "amer"
		 }
async () => {
	await graphServiceClient.communications.callsById("call-id").transfer.post(requestBody);
}


```