---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Team();
requestBody.additionalData = {
		 "template@odata.bind" : "https://graph.microsoft.com/beta/teamsTemplates('standard')",
		 "group@odata.bind" : "https://graph.microsoft.com/beta/groups('71392b2f-1765-406e-86af-5907d9bdb2ab')"
	 }
const result = async () => {
	await graphServiceClient.teams.post(requestBody);
}


```