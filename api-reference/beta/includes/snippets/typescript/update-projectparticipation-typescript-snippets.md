---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ProjectParticipation();
requestBody.allowedAudiences = AllowedAudiences.Organization;
requestBody.client = new CompanyDetail();
requestBody.client.department = "Corporate Marketing";
requestBody.client.webUrl = "https://www.contoso.com";
const result = async () => {
	await graphServiceClient.me.profile.projectsById("projectParticipation-id").patch(requestBody);
}


```