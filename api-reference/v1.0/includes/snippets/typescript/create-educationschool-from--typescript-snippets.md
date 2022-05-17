---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationSchool();
requestBody.displayName = "String";
requestBody.description = "String";
requestBody.externalSource = EducationExternalSource.String;
requestBody.externalSourceDetail = "String";
requestBody.principalEmail = "String";
requestBody.principalName = "String";
requestBody.externalPrincipalId = "String";
requestBody.lowestGrade = "String";
requestBody.highestGrade = "String";
requestBody.schoolNumber = "String";
requestBody.externalId = "String";
requestBody.phone = "String";
requestBody.fax = "String";
requestBody.createdBy = new IdentitySet();
requestBody.createdBy.additionalData = {
			 "@odata.type" : "microsoft.graph.identitySet"
		 }
requestBody.address = new PhysicalAddress();
requestBody.address.additionalData = {
			 "@odata.type" : "microsoft.graph.physicalAddress"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.educationSchool"
	 }
const result = async () => {
	await graphServiceClient.education.schools.post(requestBody);
}


```