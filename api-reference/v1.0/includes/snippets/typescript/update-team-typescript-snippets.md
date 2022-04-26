---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Team();
requestBody.memberSettings = new TeamMemberSettings();
requestBody.memberSettings.allowCreateUpdateChannels = true;
requestBody.messagingSettings = new TeamMessagingSettings();
requestBody.messagingSettings.allowUserEditMessages = true;
requestBody.messagingSettings.allowUserDeleteMessages = true;
requestBody.funSettings = new TeamFunSettings();
requestBody.funSettings.allowGiphy = true;
requestBody.funSettings.giphyContentRating = GiphyRatingType.Strict;
const result = async () => {
	await graphServiceClient.teamsById("team-id").patch(requestBody);
}


```