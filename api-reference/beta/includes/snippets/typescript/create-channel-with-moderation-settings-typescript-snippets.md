---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Channel();
requestBody.displayName = "TestChannelModeration";
requestBody.description = "Test channel moderation.";
requestBody.membershipType = ChannelMembershipType.Standard;
requestBody.moderationSettings = new ChannelModerationSettings();
requestBody.moderationSettings.userNewMessageRestriction = UserNewMessageRestriction.EveryoneExceptGuests;
requestBody.moderationSettings.replyRestriction = ReplyRestriction.Everyone;
requestBody.moderationSettings.allowNewMessageFromBots = true;
requestBody.moderationSettings.allowNewMessageFromConnectors = true;
const result = async () => {
	await graphServiceClient.teamsById("team-id").channels.post(requestBody);
}


```