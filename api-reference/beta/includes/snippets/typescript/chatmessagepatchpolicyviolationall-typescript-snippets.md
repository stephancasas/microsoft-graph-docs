---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ChatMessage();
requestBody.policyViolation = new ChatMessagePolicyViolation();
requestBody.policyViolation.policyTip = new ChatMessagePolicyViolationPolicyTip();
requestBody.policyViolation.policyTip.generalText = "This item has been blocked by the administrator.";
requestBody.policyViolation.policyTip.complianceUrl = "https://contoso.com/dlp-policy-page";
requestBody.policyViolation.policyTip.matchedConditionDescriptions = [
					"Credit Card Number"
				]
requestBody.policyViolation.verdictDetails = ChatMessagePolicyViolationVerdictDetailsTypes.AllowOverrideWithoutJustification,AllowFalsePositiveOverride;
requestBody.policyViolation.dlpAction = ChatMessagePolicyViolationDlpActionTypes.BlockAccess;
const result = async () => {
	await graphServiceClient.teamsById("team-id").channelsById("channel-id").messagesById("chatMessage-id").patch(requestBody);
}


```