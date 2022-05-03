---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationalActivity();
requestBody.institution = new InstitutionData();
requestBody.institution.location = new PhysicalAddress();
requestBody.institution.location.type = PhysicalAddressType.Business;
requestBody.institution.location.postOfficeBox = null,
requestBody.institution.location.street = "12000 E Prospect Rd";
requestBody.institution.location.city = "Fort Collins";
requestBody.institution.location.state = "Colorado";
requestBody.institution.location.countryOrRegion = "USA";
requestBody.institution.location.postalCode = "80525";
const result = async () => {
	await graphServiceClient.me.profile.educationalActivitiesById("educationalActivity-id").patch(requestBody);
}


```