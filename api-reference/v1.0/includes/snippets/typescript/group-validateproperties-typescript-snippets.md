---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = GraphServiceClient.init({authProvider});

const requestBody = new ValidatePropertiesRequestBody();
requestBody.displayName = "Myprefix_test_mysuffix";
requestBody.mailNickname = "Myprefix_test_mysuffix";
requestBody.onBehalfOfUserId = "onBehalfOfUserId-value";
async () => {
	await graphServiceClient.groupsById("group-id").validateProperties.post(requestBody);
}


```