---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationUser();
requestBody.displayName = "Dion Matheson";
requestBody.givenName = "Dion";
requestBody.middleName = null,
requestBody.surname = "Matheson";
requestBody.mail = "DionM@contoso.com";
requestBody.mobilePhone = "+1 (253) 555-0101";
requestBody.createdBy = new IdentitySet();
requestBody.createdBy.user = new Identity();
requestBody.createdBy.user.displayName = "Susana Rocha";
requestBody.createdBy.user.id = "14012";
requestBody.externalSource = EducationExternalSource.Sis;
requestBody.mailingAddress = new PhysicalAddress();
requestBody.mailingAddress.city = "Los Angeles";
requestBody.mailingAddress.countryOrRegion = "United States";
requestBody.mailingAddress.postalCode = "98055";
requestBody.mailingAddress.state = "CA";
requestBody.mailingAddress.street = "12345 Main St.";
requestBody.primaryRole = EducationUserRole.Student;
requestBody.residenceAddress = new PhysicalAddress();
requestBody.residenceAddress.city = "Los Angeles";
requestBody.residenceAddress.countryOrRegion = "United States";
requestBody.residenceAddress.postalCode = "98055";
requestBody.residenceAddress.state = "CA";
requestBody.residenceAddress.street = "12345 Main St.";
const result = async () => {
	await graphServiceClient.education.users.post(requestBody);
}


```