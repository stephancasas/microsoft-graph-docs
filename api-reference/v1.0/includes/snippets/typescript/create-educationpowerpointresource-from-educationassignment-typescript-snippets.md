---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationAssignmentResource();
requestBody.distributeForStudentWork = false;
requestBody.resource = new EducationResource();
requestBody.resource.displayName = "state diagram.pptx";
requestBody.resource.additionalData = {
			 "@odata.type" : "microsoft.graph.educationPowerPointResource",
			 "fileUrl" : "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ"
		 }
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").resources.post(requestBody);
}


```