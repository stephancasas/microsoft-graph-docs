---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new BaseTask();
requestBody.textBody = "String";
requestBody.bodyLastModifiedDateTime =  new Date("String (timestamp)");
requestBody.completedDateTime =  new Date("String (timestamp)");
requestBody.dueDateTime = new DateTimeTimeZone();
requestBody.dueDateTime.additionalData = {
			 "@odata.type" : "microsoft.graph.dateTimeTimeZone"
		 }
requestBody.startDateTime = new DateTimeTimeZone();
requestBody.startDateTime.additionalData = {
			 "@odata.type" : "microsoft.graph.dateTimeTimeZone"
		 }
requestBody.importance = Importance.String;
requestBody.recurrence = new PatternedRecurrence();
requestBody.recurrence.additionalData = {
			 "@odata.type" : "microsoft.graph.patternedRecurrence"
		 }
requestBody.displayName = "String";
requestBody.status = TaskStatus_v2.String;
requestBody.viewpoint = new TaskViewpoint();
requestBody.viewpoint.additionalData = {
			 "@odata.type" : "microsoft.graph.taskViewpoint"
		 }
requestBody.additionalData = {
		 "@odata.type" : "#microsoft.graph.task"
	 }
const result = async () => {
	await graphServiceClient.me.tasks.listsById("baseTaskList-id").tasks.post(requestBody);
}


```