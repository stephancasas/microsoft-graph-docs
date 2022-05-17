---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationalActivity();
requestBody.completionMonthYear = "Date";
requestBody.endMonthYear = "Date";
requestBody.institution = new InstitutionData();
requestBody.institution.description = null,
requestBody.institution.displayName = "Colorado State University";
requestBody.institution.location = new PhysicalAddress();
requestBody.institution.location.type = PhysicalAddressType.Business;
requestBody.institution.location.postOfficeBox = null,
requestBody.institution.location.street = "12000 E Prospect Rd";
requestBody.institution.location.city = "Fort Collins";
requestBody.institution.location.state = "Colorado";
requestBody.institution.location.countryOrRegion = "USA";
requestBody.institution.location.postalCode = "80525";
requestBody.institution.webUrl = "https://www.colostate.edu";
requestBody.program = new EducationalActivityDetail();
requestBody.program.abbreviation = "MBA";
requestBody.program.activities = null,
requestBody.program.awards = null,
requestBody.program.description = "Master of Business Administration with a major in Entreprenuership and Finance.";
requestBody.program.displayName = "Master of Business Administration";
requestBody.program.fieldsOfStudy = null,
requestBody.program.grade = "3.9";
requestBody.program.notes = null,
requestBody.program.webUrl = "https://biz.colostate.edu";
requestBody.startMonthYear = "Date";
const result = async () => {
	await graphServiceClient.me.profile.educationalActivities.post(requestBody);
}


```