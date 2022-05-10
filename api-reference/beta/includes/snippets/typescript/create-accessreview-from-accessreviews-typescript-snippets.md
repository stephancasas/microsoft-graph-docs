---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessReview();
requestBody.displayName = "TestReview";
requestBody.startDateTime =  new Date("2017-02-10T00:35:53.214Z");
requestBody.endDateTime =  new Date("2017-03-12T00:35:53.214Z");
requestBody.reviewedEntity = new Identity();
requestBody.reviewedEntity.id = "99025615-a0b1-47ec-9117-35377b10998b";
requestBody.reviewerType = "delegated";
requestBody.businessFlowTemplateId = "6e4f3d20-c5c3-407f-9695-8460952bcc68";
requestBody.description = "Sample description";
const accessreviewreviewer = new AccessReviewReviewer();
accessreviewreviewer.additionalData = {
					 "id" : "f260246a-09b1-4fd5-8d18-daed736071ec"
				 }
const accessreviewreviewer1 = new AccessReviewReviewer();
accessreviewreviewer1.additionalData = {
					 "id" : "5a4e184c-4ee5-4883-96e9-b371f8da88e3"
				 }
requestBody.reviewers = [
			accessreviewreviewer,
			accessreviewreviewer1
		]
requestBody.settings = new AccessReviewSettings();
requestBody.settings.mailNotificationsEnabled = true;
requestBody.settings.remindersEnabled = true;
requestBody.settings.justificationRequiredOnApproval = true;
requestBody.settings.autoReviewEnabled = false;
requestBody.settings.activityDurationInDays = 30;
requestBody.settings.autoApplyReviewResultsEnabled = false;
requestBody.settings.accessRecommendationsEnabled = false;
requestBody.settings.recurrenceSettings = new AccessReviewRecurrenceSettings();
requestBody.settings.recurrenceSettings.recurrenceType = "onetime";
requestBody.settings.recurrenceSettings.recurrenceEndType = "endBy";
requestBody.settings.recurrenceSettings.durationInDays = 0;
requestBody.settings.recurrenceSettings.recurrenceCount = 0;
requestBody.settings.autoReviewSettings = new AutoReviewSettings();
requestBody.settings.autoReviewSettings.notReviewedResult = "Deny";
const result = async () => {
	await graphServiceClient.accessReviews.post(requestBody);
}


```