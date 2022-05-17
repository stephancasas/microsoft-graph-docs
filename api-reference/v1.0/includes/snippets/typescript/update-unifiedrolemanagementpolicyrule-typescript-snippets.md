---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new UnifiedRoleManagementPolicyRule();
requestBody.id = "Expiration_EndUser_Assignment";
requestBody.target = new UnifiedRoleManagementPolicyRuleTarget();
requestBody.target.caller = "EndUser";
requestBody.target.operations = [
				"All"
			]
requestBody.target.level = "Assignment";
requestBody.target.inheritableSettings = [
			]
requestBody.target.enforcedSettings = [
			]
requestBody.target.additionalData = {
			 "@odata.type" : "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.unifiedRoleManagementPolicyExpirationRule",
		 "isExpirationRequired" : true,
		 "maximumDuration" : "PT1H45M"
	 }
const result = async () => {
	await graphServiceClient.policies.roleManagementPoliciesById("unifiedRoleManagementPolicy-id").rulesById("unifiedRoleManagementPolicyRule-id").patch(requestBody);
}


```