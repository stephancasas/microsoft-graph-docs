---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new EducationAssignmentResource();
requestBody.distributeForStudentWork = false;
requestBody.resource = new EducationResource();
requestBody.resource.displayName = "Template - My Story";
requestBody.resource.additionalData = {
			 "appId" : "6fbeb90c-3d55-4bd5-82c4-bfe824be4300",
			 "appIconWebUrl" : "https://statics.teams.cdn.office.net/evergreen-assets/ThirdPartyApps/6fbeb90c-3d55-4bd5-82c4-bfe824be4300_largeImage.png?v=2.0.2",
			 "teamsEmbeddedContentUrl" : "https://app.api.edu.buncee.com/player/C7B0866C9B7E485EAE21AE14DBC3FD08?embed=1&render_slide_panel=1",
			 "webUrl" : "https://app.edu.buncee.com/buncee/C7B0866C9B7E485EAE21AE14DBC3FD08",
			 "@odata.type" : "#microsoft.graph.educationTeamsAppResource"
		 }
const result = async () => {
	await graphServiceClient.education.classesById("educationClass-id").assignmentsById("educationAssignment-id").resources.post(requestBody);
}


```