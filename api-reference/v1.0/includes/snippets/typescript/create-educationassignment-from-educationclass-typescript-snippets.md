---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationAssignment();
requestBody.dueDateTime =  new Date("2021-09-07T00:00:00Z");
requestBody.displayName = "Reading test 09.03 #4";
requestBody.instructions = new EducationItemBody();
requestBody.instructions.contentType = BodyType.Text;
requestBody.instructions.content = "Read chapter 4";
requestBody.grading = new EducationAssignmentGradeType();
requestBody.grading.additionalData = {
			 "@odata.type" : "#microsoft.graph.educationAssignmentPointsGradeType",
			 "maxPoints" : 50
		 }
requestBody.assignTo = new EducationAssignmentRecipient();
requestBody.assignTo.additionalData = {
			 "@odata.type" : "#microsoft.graph.educationAssignmentClassRecipient"
		 }
requestBody.status = EducationAssignmentStatus.Draft;
requestBody.allowStudentsToAddResourcesToSubmission = true;
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignments.post(requestBody);
}


```