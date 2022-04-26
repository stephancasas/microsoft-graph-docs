---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ProjectParticipation();
requestBody.categories = [
			"Branding"
		]
requestBody.client = new CompanyDetail();
requestBody.client.displayName = "Contoso Ltd.";
requestBody.client.department = "Corporate Marketing";
requestBody.client.webUrl = "https://www.contoso.com";
requestBody.displayName = "Contoso Re-branding Project";
requestBody.detail = new PositionDetail();
requestBody.detail.company = new CompanyDetail();
requestBody.detail.company.displayName = "Adventureworks Inc.";
requestBody.detail.company.department = "Consulting";
requestBody.detail.company.webUrl = "https://adventureworks.com";
requestBody.detail.description = "Rebranding of Contoso Ltd.";
requestBody.detail.jobTitle = "Lead PM Rebranding";
requestBody.detail.role = "project management";
requestBody.detail.summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization.";
const result = async () => {
	await graphServiceClient.me.profile.projects.post(requestBody);
}


```