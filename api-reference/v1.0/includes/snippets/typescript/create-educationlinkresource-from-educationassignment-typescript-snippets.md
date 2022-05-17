---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationAssignmentResource();
requestBody.distributeForStudentWork = false;
requestBody.resource = new EducationResource();
requestBody.resource.displayName = "Where the Wonders of Learning Never Cease | Wonderopolis";
requestBody.resource.additionalData = {
			 "link" : "https://wonderopolis.org/",
			 "thumbnailPreviewUrl" : null,
			 "@odata.type" : "#microsoft.graph.educationLinkResource"
		 }
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").resources.post(requestBody);
}


```