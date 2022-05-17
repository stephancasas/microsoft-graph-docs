---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Group();
const assignedlabel = new AssignedLabel();
assignedlabel.additionalData = {
					 "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
				 }
requestBody.assignedLabels = [
			assignedlabel
		]
const result = async () => {
	await graphServiceClient.groupsById("group-id").patch(requestBody);
}


```