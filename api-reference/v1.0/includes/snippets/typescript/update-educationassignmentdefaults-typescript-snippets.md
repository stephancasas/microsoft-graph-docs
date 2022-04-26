---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationAssignmentDefaults();
requestBody.addedStudentAction = EducationAddedStudentAction.AssignIfOpen;
requestBody.notificationChannelUrl = "https://graph.microsoft.com/beta/teams('acdefc6b-2dc6-4e71-b1e9-6d9810ab1793')/channels('3da03fc4-8eac-4459-84fb-1422dc01f65e')";
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentDefaults.patch(requestBody);
}


```