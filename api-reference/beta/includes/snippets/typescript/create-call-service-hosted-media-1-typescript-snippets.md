---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Call();
requestBody.callbackUri = "https://bot.contoso.com/callback";
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
requestBody.callOptions = new CallOptions();
requestBody.callOptions.isContentSharingNotificationEnabled = true;
requestBody.callOptions.additionalData = {
			 "@odata.type" : "#microsoft.graph.outgoingCallOptions"
		 }
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = {
			 "@odata.type" : "#microsoft.graph.serviceHostedMediaConfig"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.call"
	 }
const result = async () => {
	await graphServiceClient.communications.calls.post(requestBody);
}


```