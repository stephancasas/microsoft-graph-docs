---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new InviteRequestBody();
const invitationparticipantinfo = new InvitationParticipantInfo();
invitationparticipantinfo.additionalData = {
					 "@odata.type" : "#microsoft.graph.invitationParticipantInfo",
						 ["@odata.type" , "#microsoft.graph.identitySet"],
							 ["@odata.type" , "#microsoft.graph.identity"],
							 ["id" , "+12345678901"],
				 }
requestBody.participants = [
			invitationparticipantinfo
		]
requestBody.clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").participants.invite.post(requestBody);
}


```