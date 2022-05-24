---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SubjectRightsRequest();
requestBody.type = SubjectRightsRequestType.Export;
requestBody.contentQuery = "(("Diego Siciliani" OR "Diego.Siciliani@contoso.com") OR (participants:"Diego.Siciliani@contoso.com"))";
requestBody.dataSubjectType = DataSubjectType.Customer;
requestBody.externalId = "F53BF2DA-607D-412A-B568-FAA0F023AC0B";
requestBody.displayName = "Export report for customer Id: 12345";
requestBody.description = "This is a export request";
requestBody.includeAllVersions = false;
requestBody.includeAuthoredContent = true;
requestBody.internalDueDateTime =  new Date("2022-07-20T22:42:28Z");
requestBody.dataSubject = new DataSubject();
requestBody.dataSubject.firstName = "Diego";
requestBody.dataSubject.lastName = "Siciliani";
requestBody.dataSubject.email = "Diego.Siciliani@contoso.com";
requestBody.dataSubject.residency = "USA";
requestBody.mailboxLocations = null,
requestBody.pauseAfterEstimate = true;
requestBody.regulations = [
			"CCPA"
		]
requestBody.siteLocations = new SubjectRightsRequestSiteLocation();
requestBody.siteLocations.additionalData = {
			 "@odata.type" : "microsoft.graph.subjectRightsRequestAllSiteLocation"
		 }
const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequests.post(requestBody);
}


```