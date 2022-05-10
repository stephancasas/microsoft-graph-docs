---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new Extension();
requestBody.additionalData = {
		 "@odata.type" : "Microsoft.OutlookServices.OpenTypeExtension",
		 "extensionName" : "Com.Contoso.Estimate",
		 "companyName" : "Contoso",
		 "expirationDate" : "2016-07-30T11:00:00.000Z",
		 "DealValue" : 1010100,
		 "topPicks" : [
				"Employees only",
				"Add spouse or guest",
				"Add family"
			]
	 }
const result = async () => {
	await graphServiceClient.groupsById("group-id").threadsById("conversationThread-id").postsById("post-id").extensionsById("extension-id").patch(requestBody);
}


```