---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Organization();
requestBody.marketingNotificationEmails = [
			"marketing@contoso.com"
		]
requestBody.privacyProfile = new PrivacyProfile();
requestBody.privacyProfile.contactEmail = "alice@contoso.com";
requestBody.privacyProfile.statementUrl = "https://contoso.com/privacyStatement";
requestBody.securityComplianceNotificationMails = [
			"security@contoso.com"
		]
requestBody.securityComplianceNotificationPhones = [
			"(123) 456-7890"
		]
requestBody.technicalNotificationMails = [
			"tech@contoso.com"
		]
const result = async () => {
	await graphServiceClient.organizationById("organization-id").patch(requestBody);
}


```