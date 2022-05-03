---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationSchool();
requestBody.displayName = "Fabrikam High School";
requestBody.description = "Magnate school for the arts. Los Angeles School District";
requestBody.externalSource = EducationExternalSource.String;
requestBody.principalEmail = "AmyR@fabrikam.com";
requestBody.principalName = "Amy Roebuck";
requestBody.externalPrincipalId = "14007";
requestBody.highestGrade = "12";
requestBody.lowestGrade = "9";
requestBody.schoolNumber = "10002";
requestBody.address = new PhysicalAddress();
requestBody.address.city = "Los Angeles";
requestBody.address.countryOrRegion = "United States";
requestBody.address.postalCode = "98055";
requestBody.address.state = "CA";
requestBody.address.street = "12345 Main St.";
requestBody.externalId = "10002";
requestBody.phone = "+1 (253) 555-0102";
const result = async () => {
	await graphServiceClient.education.schools.post(requestBody);
}


```