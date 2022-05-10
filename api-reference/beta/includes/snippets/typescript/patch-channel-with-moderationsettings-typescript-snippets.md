---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Channel();
requestBody.displayName = "UpdateChannelModeration";
requestBody.description = "Update channel moderation.";
requestBody.moderationSettings = new ChannelModerationSettings();
requestBody.moderationSettings.userNewMessageRestriction = UserNewMessageRestriction.Moderators;
requestBody.moderationSettings.replyRestriction = ReplyRestriction.Everyone;
requestBody.moderationSettings.allowNewMessageFromBots = true;
requestBody.moderationSettings.allowNewMessageFromConnectors = true;
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").patch(requestBody);
}


```