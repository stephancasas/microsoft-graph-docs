---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Call();
requestBody.callbackUri = "https://bot.contoso.com/callback";
requestBody.source = new ParticipantInfo();
requestBody.source.identity = new IdentitySet();
requestBody.source.identity.application = new Identity();
requestBody.source.identity.application.displayName = "Calling Bot";
requestBody.source.identity.application.id = "2891555a-92ff-42e6-80fa-6e1300c6b5c6";
requestBody.source.identity.application.additionalData = {
					 "@odata.type" : "#microsoft.graph.identity"
				 }
requestBody.source.identity.additionalData = {
				 "@odata.type" : "#microsoft.graph.identitySet"
			 }
requestBody.source.region = null,
requestBody.source.languageId = null,
requestBody.source.additionalData = {
			 "@odata.type" : "#microsoft.graph.participantInfo"
		 }
const invitationparticipantinfo = new InvitationParticipantInfo();
invitationparticipantinfo.additionalData = {
					 "@odata.type" : "#microsoft.graph.invitationParticipantInfo",
						 ["@odata.type" , "#microsoft.graph.identitySet"],
							 ["@odata.type" , "#microsoft.graph.identity"],
							 ["displayName" , "John"],
							 ["id" , "112f7296-5fa4-42ca-bae8-6a692b15d4b8"],
				 }
requestBody.targets = [
			invitationparticipantinfo
		]
requestBody.requestedModalities = [
			"audio"
		]
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = {
			 "@odata.type" : "#microsoft.graph.appHostedMediaConfig",
			 "blob" : "<Media Session Configuration>"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.call"
	 }
const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```