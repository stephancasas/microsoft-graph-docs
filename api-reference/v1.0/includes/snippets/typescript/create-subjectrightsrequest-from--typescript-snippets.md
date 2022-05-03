---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new SubjectRightsRequest();
requestBody.type = SubjectRightsRequestType.Microsoft.graph.subjectRightsRequestType;
requestBody.dataSubjectType = DataSubjectType.Microsoft.graph.dataSubjectType;
requestBody.regulations = [
			"String"
		]
requestBody.displayName = "String";
requestBody.description = "String";
requestBody.internalDueDateTime =  new Date("String (timestamp)");
requestBody.dataSubject = new DataSubject();
requestBody.dataSubject.firstName = "String";
requestBody.dataSubject.lastName = "String";
requestBody.dataSubject.email = "String";
requestBody.dataSubject.residency = "String";
requestBody.dataSubject.additionalData = {
			 "phoneNumber" : "String",
			 "SSN" : "String"
		 }
const result = async () => {
	await graphServiceClient.privacy.subjectRightsRequests.post(requestBody);
}


```