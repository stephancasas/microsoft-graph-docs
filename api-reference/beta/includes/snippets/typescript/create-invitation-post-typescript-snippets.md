---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Invitation();
requestBody.invitedUserEmailAddress = "admin@fabrikam.com";
requestBody.inviteRedirectUrl = "https://myapp.contoso.com";
const result = async () => {
	await graphServiceClient.invitations.post(requestBody);
}


```