---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Group();
requestBody.description = "Group assignable to a role";
requestBody.displayName = "Role assignable group";
requestBody.groupTypes = [
			"Unified"
		]
requestBody.isAssignableToRole = true;
requestBody.mailEnabled = true;
requestBody.securityEnabled = true;
requestBody.mailNickname = "contosohelpdeskadministrators";
requestBody.additionalData = {
		 "owners@odata.bind" : [
				"https://graph.microsoft.com/beta/users/99e44b05-c10b-4e95-a523-e2732bbaba1e"
			]
		 "members@odata.bind" : [
				"https://graph.microsoft.com/beta/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0",
				"https://graph.microsoft.com/beta/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e"
			]
	 }
const result = async () => {
	await graphServiceClient.groups.post(requestBody);
}


```