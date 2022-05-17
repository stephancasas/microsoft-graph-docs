---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new AccessReviewScheduleDefinition();
requestBody.displayName = "Test create";
requestBody.descriptionForAdmins = "New scheduled access review";
requestBody.descriptionForReviewers = "If you have any questions, contact jerry@contoso.com";
requestBody.scope = new AccessReviewScope();
requestBody.scope.additionalData = {
			 "@odata.type" : "#microsoft.graph.accessReviewQueryScope",
			 "query" : "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
			 "queryType" : "MicrosoftGraph"
		 }
const accessreviewreviewerscope = new AccessReviewReviewerScope();
accessreviewreviewerscope.additionalData = {
					 "query" : "/users/398164b1-5196-49dd-ada2-364b49f99b27",
					 "queryType" : "MicrosoftGraph"
				 }
requestBody.reviewers = [
			accessreviewreviewerscope
		]
requestBody.settings = new AccessReviewScheduleSettings();
requestBody.settings.mailNotificationsEnabled = true;
requestBody.settings.reminderNotificationsEnabled = true;
requestBody.settings.justificationRequiredOnApproval = true;
requestBody.settings.defaultDecisionEnabled = false;
requestBody.settings.defaultDecision = "None";
requestBody.settings.instanceDurationInDays = 1;
requestBody.settings.recommendationsEnabled = true;
requestBody.settings.recurrence = new PatternedRecurrence();
requestBody.settings.recurrence.pattern = new RecurrencePattern();
requestBody.settings.recurrence.pattern.type = RecurrencePatternType.Weekly;
requestBody.settings.recurrence.pattern.interval = 1;
requestBody.settings.recurrence.range = new RecurrenceRange();
requestBody.settings.recurrence.range.type = RecurrenceRangeType.NoEnd;
requestBody.settings.recurrence.range.startDate = "2020-09-08T12:02:30.667Z";
const result = async () => {
	await graphServiceClient.identityGovernance.accessReviews.definitions.post(requestBody);
}


```