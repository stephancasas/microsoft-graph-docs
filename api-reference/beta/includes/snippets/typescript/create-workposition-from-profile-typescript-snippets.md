---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new WorkPosition();
requestBody.detail = new PositionDetail();
requestBody.detail.company = new CompanyDetail();
requestBody.detail.company.displayName = "Adventureworks Ltd.";
requestBody.detail.company.department = "Consulting";
requestBody.detail.company.officeLocation = "AW23/344";
requestBody.detail.company.address = new PhysicalAddress();
requestBody.detail.company.address.type = PhysicalAddressType.Business;
requestBody.detail.company.address.street = "123 Patriachy Ponds";
requestBody.detail.company.address.city = "Moscow";
requestBody.detail.company.address.countryOrRegion = "Russian Federation";
requestBody.detail.company.address.postalCode = "RU-34621";
requestBody.detail.company.webUrl = "https://www.adventureworks.com";
requestBody.detail.jobTitle = "Senior Product Branding Manager II";
requestBody.detail.role = "consulting";
requestBody.isCurrent = true;
const result = async () => {
	await graphServiceClient.me.profile.positions.post(requestBody);
}


```